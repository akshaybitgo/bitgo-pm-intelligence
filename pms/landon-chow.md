---
type: pm-brain
name: Landon Chow
slug: landon-chow
vertical: ecosystem
title: PM — Token Management (TKM)
last_updated: 2026-03-05
tags: [tkm, token-management, grantee, locked-tokens, treasury, go-accounts, trading-flywheel, payroll, heightzero, carf]
---

# Landon Chow — PM Brain

## Role & Scope

**Title**: PM — Token Management (TKM)
**Location**: New York
**Vertical**: Ecosystem
**Reports to**: Akshay Thakur

Landon owns BitGo's Token Management (TKM) platform — the institutional-grade infrastructure for managing token grants, vesting schedules, treasury distributions, and ecosystem banking. His mandate has two tracks: (1) operational excellence on the TKM platform (automation, self-serve, compliance) and (2) the ecosystem banking/liquidity layer — turning Go Accounts into the default banking hub for token grant recipients. He's targeting $1M in trade volume by end of March 2026 via the TKM→Go→Trade flywheel.

---

## Current OKRs (H1 2026)

| Objective | Key Result | Target | Status |
|-----------|-----------|--------|--------|
| Build TKM trade revenue | TKM-driven trade volume | $0 → $1M | 🟡 In Progress |

---

## Q1 Initiatives (In)

| Priority | Initiative | Status | Target |
|----------|-----------|--------|--------|
| P0 | KYC Bypass for fully regulated customers | ✅ Completed | 1/23/2026 |
| P0 | BGA commands — self-serve grantee onboarding | ✅ Completed | 1/31/2026 |
| P0 | Go TKM ↔ Trade pairs | ✅ Completed | 3/31/2026 |
| P0 | New grantee self-serve onboarding + accept grant flow | 🟡 On Track | 3/31/2026 |
| P0 | Lock discrepancy alerting | 🟡 On Track | 3/13/2026 |
| P0 | TKM telemetry for token flows | 🟡 On Track | 3/31/2026 |
| P0 | Admin view + tooling in TKM (onboarding, unlocking, comms) | 🟡 On Track | 3/31/2026 |
| P0 | Clawback + grant editing architecture | 🟡 On Track | 3/31/2026 |
| P0 | CARF-compliant tax withholding | 🟡 On Track | 3/31/2026 |
| P0 | Notifications + alerting for admins/support | 🟡 On Track | 3/31/2026 |
| P0 | HeightZero TKM 100% deprecation | 🟡 On Track | 3/31/2026 |
| P0 | Go Accounts as default token grant deposit location | 🟡 On Track | 3/31/2026 |
| P0 | Default liquidation to goUSD + rewards generation | 🔴 Blocked | 3/31/2026 |
| P0 | Locked token staking on Go | ⚪ Not Started | 3/31/2026 |
| P1 | Circuit breaker to freeze wallets | ⚪ Not Started | 3/13/2026 |
| P0 | Automated treasury management (auto-schedule + distribute) | ⚪ Not Started | 3/31/2026 |

## Q2 Initiatives (In/Planned)

| Priority | Initiative | Status | Target |
|----------|-----------|--------|--------|
| P0 | Token grant-backed borrowing MVP | ⚪ Not Started | Q2 TBD |
| P1 | Pre-TGE partnerships | ⚪ Not Started | Q2 TBD |
| P1 | Secondary/private markets for locked tokens | ⚪ Not Started | Q2 TBD |
| P2 | Early exercise + token buybacks | ⚪ Not Started | Q2 TBD |
| P2 | Payroll Step 1 — ERP integration for crypto payroll | ⚪ Not Started | Q2 TBD |
| P2 | Payroll Step 2 — withholding + remittance workflows | ⚪ Not Started | Q2 TBD |

---

## Focus Areas

| Theme | Description |
|-------|-------------|
| TKM Platform Operations | Self-serve onboarding, grant editing, clawback architecture, HeightZero migration, CARF compliance, admin tooling. Remove manual eng dependency for all grantee ops. |
| Trading Flywheel | Grant wallet → Go Accounts → trade/stake. Target $1M trade volume by end of March via grantee comms + whitelisting. Telemetry in place to track funnel. |
| Ecosystem Banking (Go Accounts) | Go as default grant deposit location; default liquidation to goUSD; locked token staking. Turns TKM into a financial operating layer for token ecosystems. |
| Locked Token Products (Q2) | Borrowing against locked tokens, secondary markets, early exercise. Long-term: TKM as a full token lifecycle financial services platform. |
| Payroll (Q2, Exploratory) | Crypto payroll with withholding + remittance; POC planned with BitGo itself first. |

---

## Key Blockers

- **Default liquidation to goUSD (P0, Blocked)**: Likely depends on Go Accounts infrastructure (Gobi) and/or liquidity partner readiness; needs resolution for March target.
- **Locked token staking (P0, Not Started)**: Complex — requires TKM + Go + staking platform integration; may slip Q1.

---

## Key Partners / Clients

| Partner | Context |
|---------|---------|
| Token Foundation Grantees | Core TKM clients; self-serve onboarding + distributions |
| HeightZero | Legacy platform being deprecated; 100% migration target by 3/31 |
| BitGo (internal) | Payroll POC target (step 1) |

---

## Key Dependencies

- **Gobi Nadesh** — Go Accounts platform; Go as default deposit location; locked token staking on Go; default liquidation to goUSD all depend on Gobi's infrastructure
- **Gaurav Pal** — Locked token staking is listed in Gaurav's area too; cross-PM coordination needed
- **Richard Xie** — Go Staking foundation supports locked token staking use case

---

## Context: TKM Strategy

TKM is positioned as the operating layer for token foundation treasury management. The H1 2026 flywheel thesis is: onboard grantee organizations onto TKM → route grant wallets through Go Accounts → unlock trade/stake revenue from idle tokens. The $1M trade volume target by end of March 2026 is the first proof point of this model.

The longer-term vision (Q2+) is to build ecosystem banking infrastructure — borrowing against locked tokens, secondary markets for pre-TGE allocations, and payroll — making BitGo the institutional financial operating system for token ecosystems.

---

## Open Items

- [ ] Unblock default liquidation to goUSD — identify dependency and resolution path
- [ ] Confirm locked token staking delivery timeline with Gobi/Richard/Gaurav
- [ ] Push grantee comms/whitelisting to drive $1M trade volume by March 31
- [ ] Define "on-chain OTC" for synchronized unlock days (exploratory, noted from roadmap context)
- [ ] Scope token grant-backed borrowing MVP for Q2 with eng

---

*Last updated: 2026-03-05 — built from Q1/Q2 roadmap CSV*
