---
title: "Sự kiện"
description: "Options: { id?, priority?, ignoreCancelled?, filter? }. Safe Mode uses the stable names above; fully-qualified Bukkit/Paper classes require Native Mode and native.paper."
icon: terminal
---

```js
on("playerJoin", ({ player }) => {
  player.send("<green>Welcome to Nexora!</green>");
});

command("heal", {
  permission: "example.heal",
  playerOnly: true,
  execute({ player }) {
    player.heal();
    player.send("<green>Healed.</green>");
  }
});
```

## CommandDefinition

| Field | Type |
| --- | --- |
| aliases | string[] |
| permission | string |
| description | string |
| usage | string |
| playerOnly | boolean |
| execute(context) | void &#124; Promise&lt;void&gt; |
| suggest(context) | string[]; synchronous and permission-aware |

## Sự kiện

| Event | Data |
| --- | --- |
| playerJoin | player |
| playerQuit | player, reason |
| playerDeath | player, message |
| blockBreak | player, block |
| blockPlace | player, block |
| playerChat | player, message |
| entityDamage | entity, damager?, damage, cause |
| inventoryClick | player, slot, click |
| inventoryClose | player |
