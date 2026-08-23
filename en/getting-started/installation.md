---
title: "Installation"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code only when live status or GUI preview is wanted."
icon: package
---

Stop the server, copy NexoraEngine.jar into plugins, start with java -jar server.jar nogui, save the initial token shown once in the console, and place each workspace below plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
