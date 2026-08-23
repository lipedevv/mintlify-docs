---
title: "GUI Shop"
description: "Межі: 1–6 рядів скрині, кількість 1–99, 20 tick/с, HTTP 100–60000 мс і до 100 SQL-операцій у транзакції. Цей випуск реалізує лише GUI скрині."
icon: shopping-cart
---

This transaction-safe example checks inventory space, conditionally debits integer cents, delivers once and refunds when delivery becomes impossible.

```js
await database.execute("CREATE TABLE IF NOT EXISTS accounts (uuid TEXT PRIMARY KEY, cents INTEGER NOT NULL CHECK(cents >= 0))");

const shop = gui.chest({ id: "shop", title: "<gold>Shop</gold>", rows: 3 });
shop.slot(13, item("DIAMOND", { name: "<aqua>Diamond</aqua>" }), async ({ player }) => {
  const product = item("DIAMOND");
  if (!player.inventory.canFit(product)) {
    player.send("<red>Your inventory is full.</red>");
    return;
  }
  const result = await database.transaction([
    { sql: "UPDATE accounts SET cents = cents - ? WHERE uuid = ? AND cents >= ?",
      parameters: [5000, player.uuid, 5000], maximumAffectedRows: 1 }
  ]);
  if (result.affectedRows[0] !== 1) return;
  if (!player.online || !player.inventory.tryAdd(product)) {
    await database.transaction([
      { sql: "UPDATE accounts SET cents = cents + ? WHERE uuid = ?",
        parameters: [5000, player.uuid], minimumAffectedRows: 1, maximumAffectedRows: 1 }
    ]);
    return;
  }
  player.send("<green>Purchase complete.</green>");
});

command("shop", { playerOnly: true, execute({ player }) { shop.open(player); } });

const task = scheduler.repeat(20, () => log.debug("one second"));
const value = await storage.get("example", { visits: 0 });
await storage.set("example", { visits: value.visits + 1 });
const response = await http.get("https://example.com/api", { timeout: 5000 });
```

> Always validate online state, balance and inventory again inside the click callback. Never trust the GUI item as transaction state.
