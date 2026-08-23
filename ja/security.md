---
title: "セキュリティと Native Mode"
description: "Safe Mode は HostAccess.NONE で開始します。127.0.0.1、認証、最小 capability を維持し、信頼できないコードへ native.java/native.paper を与えないでください。"
icon: shield-check
---

Native Mode must be enabled in both `config.yml` and `workspace.json`. Treat a native workspace exactly like a Java plugin and review all of its source before enabling it.
