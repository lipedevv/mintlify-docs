---
title: "Structura workspace"
description: "Numele folderului trebuie să coincidă cu id-ul manifestului. Entry trebuie să fie .js sau .mjs. Importurile JavaScript/JSON relative rămân în workspace; folderele ascunse,…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Primul script

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
