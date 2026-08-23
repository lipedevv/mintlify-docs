---
title: "โครงสร้าง Workspace"
description: "ชื่อโฟลเดอร์ต้องตรงกับ id ใน manifest และ entry ต้องเป็น .js หรือ .mjs การ import JavaScript/JSON แบบ relative ถูกจำกัดใน Workspace; โฟลเดอร์ซ่อน, nodemodules, dist และ TypeScript…"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## สคริปต์แรก

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
