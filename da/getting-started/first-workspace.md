---
title: "Workspace-struktur"
description: "Mappenavnet skal matche manifestets id. Entry skal være .js eller .mjs. Relative JavaScript/JSON-imports bliver i workspace; skjulte mapper, nodemodules, dist og TypeScript…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Første script

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
