---
title: "Kurulum"
description: "Desteklenen hedef: Paper 1.21.8 ve Java 21 veya üzeri. VS Code yalnızca Nexora Connect canlı durum ve GUI önizlemesi için gerekir."
icon: package
---

Sunucuyu durdurun, NexoraEngine.jar dosyasını plugins klasörüne kopyalayın, java -jar server.jar nogui ile başlatın, yalnızca bir kez gösterilen ilk tokenı saklayın ve workspace’leri plugins/NexoraEngine/workspaces altına koyun.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
