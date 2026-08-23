---
title: "Inštalácia"
description: "Podporovaný cieľ: Paper 1.21.8 a Java 21 alebo novšia. VS Code je potrebný len pre živý stav alebo náhľad GUI v Nexora Connect."
icon: package
---

Zastavte server, skopírujte NexoraEngine.jar do plugins, spustite java -jar server.jar nogui, uložte počiatočný token zobrazený iba raz a vložte workspace do plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
