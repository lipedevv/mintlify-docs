---
title: "Workspace structure"
description: "The directory name must equal the manifest id. The entry must be .js or .mjs. Relative JavaScript and JSON imports stay inside the workspace; hidden folders, nodemodules, dist and…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## First script

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
