---
title: "Instalare"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code este necesar doar pentru starea live sau previzualizarea GUI din Nexora Connect."
icon: package
---

Oprește serverul, copiază NexoraEngine.jar în plugins, pornește cu java -jar server.jar nogui, păstrează tokenul inițial afișat o singură dată și pune workspace-urile în plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
