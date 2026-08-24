---
name: nexora-debugging
description: Diagnose Nexora workspace startup, reload, command, event, GUI, promise, database, and compatibility failures using logs and the documented runtime lifecycle.
license: Proprietary documentation
metadata:
  author: lipedevv
  version: "1.0.0"
---

# Nexora runtime debugging

Start from the first Nexora exception or rejected callback, not downstream symptoms.

- Capture the complete log from workspace validation/startup through the failing action, including workspace id, callback kind, revision, and Java/Paper versions.
- Separate expected profiler warnings from failures. A slow-callback warning does not mean the workspace stopped.
- Verify the server uses Java 21 for Paper 1.20.6–1.21.11 or Java 25 for Paper 26.x.
- Confirm the workspace path, manifest id, JavaScript entry file, capabilities, and every imported relative file.
- Reproduce once after a clean automatic reload and once after a clean server restart when lifecycle state is relevant.
- For asynchronous errors, trace the originating promise/database/HTTP call and confirm the workspace was still running when completion resumed.
- For GUI and command issues, verify registration succeeded before debugging callback code.
- Do not recommend disabling runtime safety checks or switching to Native Mode unless the documented root cause requires it.

Return the root cause, evidence, affected files, minimal correction, regression test, and any remaining uncertainty.
