---
title: "Installation"
description: "Mål som stöds: Paper 1.21.8 och Java 21 eller senare. VS Code behövs endast för live-status eller GUI-förhandsvisning med Nexora Connect."
icon: package
---

Stoppa servern, kopiera NexoraEngine.jar till plugins, starta med java -jar server.jar nogui, spara den initiala token som visas en gång och placera workspaces under plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
