---
title: "문제 해결 및 운영 체크리스트"
description: "변경이 거부되면 첫 workspace 경고를 수정하고 리비전을 삭제하지 마십시오. 포트가 사용 중이면 이전 프로세스를 종료하고 같은 월드로 Paper 두 개를 실행하지 말며 Windows에서는 nogui를 사용하십시오."
icon: wrench
---

## Production checklist

운영 전 workspaces/storage 백업, 시작/중지, 권한, 가득 찬 인벤토리와 잔액 부족을 테스트하고 토큰을 보호하며 광고한 정확한 Paper 빌드를 검증하십시오.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
