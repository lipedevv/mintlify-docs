---
title: "安全与原生模式"
description: "安全模式以 HostAccess.NONE 启动。保持绑定 127.0.0.1、启用认证并最小化能力；不要向不受信任代码授予 native.java 或 native.paper。"
icon: shield-check
---

Native Mode must be enabled in both `config.yml` and `workspace.json`. Treat a native workspace exactly like a Java plugin and review all of its source before enabling it.
