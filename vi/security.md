---
title: "Bảo mật và Native Mode"
description: "Safe Mode bắt đầu với HostAccess.NONE. Giữ 127.0.0.1, bật xác thực, dùng capability tối thiểu; không cấp native.java/native.paper cho mã không tin cậy."
icon: shield-check
---

Native Mode must be enabled in both `config.yml` and `workspace.json`. Treat a native workspace exactly like a Java plugin and review all of its source before enabling it.
