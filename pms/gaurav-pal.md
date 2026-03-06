---
type: pm-brain
name: Gaurav Pal
slug: gaurav-pal
vertical: ecosystem
title: PM — Staking Utilization + Auto Staking
last_updated: 2026-03-05
tags: [staking, auto-staking, smart-staking, gas-tank, self-serve, solana, hypeevm, utilization, stuck-transactions]
---

# Gaurav Pal — PM Brain

## Role & Scope

**Title**: PM — Staking Utilization + Auto Staking
**Location**: Bangalore
**Vertical**: Ecosystem
**Reports to**: Akshay Thakur

Gaurav owns two related mandates: (1) driving staking utilization across BitGo's existing client base — getting eligible assets actively staked — and (2) building the Auto Staking product (opt-in, instant withdrawal, recommendation engine). He also owns gas tank infrastructure (EVM fee management) and self-serve chain onboarding tooling (Phase 3/4). He's the PM most directly responsible for converting idle custody assets into staking AUC.

---

## Current OKRs (H1 2026)

| Objective | Key Result | Target | Status |
|-----------|-----------|--------|--------|
| Staking utilization | Stake 30% of eligible assets in Q1/Q2 new client cohort | 30% utilization | 🟡 In Progress |

---

## Q1 Initiatives (In)

| Priority | Initiative | Status | Target |
|----------|-----------|--------|--------|
| P0 | KYC Bypass for fully regulated customers | ✅ Completed | 1/23/2026 |
| P0 | HYPEEVM staking support | ✅ Completed | 1/29/2026 |
| P0 | Staking discoverability — remove feature flags, provide access | 🔴 Blocked | 2/28/2026 |
| P0 | Smart Staking — recommendation engine for intelligent staking | 🟡 On Track | 3/31/2026 |
| P0 | HYPEEVM bridging support | 🟡 On Track | 3/31/2026 |
| P2 | Self-serve chain onboarding Phase 3 (API layer, auto-provision) | ✅ Completed | 3/31/2026 |
| P2 | Self-serve chain onboarding Phase 3 (testing) | 🟡 On Track | 3/31/2026 |
| P2 | Notifications/alerting for stuck transactions | 🟡 On Track | 3/31/2026 |
| P3 | Gas Tank — fee address creation (EVMs) | 🟡 On Track | 2/28/2026 |
| P3 | Gas Tank — fee auto funding (EVMs) | 🟡 On Track | 4/15/2026 |

## Q2 Initiatives (In/Planned)

| Priority | Initiative | Status | Target |
|----------|-----------|--------|--------|
| P1 | Solana: Close ATA address (API/UI) — retrieve SOL/token funds to root | ⚪ Not Started | TBD |
| P2 | Self-serve chain onboarding Phase 4 (workflow-based, no-code) | ⚪ Not Started | 6/30/2026 |
| P3 | Gas Tank — fee address creation (L1 chains) | ⚪ Not Started | 6/30/2026 |
| P3 | Gas Tank — fee auto funding (L1 chains) | 🟡 On Track | 4/15/2026 |

## Out of Scope / Backlog

| Priority | Initiative | Status | Notes |
|----------|-----------|--------|-------|
| P0 | Assets Identity & Symbol Management | ⚪ Not Started | Out of Q1/Q2 |
| P2 | Payments — global remittances (US→India stablecoin) | ⚪ Not Started | TBD — needs WC team input |
| P2 | Payments — WalletConnect Payments | ⚪ Not Started | TBD |
| P2 | Error message improvements | ⚪ Not Started | Q2 out |
| P4 | Help tooltips / onboarding walkthroughs | ⚪ Not Started | Backlog |
| P5 | Launch your own rollup blockchain (with BitGo) | ⚪ Not Started | Exploratory |

---

## Focus Areas

| Theme | Description |
|-------|-------------|
| Auto Staking | Opt-in auto staking with instant withdrawal; recommendation engine (Smart Staking); ~7 initial clients at beta; Binance staking (~$175M pipeline) |
| Staking Discoverability | Remove feature flags; surface staking options to clients who haven't opted in; critical to hitting 30% utilization OKR |
| Gas Tank (EVM) | Automated gas fee management for GoAccount-based wallets and enterprise clients; reduces friction in high-volume EVM operations |
| Self-Serve Chain Onboarding | Phase 3: reduce onboarding timeline from 4 weeks → 2 weeks via API automation. Phase 4: workflow-based, no-code. |
| Solana UX | Close ATA address + retrieve funds; reduces locked liquidity; client UX improvement |

---

## Key Blockers

- **Staking Discoverability (P0, Blocked)**: Feature flags still gating clients from discovering staking; slipped 2/28 target. Direct impact on 30% utilization OKR.

---

## Key Partners / Clients

| Partner/Client | Context |
|---------------|---------|
| Binance | ~$175M staking pipeline; part of Auto Staking beta |
| ~7 Initial Clients | Auto Staking beta cohort (Feb 15 beta, slipped) |

---

## Key Dependencies

- **Richard Xie** — Auto Stake V1 (staking infra) is a dependency for Gaurav's utilization goals
- **Gobi Nadesh** — Gas Tank fee address for Go Accounts; Go-based staking discovery surface
- **Anantha Padmanabhan** — Self-serve chain onboarding overlap; staking chain additions
- **Landon Chow** — locked token staking (P0 in Landon's list) connects to Go ecosystem banking

---

## Open Items

- [ ] Unblock staking discoverability — identify feature flag removal path and timeline
- [ ] Confirm Auto Staking beta client count and Binance pipeline status
- [ ] Coordinate Solana Close ATA scoping with eng for Q2
- [ ] Define Phase 4 self-serve onboarding requirements (workflow-based, no-code)
- [ ] Payments (remittance/WC) — assess priority vs. staking workload

---

*Last updated: 2026-03-05 — built from Q1/Q2 roadmap CSV*
