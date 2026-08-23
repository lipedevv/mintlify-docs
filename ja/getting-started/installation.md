---
title: "インストール"
description: "対応対象は Paper 1.21.8 と Java 21 以降です。VS Code は Nexora Connect のライブ状態または GUI プレビューを使う場合のみ必要です。"
icon: package
---

サーバーを停止し、NexoraEngine.jar を plugins にコピーし、java -jar server.jar nogui で起動します。一度だけ表示される初期トークンを保存し、Workspace を plugins/NexoraEngine/workspaces に配置します。

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
