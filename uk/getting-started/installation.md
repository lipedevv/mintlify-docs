---
title: "Встановлення"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code потрібен лише для live-стану чи перегляду GUI у Nexora Connect."
icon: package
---

Зупиніть сервер, скопіюйте NexoraEngine.jar до plugins, запустіть java -jar server.jar nogui, збережіть початковий токен, що показується один раз, і покладіть workspace у plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
