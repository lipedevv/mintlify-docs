---
name: nexora-transactional-gui
description: Build and review Nexora GUI shops and other inventory interfaces where money, item delivery, persistence, duplicate-click protection, and refunds must remain consistent.
license: Proprietary documentation
metadata:
  author: lipedevv
  version: "1.0.0"
---

# Nexora transactional GUI development

Use the documented GUI, inventory, economy, and database APIs. Do not substitute Bukkit internals or invented convenience methods.

For every purchase flow:

1. Resolve the product from trusted server-side configuration; never trust GUI text or client-provided price data.
2. Reject invalid amount, offline player, missing permission, insufficient balance, full inventory, and duplicate/in-flight clicks.
3. Use a conditional debit or database transaction so concurrent clicks cannot overspend.
4. Deliver the exact item only after the debit succeeds.
5. If delivery fails after debit, perform an idempotent compensation/refund and record the failure.
6. Persist a unique transaction identifier and enough audit data to investigate retries without duplicating rewards.
7. Refresh or close the GUI safely after completion and clear per-player locks during disconnect, shutdown, and reload.

Test success, insufficient funds, full inventory, rapid double-click, two simultaneous purchases, disconnect during purchase, reload during an operation, database failure, delivery failure, and retry after compensation.
