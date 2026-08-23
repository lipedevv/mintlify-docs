---
title: "Installatie"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code is alleen nodig voor live status of GUI-preview met Nexora Connect."
icon: package
---

Stop de server, kopieer NexoraEngine.jar naar plugins, start met java -jar server.jar nogui, bewaar het eenmalig getoonde initiële token en plaats workspaces onder plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
