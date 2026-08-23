---
title: "Struktura workspace"
description: "Název složky se musí rovnat id manifestu. Entry musí být .js nebo .mjs. Relativní JavaScript/JSON importy zůstávají ve workspace; skryté složky, nodemodules, dist a TypeScript se…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## První skript

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
