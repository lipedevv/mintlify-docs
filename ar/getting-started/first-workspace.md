---
title: "بنية مساحة العمل"
description: "يجب أن يطابق اسم المجلد id في البيان، وأن يكون entry بصيغة .js أو .mjs. تبقى استيرادات JavaScript/JSON النسبية داخل مساحة العمل؛ ويتم تجاهل المجلدات المخفية وnodemodules وdist…"
icon: rocket
---

<div dir="rtl">

# 🚀 بنية مساحة العمل

```text
plugins/NexoraEngine/workspaces/my-workspace/
├── workspace.json
├── index.js
└── services/
```

## أول سكربت

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
