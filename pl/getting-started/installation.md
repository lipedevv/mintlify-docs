---
title: "Instalacja"
description: "Wspierany cel: Paper 1.21.8 oraz Java 21 lub nowsza. VS Code jest potrzebny tylko do statusu na żywo i podglądu GUI w Nexora Connect."
icon: package
---

Zatrzymaj serwer, skopiuj NexoraEngine.jar do plugins, uruchom java -jar server.jar nogui, zachowaj początkowy token pokazany tylko raz i umieść workspace w plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
