---
title: "Installation"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code kræves kun til live-status eller GUI-preview med Nexora Connect."
icon: package
---

Stop serveren, kopier NexoraEngine.jar til plugins, start med java -jar server.jar nogui, gem den første token som kun vises én gang, og læg workspaces under plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
