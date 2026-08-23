---
title: "Instalação"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code só é necessário para status ao vivo e prévia de GUI pelo Nexora Connect."
icon: package
---

Pare o servidor, copie NexoraEngine.jar para plugins, inicie com java -jar server.jar nogui, guarde o token inicial exibido uma única vez e coloque cada workspace em plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
