---
title: "Workspace の構成"
description: "フォルダー名はマニフェスト id と一致する必要があります。entry は .js または .mjs です。相対 JavaScript/JSON import は Workspace 内に制限され、隠しフォルダー、nodemodules、dist、TypeScript は無視されます。"
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## 最初のスクリプト

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
