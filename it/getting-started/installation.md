---
title: "Installazione"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code serve solo per stato live e anteprima GUI di Nexora Connect."
icon: package
---

Arresta il server, copia NexoraEngine.jar in plugins, avvia con java -jar server.jar nogui, conserva il token iniziale mostrato una sola volta e inserisci i workspace in plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
