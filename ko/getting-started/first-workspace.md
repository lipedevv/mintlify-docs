---
title: "Workspace 구조"
description: "폴더 이름은 매니페스트 id와 같아야 합니다. entry는 .js 또는 .mjs여야 합니다. 상대 JavaScript/JSON 가져오기는 workspace 내부로 제한되며 숨김 폴더, nodemodules, dist, TypeScript는 무시됩니다."
icon: rocket
---

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## 첫 스크립트

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
