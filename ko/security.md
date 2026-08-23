---
title: "보안 및 Native Mode"
description: "Safe Mode는 HostAccess.NONE으로 시작합니다. 127.0.0.1과 인증을 유지하고 최소 capability만 사용하며 신뢰하지 않는 코드에 native.java/native.paper를 주지 마십시오."
icon: shield-check
---

Native Mode must be enabled in both `config.yml` and `workspace.json`. Treat a native workspace exactly like a Java plugin and review all of its source before enabling it.
