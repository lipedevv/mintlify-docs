---
title: "Cài đặt"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code chỉ cần khi dùng trạng thái trực tiếp hoặc xem trước GUI của Nexora Connect."
icon: package
---

Dừng máy chủ, chép NexoraEngine.jar vào plugins, chạy java -jar server.jar nogui, lưu token ban đầu chỉ hiện một lần và đặt workspace trong plugins/NexoraEngine/workspaces.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
