# Engineering portfolio | Architecture notes

This page documents **high-level, publicly described architecture**. It does not claim any live deployment or production certification.

## CCO — Operational control platform

**Source:** [CCO_PTM public README](https://github.com/Lockowom/CCO_PTM)

```text
Web UI (React + Vite)
    |
    +-- State & queries (Zustand / React Query)
    |
    +-- Operational modules
    |      Inbound | Inventory | Outbound | TMS | Quality | After-sales
    |
    +-- Supabase services
    |      PostgreSQL | Auth & RLS | Realtime | Edge Functions
    |
    +-- Supporting integrations
           Express proxy | Routes/Maps | Android via Capacitor
```

**Design topics:** modular operational workflows, permission boundaries, stock traceability, role-driven interfaces, mobile scanning, offline queues and logistics process automation. These are architectural themes described in the repository, not a guarantee of operational readiness.

## INVEN3 — Physical inventory capture

**Sources:** [inventario](https://github.com/Lockowom/inventario) and [Inventario-](https://github.com/Lockowom/Inventario-). Both public READMEs currently describe the same INVEN3 concept; they should **not** be presented as two independent finished products.

```text
Inventory capture devices
    |
    +-- Offline-first mobile workflow
    |      Local storage / queued operations
    |
    +-- Data synchronization and reconciliation
    |
    +-- Supabase / PostgreSQL
           Auth | Protected data | Inventory records
```

**Design topics:** blind physical counting, offline synchronization, identity by SKU/lot/serial, audit trails, idempotency, validated exports and controlled reconciliation. The public READMEs contain older phase-status text; check the project and its release evidence for current state.

## Portfolio quality gates

- Link only to repositories that are actually public.
- Do not display screenshots unless permissions and redaction are confirmed.
- Never publish customer names, internal operational figures, credentials, tokens, endpoints with secrets or private employee data.
- Distinguish implemented features, designs, prototypes and verified deployments.
- Keep projects' development pipelines separate from the portfolio profile.

## Next showcase assets

Approved and redacted application screenshots, a short UI walkthrough, an architecture decision record, and validated non-sensitive performance metrics will improve this portfolio substantially.
