---
title: "Cấu trúc workspace"
description: "Tên thư mục phải trùng với id manifest. Entry phải là .js hoặc .mjs. Import JavaScript/JSON tương đối bị giới hạn trong workspace; thư mục ẩn, nodemodules, dist và TypeScript bị bỏ…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## Script đầu tiên

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
