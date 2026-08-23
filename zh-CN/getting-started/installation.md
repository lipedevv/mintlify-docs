---
title: "安装"
description: "支持目标：Paper 1.21.8 与 Java 21 或更高版本。只有使用 Nexora Connect 的实时状态或 GUI 预览时才需要 VS Code。"
icon: package
---

停止服务器，将 NexoraEngine.jar 复制到 plugins，使用 java -jar server.jar nogui 启动，保存控制台仅显示一次的初始令牌，并将 workspace 放入 plugins/NexoraEngine/workspaces。

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
