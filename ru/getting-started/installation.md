---
title: "Установка"
description: "Поддерживаемая цель: Paper 1.21.8 и Java 21 или новее. VS Code нужен Nexora Connect только для живого состояния и предпросмотра GUI."
icon: package
---

Остановите сервер, поместите NexoraEngine.jar в plugins, запустите java -jar server.jar nogui, сохраните показанный один раз начальный токен и разместите workspace в plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
