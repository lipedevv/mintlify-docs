---
title: "Установка"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code нужен Nexora Connect только для живого состояния и предпросмотра GUI."
icon: package
---

Остановите сервер, поместите NexoraEngine.jar в plugins, запустите java -jar server.jar nogui, сохраните показанный один раз начальный токен и разместите workspace в plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
