---
title: "Sicherheit und Native Mode"
description: "Safe Mode startet mit HostAccess.NONE. 127.0.0.1 und Authentifizierung beibehalten, Capabilities minimieren und native.java/native.paper nie fremdem Code geben."
icon: shield-check
---

Native Mode must be enabled in both `config.yml` and `workspace.json`. Treat a native workspace exactly like a Java plugin and review all of its source before enabling it.
