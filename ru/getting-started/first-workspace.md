---
title: "Структура workspace"
description: "Имя папки должно совпадать с id манифеста. Точка входа — .js или .mjs. Относительные JavaScript/JSON-импорты не выходят за workspace; скрытые папки, nodemodules, dist и TypeScript…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Первый скрипт

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
