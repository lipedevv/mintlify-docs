---
title: "Telepítés"
description: "Támogatott cél: Paper 1.21.8 és Java 21 vagy újabb. VS Code csak a Nexora Connect élő állapotához vagy GUI előnézetéhez kell."
icon: package
---

Állítsd le a szervert, másold a NexoraEngine.jar fájlt a plugins mappába, indítsd java -jar server.jar nogui paranccsal, őrizd meg az egyszer megjelenő kezdeti tokent, és tedd a workspace mappákat a plugins/NexoraEngine/workspaces alá.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
