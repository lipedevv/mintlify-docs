---
title: "Säkerhet och Native Mode"
description: "Safe Mode startar med HostAccess.NONE. Behåll 127.0.0.1 och autentisering, minimera capabilities och ge aldrig native.java/native.paper till opålitlig kod."
icon: shield-check
---

Native Mode must be enabled in both `config.yml` and `workspace.json`. Treat a native workspace exactly like a Java plugin and review all of its source before enabling it.
