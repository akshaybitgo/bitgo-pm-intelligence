---
type: pm-brain
name: "Gobi Nadesh"
vertical: "ecosystem"
role: "Product Manager"
team: Product
slack: "@gobinadesh496"
last_updated: 2026-03-03
---

# Gobi Nadesh — PM Brain File

## My Vertical & OKR

**Vertical**: Ecosystem (under Director Akshay Thakur)
**Area**: Go Accounts + Hub-and-Spoke
**Location**: Toronto
**H1 OKR**: Transform Go Accounts into an Active Hub — 20% Asset Utilization Rate, 25% Spoke Multiplier, 15% Time-to-First-Utilization within 7 days. On track to generate >$15M net revenue run rate by 6/30/2026.

## My Team

| Name | Location | Role | Focus Area |
|------|----------|------|------------|
| Steven Harris | — | E4 Engineer | Architecture, yield-bearing tokens |
| Akash Gianchandani | — | E4 Engineer | Canton (wrapping ~Mar 15), then available |
| Roland Borges | — | E4 Engineer | WD Incoming (wrapping soon), best fit for front-end UI |
| Sampras Saha | — | E3 Engineer | AMS Integration |
| Austen Cheethirala | — | E2 Engineer | AMS Integration |
| Girish Vegesna | — | E2 Engineer | Go Accounts platform |
| Ryan Deng | — | E2 Engineer | Token Management (ramping) |
| Tony Yu | — | Intern | Alerting (limited capacity) |

## Active Initiatives

| Initiative | Status | Key Date | Owner | Notes |
|------------|--------|----------|-------|-------|
| Tri-Party out of Go | Active — PRD done | Early Q2 ship | Gobi | Self-serve redesign, 1 engineer needed |
| Figure Markets (FIGR) | Phase 1 shipped (seg wallets) | Phase 2 TBD | Gobi | Phase 2 = Go integration, waiting on architecture from wallet team |
| Go Account UI/UX | Active — 8 todos | Q2 quick wins | Gobi | Timeline, deposits, fiat display, dashboard |
| App Store (Go Hub) | Design phase | Q2 v1 | Gobi | Three-world architecture, unified dashboard |
| Stablecoin Fungibility | POC in progress | End Q1 | Tres/Eugene | Go provides infra for cross-chain swaps |
| AI Insights Agent | Discovery | Q2 (2-3 wk experiment) | Gobi | Rule-based MVP experiment, scoped down from full build |
| Staking | Phase 1 partially shipped | Q2 | Richard Xie | Staking out of Go Accounts |
| Token Management | Awaiting resourcing | Q2 | Landon / Ryan Deng | Awaiting Go Team resourcing to review updated TDD |

## Key Partners / Deals

| Partner | Product | Status | Priority | Notes |
|---------|---------|--------|----------|-------|
| Figure Markets / Futu-Moomoo | FIGR integration (tokenized securities) | Phase 1 shipped (seg wallets) | High | Phase 2 = Go integration, waiting on wallet team architecture |

## Open Items / Blockers

- [ ] Triparty: secure 1 engineer for Phase 1
- [ ] FIGR Phase 2: waiting on wallet team architecture for Go integration
- [ ] App Store v1 scope: "referral marketplace" not yet defined — what's the MVP?
- [ ] Token Management: awaiting Go Team resourcing to review updated TDD
- [ ] Staking Phase 1: which assets are live? Current adoption rate?

## Recent Decisions

<!-- Auto-updated by pm-debrief connector. Do not edit manually. -->
| Date | Decision | Context |
|------|----------|---------|
| | | |

## Cross-functional Dependencies

| Team | Dependency | Status |
|------|-----------|--------|
| Engineering | Mike Comstock makes final engineer allocation decisions | Ongoing |
| Engineering | Steven Harris — architecture decisions across all Go initiatives | Available |
| Engineering | Wallet team — FIGR Phase 2 Go integration architecture | Waiting |
| Trust Ops | — | — |

## Context Dump

### Strategic Framing
Go Accounts is BitGo's "hub-and-spoke" platform: a single account that connects to Staking, Financing, Trading, and Token Management services. H1 2026 focus is driving utilization — getting deposited assets actively used in at least 2+ spokes. The north star is Asset Utilization Rate (AUR) reaching 20%.

### Key Product Areas
- **Go Accounts Platform**: Core accounting/custody — Lightning deposits, AMS cutover, event-driven processing, Canton integration
- **Tri-Party**: Self-serve triparty product built on Go (biggest Q2 initiative)
- **Go Hub / App Store**: Unified dashboard with referral marketplace for spoke discovery
- **AI Insights Agent**: Rule-based capital efficiency nudges (e.g., "you have idle BTC — consider staking")
- **Yield-Bearing Tokens**: YLDS and Provenance token support natively in Go

### How We Make Money
- Fees on spoke utilization (staking commissions, financing interest, trading fees)
- NRE for large integrations
- Goal: >$15M net revenue run rate by 6/30/2026

### Biggest Risks / Watchouts
- Eng resourcing: several initiatives not yet staffed (Insight Agent, App Store)
- FIGR Phase 2 depends on wallet team architecture
- TKM → Go awaiting Go Team resourcing to review updated TDD
- AMS cutover timeline determines when Sam + Austen become available

### Who to Know
- **Akshay Thakur** — Director, Ecosystem (my manager)
- **Steven Harris** — E4, Go Accounts architect
- **Mike Comstock** — Makes final eng allocation decisions
- **Landon Chow** — PM, Token Management / Go Hub
- **Nuri** — CPO
- **Chen** — CRO

---

*Last updated: 2026-03-03*
*To update: run `pm-update-brain` or edit this file directly and commit*
