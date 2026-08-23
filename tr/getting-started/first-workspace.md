---
title: "Workspace yapısı"
description: "Klasör adı manifest id ile aynı olmalıdır. Giriş .js veya .mjs olmalıdır. Göreli JavaScript/JSON içe aktarımları workspace içinde kalır; gizli klasörler, nodemodules, dist ve…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## İlk script

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
