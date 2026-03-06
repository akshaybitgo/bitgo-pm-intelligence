---
type: vertical-index
slug: custody-platform
name: Custody & Platform
pm_owner: Ahmed Elmasry
status: active
last_updated: 2026-03-05
tags: [custody, wallets, hsm, mpc, tss, platform, api, dkls23, pqc, developer-experience, migration, agent-wallets]
---

# Custody & Platform

> **PM**: Ahmed Elmasry — see [ahmed-elmasry.md](../../pms/ahmed-elmasry.md) for full context.

## What This Vertical Owns

Custody & Platform is the foundational layer of BitGo. It encompasses the core wallet infrastructure, key management (HSM/MPC/TSS), institutional custody services, and the developer platform (APIs, SDKs, integrations). Every other vertical depends on Custody & Platform as its infrastructure backbone.

**Core products:**
- Self-managed wallets (hot, warm, cold)
- Qualified custody (institutional-grade)
- Multi-Party Computation (MPC) key management
- Hardware Security Modules (HSM)
- BitGo APIs and developer SDKs
- Policy engine and governance controls

## Q2 2026 OKRs (Summary)

| Objective | Status |
|-----------|--------|
| Obj 1: Default MPC migration destination — Fireblocks key-preserving flow + multi-provider playbook | ⚪ Planned |
| Obj 2: Developer control plane — Dashboard, MCP AI assistant, TTFC -20%, NPS +5 | ⚪ Planned |
| Obj 3: Signing stack hardened — DKLS-23 + EdDSA upgrade, FROST/Zcash, red team, PQC roadmap | 🟡 In Progress |
| Obj 4: Agentic wallet foundation — monitoring, guardrails, MCP wallet primitives | ⚪ Planned |

*→ Full OKR detail: [ahmed-elmasry.md](../../pms/ahmed-elmasry.md)*

## Active Initiatives

| Initiative | PM | Status | Target | Notes |
|-----------|-----|--------|--------|-------|
| GG18 → DKLS-23 MPC upgrade | Ahmed Elmasry | 🟡 In Progress | 6/30/2026 | Zero regression requirement; Silence Labs partnership |
| Legacy EdDSA → Threshold EdDSA/Schnorr | Ahmed Elmasry | 🟡 In Progress | 6/30/2026 | Coordinated with DKLS-23 migration |
| Post-quantum MPC roadmap | Ahmed Elmasry + CISO | ⚪ Planned | H1 2026 | R&D co-ownership needed; planning horizon item |
| Fireblocks → BitGo migration flow | Ahmed Elmasry | ⚪ Planned | Q2 2026 | Key-preserving; ≥1 live enterprise migration |
| Developer Dashboard (control plane) | Ahmed Elmasry | ⚪ Planned | Q2 2026 | API usage, webhooks, debugging, token management |
| MCP-backed AI assistant (dev XP) | Ahmed Elmasry | ⚪ Planned | Q2 2026 | Alignment with Akshay's generic framework pending |
| FROST / Zcash shielded signing | Ahmed Elmasry | ⚪ Planned | Q2 2026 | Ecosystem dep. (Zcash shielded tx) |
| AI-driven red team exercise | Ahmed Elmasry + CISO | ⚪ Planned | Q2 2026 | ≥5 ranked remediations; ≥3 resolved in H1 |
| Agent wallet monitoring + guardrails | Ahmed Elmasry | ⚪ Planned | 5/15 internal | Spend limits, circuit breakers, audit trail |
| Agent wallet MCP layer | Ahmed Elmasry | ⚪ Planned | 6/30/2026 | ≥3 internal teams/pilot partners using agent APIs |

## Key Contacts

| Role | Person |
|------|--------|
| PM Owner | Ahmed Elmasry |
| Engineering Lead | TBD |
| CISO | TBD |
| R&D Counterpart (PQC) | TBD |

## Cross-Vertical Dependencies

- **Ecosystem**: Chain and token onboarding runs on wallet infrastructure
- **Prime**: Prime brokerage uses custody wallet layer for settlement
- **CaaS**: Crypto-as-a-Service clients consume wallet APIs directly
- **SCaaS**: Stablecoin infrastructure uses custody rails for minting/burning

## Open Blockers

| Blocker | Owner | Since |
|---------|-------|-------|
| _(to be filled)_ | | |

## Key Dates

| Date | Event |
|------|-------|
| _(to be filled)_ | |

---

*Last updated: 2026-03-05 — populated with Ahmed Elmasry's Q2 OKR mandate.*
