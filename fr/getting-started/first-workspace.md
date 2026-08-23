---
title: "Structure du workspace"
description: "Le dossier doit porter le même nom que l’id du manifeste. L’entrée doit être .js ou .mjs. Les imports JavaScript/JSON relatifs restent dans le workspace ; dossiers cachés,…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Premier script

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
