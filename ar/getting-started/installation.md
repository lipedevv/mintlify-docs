---
title: "التثبيت"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code فقط للحالة المباشرة أو معاينة GUI عبر Nexora Connect."
icon: package
---

<div dir="rtl">

# 📦 التثبيت

أوقف الخادم، وانسخ NexoraEngine.jar إلى plugins، وشغّل java -jar server.jar nogui، واحفظ الرمز الأولي الذي يظهر مرة واحدة، ثم ضع مساحات العمل في plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.

</div>
