---
title: "Встановлення"
description: "Підтримувана ціль: Paper 1.21.8 та Java 21 або новіша. VS Code потрібен лише для live-стану чи перегляду GUI у Nexora Connect."
icon: package
---

Зупиніть сервер, скопіюйте NexoraEngine.jar до plugins, запустіть java -jar server.jar nogui, збережіть початковий токен, що показується один раз, і покладіть workspace у plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
