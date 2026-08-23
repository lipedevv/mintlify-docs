---
title: "Struktur workspace"
description: "Nama folder harus sama dengan id manifest. Entry harus .js atau .mjs. Impor JavaScript/JSON relatif dibatasi dalam workspace; folder tersembunyi, nodemodules, dist, dan TypeScript…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Skrip pertama

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
