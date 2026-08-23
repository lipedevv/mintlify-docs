---
title: "Installation"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code wird für Nexora Connect nur für Live-Status oder GUI-Vorschau benötigt."
icon: package
---

Server stoppen, NexoraEngine.jar nach plugins kopieren, mit java -jar server.jar nogui starten, den einmal angezeigten Start-Token sichern und Workspaces unter plugins/NexoraEngine/workspaces ablegen.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
