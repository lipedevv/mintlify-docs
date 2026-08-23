---
title: "Instalare"
description: "Țintă suportată: Paper 1.21.8 și Java 21 sau mai nou. VS Code este necesar doar pentru starea live sau previzualizarea GUI din Nexora Connect."
icon: package
---

Oprește serverul, copiază NexoraEngine.jar în plugins, pornește cu java -jar server.jar nogui, păstrează tokenul inițial afișat o singură dată și pune workspace-urile în plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
