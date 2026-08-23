---
title: "Konfigurácia enginu"
description: "Nexora 1.0.0 enforces startup and callback timeouts, pending task limits, concurrent network limits, log rate limits and rate-limited slow-callback diagnostics."
icon: settings
---

| Key | Default |
| --- | --- |
| engine.workspaces-directory | workspaces |
| engine.revisions-to-keep | 10 |
| engine.auto-reload | true |
| engine.auto-reload-debounce-ms | 600 |
| server.enabled / host / port | true / 127.0.0.1 / 8123 |
| security.native-mode | false |
| security.require-authentication | true |
| security.token | empty; initial random token is generated |
| security.rate-limit-per-minute | 240 |
| limits.maximum-startup-ms | 10000 |
| limits.maximum-execution-ms | 250 |
| limits.maximum-pending-tasks | 1000 per workspace |
| limits.maximum-network-requests | 20 concurrent per workspace |
| limits.maximum-log-rate | 100 messages/second per workspace |
| profiler.enabled | true |
| profiler.slow-execution-ms | 10 |
| metrics.interval-ms | 1000 |
