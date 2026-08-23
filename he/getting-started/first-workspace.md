---
title: "מבנה Workspace"
description: "שם התיקייה חייב להתאים ל-id במניפסט. entry חייב להיות .js או .mjs. ייבואי JavaScript/JSON יחסיים נשארים בתוך ה-Workspace; תיקיות מוסתרות, nodemodules, dist ו-TypeScript נזנחים."
icon: rocket
---

<div dir="rtl">

# 🚀 מבנה Workspace

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## הסקריפט הראשון

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

</div>
