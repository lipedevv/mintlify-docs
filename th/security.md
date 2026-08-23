---
title: "ความปลอดภัยและ Native Mode"
description: "Safe Mode เริ่มด้วย HostAccess.NONE คงการ bind ที่ 127.0.0.1 เปิด authentication และใช้ capability ต่ำสุด ห้ามให้ native.java/native.paper แก่โค้ดที่ไม่เชื่อถือ"
icon: shield-check
---

Native Mode must be enabled in both `config.yml` and `workspace.json`. Treat a native workspace exactly like a Java plugin and review all of its source before enabling it.
