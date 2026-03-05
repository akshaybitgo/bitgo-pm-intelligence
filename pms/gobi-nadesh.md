---
type: pm-brain
name: Gobi Nadesh
vertical: ecosystem
team: integrated-account-hub
location: Toronto
last_updated: 2026-03-05
---

# Gobi Nadesh — PM Brain File

## Role & Scope

PM for the Integrated Account Hub sub-vertical within Ecosystem. Owns Go Accounts product — specifically front-end changes within app.go (not entire platform navigation). Reports to Akshay Thakur.

---

## Q2/Q3 Charter — 4 Core Initiatives

### 1. Go Accounts UX — Hub-and-Spoke Model
**Objective**: Execute the Go Account hub-and-spoke model within app.go UX.
**Approach**: Weekly experiments and prototypes (using Vercel for fast validation), challenge Kinugi's current UI assumptions.
**KPI**: Define 90% end state of the UI; create Q2/Q3/Q4 roadmap for subtle migration to final state.
**Scope constraint**: Limited to Go accounts changes — not entire platform navigation.

### 2. Insights Hub / Allocation Engine
**Objective**: Build a 1-inch abstraction model that suggests investment options across different yield-bearing strategies based on a client's risk profile.
**Target audience**: Smaller firms, family offices, companies new to crypto (and large asset managers interested in DeFi insights).
**Four strategies**: Staking, DeFi, lend/borrow, Binance integration.
**KR**: Build allocation engine abstracting 4 strategies → recommends weighted portfolio + return rate based on risk profile.
**Two UX experiences**: (1) "Soup" — show all strategies; (2) User-guided risk appetite process drawing on DeFi deployment signals.
**Q2 dependencies**: Natively yield-bearing assets, rebase tokens, money market funds (MMFs) in Go accounts.
**Test approach**: LaunchDarkly quick testing to validate if insights drive down time-to-utilization.
**Note**: Stable coin fungibility removed from Q2 scope.

### 3. Marketplace
**Objective**: Third-party vendor upsell platform.
**Status**: Confirmed as third main remit alongside Insights/Allocation Engine.

### 4. Scenario Analyzer / Risk Profile *(Phase 2)*
**Objective**: Marry the allocation engine with risk profile + macroeconomic assumptions. Users tweak assumptions and receive adjusted recommendations.
**Status**: Phase 2 of Insights work — not Q2 scope. Planning horizon Q3/Q4.

---

## Binance Integration (New Q2 Item)
**Description**: Integrating Binance products via a complex jurisdictional money movement model using BitGo Dubai to serve US customers.
**Requirements**: Legal and compliance validation required. Dedicated full-time PM from India (Anant) + resources from Landon's team proposed.
**Owner**: Gobi + India PM (Anant, TBD to be formalized)
**Status**: Newly added; resource allocation pending.

---

## AI / MCP Initiatives (Cross-functional with Akshay)

### Two-Stream Development Strategy
**Stream 1 — Gobi**: Quick iteration, constrained releases (not GA), hypothesis testing, feedback gathering on initial AI concepts.
**Stream 2 — Akshay**: Generic agentic framework incorporating Gobi's feedback; psychological applicability of AI over specific features.

**Key principle**: Build generic framework so any new use case takes <30 min to spin up. Focus on institutional clients, not consumer agentic wallets.
**Self-reflection requirement**: Framework must incorporate feedback loops so agents iteratively improve themselves (V2 creation through self-reflection).

### Coordination
Gobi to lead quick iteration; Akshay + Gobi + Ahmed to align on reconciling developer experience (Ahmed's scope) with the general AI approach.

---

## Team & Dependencies

| Person | Role | Dependency |
|--------|------|-----------|
| Richard Xie | PM, Staking | Staking expansion out of Go — Richard is owner |
| Landon Chow | PM, Token Management | Potential resource for Gobi; coordinate on Binance overlap |
| Ahmed Elmasry | PM, Dev Experience / MCP | MCP server alignment; developer experience scope |
| Anant | PM (India) | Proposed for Binance project full-time |
| Nuri | CPO | Tasked Gobi with Insights Hub for Q2 |
| Mike | CEO | Gobi formalizing gas funding bot project with Mike |

---

## Q2 Roadmap Items
- Expansion of staking out of Go (Richard owns)
- Token management integration
- Rebase token support
- Automating third-party integrations (Phase 1: remove manual Prime Operations work)
- Insights Hub / Allocation Engine
- Marketplace (third-party vendor upsell)
- Binance integration (new)
- ~~Stable coin fungibility~~ *(deleted)*

---

## Open Items / Decisions Needed

| Item | Owner | Status |
|------|-------|--------|
| Singapore AI R&D event (late March / early April) | Akshay | Pending budget confirmation by 2026-03-09 |
| Landon + Gobi + Akshay: finalize 1-inch abstraction model objective | Akshay | Scheduled for 2026-03-06 |
| Binance document review | Gobi | Waiting for Akshay to share doc |
| Anant assignment to Gobi for Binance | Akshay | Pending formalization |
| Ahmed alignment call (dev XP vs general AI approach) | Akshay + Gobi | To be scheduled |
| Hub-and-spoke roadmap formalization (Q2/Q3/Q4) | Gobi | Pending |

---

*Last updated: 2026-03-05 | Source: Gobi/Akshay 1:1 meeting notes*
