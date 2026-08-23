---
title: "Workspace felépítése"
description: "A mappanév egyezzen a manifest id értékével. Az entry .js vagy .mjs legyen. A relatív JavaScript/JSON importok a workspace-ben maradnak; a rejtett mappák, nodemodules, dist és…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Első szkript

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
