---
title: "API HTTP administrativa"
description: "Use Authorization: Bearer <token>. Keep the service bound to 127.0.0.1 unless TLS, firewall rules and a secured reverse proxy are configured."
icon: globe
---

| Method | Path | Scope |
| --- | --- | --- |
| GET | /health | none |
| GET | /api/v1/server | read |
| GET | /api/v1/workspaces | read |
| POST | /api/v1/workspaces/{id}/restart | deploy |
| POST | /api/v1/workspaces/{id}/enable | deploy |
| POST | /api/v1/workspaces/{id}/disable | deploy |
| POST | /api/v1/workspaces/{id}/rollback/{revision} | deploy |
| GET | /api/v1/gui-snapshots | read |
| GET | /api/v1/profiler | read |
| POST | /api/v1/tokens | admin |
| DELETE | /api/v1/tokens/{id} | admin |
| WS | /api/v1/live | read |
