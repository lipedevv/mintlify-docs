---
title: "Installation"
description: "Cible prise en charge : Paper 1.21.8 et Java 21 ou plus récent. VS Code n’est requis que pour l’état en direct et l’aperçu GUI de Nexora Connect."
icon: package
---

Arrêtez le serveur, copiez NexoraEngine.jar dans plugins, lancez java -jar server.jar nogui, conservez le jeton initial affiché une seule fois et placez les workspaces dans plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
