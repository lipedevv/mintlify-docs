---
title: "Instalación"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code solo para estado en vivo o vista previa de GUI."
icon: package
---

Detén el servidor, copia NexoraEngine.jar en plugins, inicia con java -jar server.jar nogui, guarda el token inicial mostrado una sola vez y coloca cada workspace en plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
