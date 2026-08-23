---
title: "자동 다시 로드"
description: "workspace.json, .js, .mjs 또는 로컬 .json을 저장하면 검증합니다. 후보 리비전을 격리 준비한 뒤 Paper 메인 스레드에서 교체합니다. 실패하면 마지막 정상 리비전이 유지됩니다."
icon: refresh-cw
---

> Saving `workspace.json`, `.js`, `.mjs` or local `.json` files is enough. There is no Deploy Workspace command.

변경이 거부되면 첫 workspace 경고를 수정하고 리비전을 삭제하지 마십시오. 포트가 사용 중이면 이전 프로세스를 종료하고 같은 월드로 Paper 두 개를 실행하지 말며 Windows에서는 nogui를 사용하십시오.
