---
title: "Workspace-structuur"
description: "De mapnaam moet gelijk zijn aan de manifest-id. De entry moet .js of .mjs zijn. Relatieve JavaScript/JSON-imports blijven in de workspace; verborgen mappen, nodemodules, dist en…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Eerste script

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
