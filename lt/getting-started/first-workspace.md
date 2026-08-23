---
title: "Workspace struktūra"
description: "Aplanko pavadinimas turi sutapti su manifesto id. Entry turi būti .js arba .mjs. Santykiniai JavaScript/JSON importai lieka workspace; paslėpti aplankai, nodemodules, dist ir…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Pirmasis skriptas

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
