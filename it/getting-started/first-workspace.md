---
title: "Struttura del workspace"
description: "Il nome della cartella deve coincidere con l’id del manifest. L’entry deve essere .js o .mjs. Gli import JavaScript/JSON relativi restano nel workspace; cartelle nascoste,…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Primo script

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
