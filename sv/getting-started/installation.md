---
title: "Installation"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code behövs endast för live-status eller GUI-förhandsvisning med Nexora Connect."
icon: package
---

Stoppa servern, kopiera NexoraEngine.jar till plugins, starta med java -jar server.jar nogui, spara den initiala token som visas en gång och placera workspaces under plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
