---
title: "安装"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code。"
icon: package
---

停止服务器，将 NexoraEngine.jar 复制到 plugins，使用 java -jar server.jar nogui 启动，保存控制台仅显示一次的初始令牌，并将 workspace 放入 plugins/NexoraEngine/workspaces。

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
