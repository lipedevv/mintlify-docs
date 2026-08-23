---
title: "Instalace"
description: "Podporovaný cíl: Paper 1.21.8 a Java 21 nebo novější. VS Code je nutný pouze pro živý stav nebo náhled GUI v Nexora Connect."
icon: package
---

Zastavte server, zkopírujte NexoraEngine.jar do plugins, spusťte java -jar server.jar nogui, uložte počáteční token zobrazený jen jednou a vložte workspace do plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
