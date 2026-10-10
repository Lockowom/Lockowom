# Real UI showcase — evidence audit

**Audit date:** 2026-10-10  
**Scope:** public default branches of [CCO_PTM](https://github.com/Lockowom/CCO_PTM) and [inventario (INVEN3)](https://github.com/Lockowom/inventario).

## Findings

A recursive GitHub repository-tree check found application launcher icons and PWA icon assets, but **no identifiable real UI screenshots** suitable for a product gallery in these public repository trees. Android launcher images are not evidence of the application's screen design.

| Project | Real UI screenshots approved for publication | Public conceptual illustration |
| --- | --- | --- |
| CCO PTM | None verified in inspected repository tree | [Visual card](../assets/cco-card.svg) |
| INVEN3 | None verified in inspected repository tree | [Visual card](../assets/inven3-card.svg) |

This is not proof that screenshots do not exist in other branches, releases, external deployments or private QA environments. No authenticated screens or customer data were accessed.

## Capture specification

1. Use a QA or local environment with synthetic or fully anonymized data.
2. Capture CCO overview, inventory and dispatch flows in desktop 16:9.
3. Capture INVEN3 login-independent counting screen, offline state and reconciliation on an Android test device (portrait 9:16).
4. Review images at 100% zoom for names, addresses, client identifiers, stock figures, serial/lot numbers, notifications, environment URLs, API tokens and QR/barcode payloads.
5. Publish only images explicitly approved for public use. Label screens by app, version and environment; do not infer production status.
6. Optimize images, strip metadata and use descriptive alternative text.
7. Replace the conceptual gallery cards only after real evidence exists; keep artwork labeled when retained.

## Release gate

- [ ] Real UI image exists
- [ ] Synthetic/anonymized records confirmed
- [ ] Security and privacy review complete
- [ ] Publication rights confirmed
- [ ] Version and test environment identified
- [ ] Accessibility text and link tested

**Until all checks pass, the profile must not display a mockup as an actual screenshot.**
