---
title: "Workspace-struktur"
description: "Mappnamnet måste matcha manifestets id. Entry måste vara .js eller .mjs. Relativa JavaScript/JSON-importer stannar i workspace; dolda mappar, nodemodules, dist och TypeScript…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Första skriptet

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
