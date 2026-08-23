---
title: "Kurulum"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code yalnızca Nexora Connect canlı durum ve GUI önizlemesi için gerekir."
icon: package
---

Sunucuyu durdurun, NexoraEngine.jar dosyasını plugins klasörüne kopyalayın, java -jar server.jar nogui ile başlatın, yalnızca bir kez gösterilen ilk tokenı saklayın ve workspace’leri plugins/NexoraEngine/workspaces altına koyun.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
