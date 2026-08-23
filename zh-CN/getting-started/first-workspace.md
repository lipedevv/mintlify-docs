---
title: "Workspace 结构"
description: "目录名必须与清单 id 相同。入口必须是 .js 或 .mjs。相对 JavaScript/JSON 导入被限制在 workspace 内；隐藏目录、nodemodules、dist 和 TypeScript 会被忽略。"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## 第一个脚本

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
