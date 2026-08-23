---
title: "Struktura workspace"
description: "Nazwa folderu musi odpowiadać id manifestu. Plik wejściowy musi mieć .js lub .mjs. Importy względne JavaScript/JSON pozostają w workspace; ukryte foldery, nodemodules, dist i…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Pierwszy skrypt

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
