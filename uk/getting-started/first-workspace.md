---
title: "Структура workspace"
description: "Назва папки має збігатися з id маніфесту. Entry повинен бути .js або .mjs. Відносні JavaScript/JSON імпорти залишаються в workspace; приховані папки, nodemodules, dist і TypeScript…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Перший скрипт

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
