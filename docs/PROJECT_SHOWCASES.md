# Project showcases

> Documentation-only case studies, based on public repository READMEs. No claims of production readiness or measured business impact are made without independent evidence.

## CCO PTM — Operational control

**[Public repository](https://github.com/Lockowom/CCO_PTM)**

**Problem domain:** coordination of warehouse, inventory, dispatch, quality and after-sales operations across different roles and devices.

**Solution described:** a modular React/Vite application using Supabase/PostgreSQL, role-based access, operational modules, mobile scanning and offline-capable workflows.

**Engineering considerations**
- Permission-aware interfaces and access control at the database layer.
- Traceable inventory and dispatch records.
- Mobile workflows, scanning and intermittent connectivity.
- Separation of modules and controlled deployments.

**Technologies documented:** React, Vite, TypeScript/JavaScript, Tailwind CSS, Supabase, PostgreSQL, Capacitor, Dexie, Vitest.

**Evidence:** [project README](https://github.com/Lockowom/CCO_PTM/blob/main/README.md). This page does not independently verify deployments or compliance certification.

## INVEN3 — Offline-first physical inventory

**[Public repository](https://github.com/Lockowom/inventario)**

**Problem domain:** physical warehouse counts with multiple devices, unreliable connectivity and strict reconciliation requirements.

**Solution described:** blind physical counting, local persistence, synchronization, snapshots, idempotent record handling and data export specifications.

**Engineering considerations**
- Separate physical counts from expected system stock.
- Identify inventory by product and, where relevant, lot/serial.
- Prevent duplicate writes and make retries safe.
- Preserve the audit trail across adjustments and reviews.

**Evidence:** [project README](https://github.com/Lockowom/inventario/blob/main/README.md). Its public phase label may lag behind current development; do not interpret it as a release certificate.

## Gym Stats Pro — Web application

**[Public repository](https://github.com/Lockowom/gym-stats-pro)**

**Confirmed public stack:** React, TypeScript and Vite. The current README is largely the Vite starter template, so features, users, deployment and outcome are **not yet independently documented**.

**Next documentation step:** replace the starter README with screenshots and a functional overview only after inspecting the actual source and confirming the intended showcase scope.

## Honest showcase criteria

Before calling any project shipped or production-ready, establish:
1. Verifiable release or deployment evidence.
2. A sanitized screenshot or demo using synthetic data.
3. Clear user workflows and technology architecture.
4. A reproducible build or test baseline.
5. Explicit limitations, license and privacy considerations.

See [architecture notes](ARCHITECTURE.md) for high-level system diagrams.
