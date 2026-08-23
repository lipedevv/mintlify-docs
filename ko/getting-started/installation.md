---
title: "설치"
description: "Paper 1.20.6–26.2 · Java 21 (Paper 1.20.6–1.21.11) · Java 25 (Paper 26.x). VS Code는 Nexora Connect의 실시간 상태 또는 GUI 미리보기에만 필요합니다."
icon: package
---

서버를 중지하고 NexoraEngine.jar를 plugins에 복사한 뒤 java -jar server.jar nogui로 시작하십시오. 콘솔에 한 번만 표시되는 초기 토큰을 보관하고 workspace를 plugins/NexoraEngine/workspaces에 넣으십시오.

## Nexora Connect

VS Code → Extensions → Install from VSIX → `nexora-connect.vsix`. Run `Nexora: Connect` and enter the initial token. `Nexora: Open GUI Preview` previews an open `.gui.js` file. Source files are never deployed by the extension; saving them triggers the engine's automatic reload.
