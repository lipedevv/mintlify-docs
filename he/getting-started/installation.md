---
title: "התקנה"
description: "יעד נתמך: Paper 1.21.8 ו-Java 21 ומעלה. VS Code נדרש רק למצב חי או תצוגה מקדימה של GUI דרך Nexora Connect."
icon: package
---

<div dir="rtl">

# 📦 התקנה

עצרו את השרת, העתיקו NexoraEngine.jar אל plugins, הפעילו java -jar server.jar nogui, שמרו את ה-token הראשוני שמוצג פעם אחת, והניחו Workspaces תחת plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.

</div>
