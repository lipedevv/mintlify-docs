---
title: "Sorun giderme ve üretim kontrol listesi"
description: "Değişiklik reddedilirse ilk workspace uyarısını düzeltin, sürümleri silmeyin. Port doluysa eski süreci durdurun, aynı dünya için iki Paper açmayın ve Windows’ta nogui kullanın."
icon: wrench
---

## Production checklist

Üretimden önce workspaces/storage yedeği alın; başlatma/durdurma, izinler, dolu envanter ve yetersiz bakiye testlerini yapın; tokenı koruyun ve ilan edilen Paper buildini test edin.

- Never launch two Paper processes against the same world directory.
- Use `java -jar server.jar nogui` on Windows.
- Back up workspaces, storage and databases before upgrading.
- Test insufficient funds, full inventories, disconnects and restarts.
