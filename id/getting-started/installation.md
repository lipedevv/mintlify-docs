---
title: "Instalasi"
description: "Target yang didukung: Paper 1.21.8 dan Java 21 atau lebih baru. VS Code hanya diperlukan untuk status langsung atau pratinjau GUI Nexora Connect."
icon: package
---

Hentikan server, salin NexoraEngine.jar ke plugins, mulai dengan java -jar server.jar nogui, simpan token awal yang hanya ditampilkan sekali, lalu taruh workspace di plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
