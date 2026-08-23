---
title: "Štruktúra workspace"
description: "Názov priečinka musí zodpovedať id manifestu. Entry musí byť .js alebo .mjs. Relatívne JavaScript/JSON importy zostávajú vo workspace; skryté priečinky, nodemodules, dist a…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Prvý skript

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
