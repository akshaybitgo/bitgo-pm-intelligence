---
type: pm-brain
name: Ahmed Elmasry
slug: ahmed-elmasry
vertical: custody-platform
title: PM — HSM & MPC + Developer Experience
last_updated: 2026-03-05
tags: [custody, hsm, mpc, tss, dkls23, developer-experience, api, pqc, migration, agent-wallets, fireblocks, red-team]
---

# Ahmed Elmasry — PM Brain

## Role & Scope

**Title**: PM — HSM & MPC + Developer Experience
**Vertical**: Custody Platform
**Location**: San Francisco
**Reports to**: CPO / Custody Platform leadership

Ahmed owns two distinct but deeply connected areas: BitGo's cryptographic signing stack (HSM, MPC/TSS protocols, key management security) and the developer platform (APIs, SDKs, integration experience, developer tooling). He is also the primary PM interface for the Offensive Security initiative (post-quantum MPC roadmap, red team exercise) and the emerging agentic wallet foundation.

---

## Q2 2026 OKR Mandate

### Objective 1: Make BitGo the default migration destination for institutional MPC clients

*Framing: Not just "easiest" (feature claim) — "default" (market position). Revenue-relevant via pipeline signal.*

| Key Result | Target | Status |
|-----------|--------|--------|
| Ship Fireblocks → BitGo public key-preserving migration flow; ≥1 live enterprise migration with zero key material re-generation | 1 live migration | ⚪ Planned |
| Deliver reusable migration playbook covering ≥2 MPC providers (Fireblocks + 1 other), validated by R&D — reduces scoping time from weeks to days | 2 providers covered | ⚪ Planned |
| *(Stretch)* Build migration pipeline: ≥3 qualified enterprise conversations in active migration discovery by 6/30, tracked in CRM with Chen's team | 3 qualified conversations | ⚪ Stretch |

---

### Objective 2: Establish BitGo's developer control plane as the default integration layer

*Strongest objective. Tightened AI KR, added time-to-integration as north star metric.*

| Key Result | Target | Status |
|-----------|--------|--------|
| Launch Developer Dashboard as primary control plane for API usage, token management, webhooks, and debugging; 70%+ active adoption among API customers by 6/30 | 70% adoption | ⚪ Planned |
| Embed MCP-backed AI assistant (error explanations, usage anomaly detection, guided debugging); reduce developer-related support ticket volume by 30% — baseline locked with SE and CSM by end of March | -30% support tickets | ⚪ Planned |
| Reduce median time-to-first-successful-API-call for net new integrators by 20% (baseline from current onboarding funnel data) | -20% TTFC | ⚪ Planned |
| Improve integrator NPS by 5+ points — launch baseline survey by March 31, confirm target by April 15 | +5 NPS pts | ⚪ Planned |

---

### Objective 3: Harden and future-proof BitGo's signing stack

*Renamed from "leader in PQC & privacy." Organized as coherent arc: modernize → extend → stress-test → chart quantum path.*

| Key Result | Target | Status |
|-----------|--------|--------|
| Complete signing stack modernization: legacy EdDSA → threshold EdDSA/Schnorr, GG18 → DKLS-23; zero regression on existing signing coverage; shipped to production by 6/30 | Production by 6/30 | 🟡 In Progress |
| Launch FROST-based signing for Zcash shielded transactions; ≥1 enterprise client live with shielded transaction capability | 1 enterprise client live | ⚪ Planned |
| Execute AI-driven red team exercise on wallet signing stack; deliver internal findings report with ≥5 ranked actionable remediation items; ≥3 remediation items resolved or scheduled within H1 | Report + 3 remediations | ⚪ Planned |
| Publish BitGo PQC readiness roadmap: threat model, 3-year migration path, ≥1 pilot implementation scoped — co-owned with CISO and R&D counterpart | Published roadmap | ⚪ Planned |

---

### Objective 4: Deliver an institutional-grade agentic wallet foundation

*Added adoption signal and stretch for ecosystem positioning. MCP layer KR aligns with broader Agent Wallets initiative.*

| Key Result | Target | Status |
|-----------|--------|--------|
| Launch agent visibility and monitoring dashboard: activity logs, spend, policy events, circuit breaker triggers, full audit trail — live for internal testing by 5/15 | Live by 5/15 | ⚪ Planned |
| Implement agent policy guardrails (spend limits, circuit breakers, expiry, approval gates) with 100% coverage of agent-initiated signing paths before any external launch | 100% coverage | ⚪ Planned |
| Expose wallet primitives via internal MCP layer; ≥3 internal teams or pilot partners actively using agent APIs by 6/30 | 3 internal users | ⚪ Planned |
| *(Stretch)* Co-define agentic wallet interface standards with ≥1 ecosystem partner — positions BitGo to influence emerging institutional agent wallet spec | 1 ecosystem partner | ⚪ Stretch |

---

## Active Initiatives

| Initiative | Status | ETA | Key Dependency |
|-----------|--------|-----|----------------|
| GG18 → DKLS-23 signing upgrade | 🟡 In Progress | 6/30/2026 | Zero regression requirement; staged rollout |
| Legacy EdDSA → Threshold EdDSA/Schnorr | 🟡 In Progress | 6/30/2026 | Coordinated with DKLS-23 migration |
| Developer Dashboard (control plane) | ⚪ Planned | Q2 2026 | API usage telemetry pipeline; SE/CSM baseline data |
| MCP-backed AI assistant (developer XP) | ⚪ Planned | Q2 2026 | MCP server architecture — alignment with Akshay's generic framework |
| Fireblocks → BitGo migration flow | ⚪ Planned | Q2 2026 | R&D validation; key-preserving protocol design |
| Migration playbook (multi-provider) | ⚪ Planned | Q2 2026 | Fireblocks flow complete first; Chen's team CRM tracking |
| FROST / Zcash shielded signing | ⚪ Planned | Q2 2026 | Zcash shielded tx completion (ecosystem dep.) |
| AI-driven red team exercise | ⚪ Planned | Q2 2026 | CISO co-ownership; R&D lead identification |
| PQC readiness roadmap | ⚪ Planned | H1 2026 | CISO + R&D co-ownership; not a live threat yet — planning problem |
| Agent wallet foundation (monitoring + guardrails) | ⚪ Planned | 5/15 internal | Cross-functional with Ecosystem Agent Wallets initiative |
| Agent wallet MCP layer exposure | ⚪ Planned | 6/30/2026 | Internal pilot partners; Akshay AI framework alignment |

---

## Cross-Functional Dependencies

| Dependency | Direction | Who | What |
|-----------|-----------|-----|------|
| Ecosystem | Custody ← | Akshay Thakur | Generic agentic framework must reconcile with Ahmed's MCP server scope |
| Ecosystem | Custody ← | Gobi Nadesh | Developer XP alignment; AI two-stream reconciliation call pending |
| CISO | Custody → | TBD | PQC roadmap co-ownership; red team exercise joint execution |
| R&D | Custody → | TBD | DKLS-23, FROST, PQC — cryptography R&D partnership |
| Sales/CRO | Custody → | Chen's team | Migration pipeline — CRM tracking for ≥3 qualified migration prospects |
| SE / CSM | Custody → | TBD | Developer NPS baseline; support ticket volume baseline |
| Legal / OC | Custody → | TBD | Privacy coin / shielded transaction policy review |

---

## Open Items

- [ ] Lock developer support ticket baseline with SE and CSM teams (by end of March — needed for Obj 2 KR2)
- [ ] Launch integrator NPS baseline survey by March 31
- [ ] Identify ≥1 enterprise prospect for Fireblocks migration pilot
- [ ] Define second MPC provider for migration playbook (beyond Fireblocks)
- [ ] Confirm CISO co-owner for PQC roadmap and red team exercise
- [ ] Identify R&D counterpart for PQC roadmap and signing stack modernization
- [ ] Schedule alignment call with Akshay + Gobi to reconcile developer XP / MCP scope with generic AI framework
- [ ] Get internal pilot partners committed for agent wallet MCP layer (target: ≥3 by 6/30)
- [ ] Define agent wallet interface standard draft for ecosystem partner outreach (stretch)

---

## Recent Decisions

| Date | Decision | Rationale |
|------|----------|-----------|
| 2026-03-05 | AI OKR scoped to developer control plane, not generic agent strategy | Akshay owns the generic agentic framework; Ahmed's AI scope is developer experience (MCP-backed assistant, anomaly detection, guided debugging) |
| 2026-03-05 | MCP scope flagged as too narrow — needs year-out vision | Akshay's view: developer XP MCP server must account for all personas (CSMs, sales, developers); alignment call with Gobi + Ahmed pending |
| 2026-03-02 | PQC roadmap: planning problem, not live threat | CEO briefing confirmed PQC is strategic horizon item; co-own with CISO + R&D, not Ahmed solo |
| 2026-03-02 | Offensive security: red team over compliance audit | CISO + R&D joint ownership model — sequential "build then review" model too slow |

---

## Context Dump

### DKLS-23 and Signing Stack Modernization
BitGo is upgrading its MPC/TSS protocol stack: GG18 → DKLS-23 (next-gen threshold signature scheme, lower communication overhead, stronger security proofs) and legacy EdDSA → threshold EdDSA/Schnorr. Both need zero regression on existing signing coverage — any client on existing protocols must continue to work without re-keying. Silence Labs is the primary MPC engineering partner in this stack.

### Fireblocks Migration Strategy
BitGo's competitive positioning: Fireblocks clients considering migration have historically faced the hard problem of key material re-generation (clients don't want to re-issue keys to hundreds of counterparties). Ahmed owns the solution: a public key-preserving migration flow that lets enterprise clients move their MPC key shares to BitGo without generating new keys. This is a significant moat if executed well and validated by R&D. First live migration is the proof point; a reusable multi-provider playbook turns it into a repeatable revenue motion.

### Developer Experience — Control Plane
Developer Dashboard is the north star product: a unified control plane where API customers can inspect usage, manage tokens, configure webhooks, review policy events, and debug issues — without needing to file support tickets or loop in BitGo SEs. MCP-backed AI assistant sits on top: contextual error explanations, anomaly detection on API usage patterns, guided debugging flows. The key metric linkage: time-to-first-successful-API-call and integrator NPS. Both need baselines locked by end of March.

### MCP Server — Scope Alignment Needed
Ahmed is building an MCP server for developer experience. Akshay's view (from Mar 5 Gobi 1:1): the scope is currently too narrow. The MCP layer should be designed with a year-out vision for every persona who will use it — CSMs, sales reps, developers, and internal PMs all have distinct tool needs. Ahmed's developer XP MCP needs to reconcile with Akshay's generic agentic framework to avoid duplicated infrastructure. Alignment call with Akshay + Gobi pending.

### PQC and Post-Quantum Roadmap
Not an imminent threat — planning horizon problem. BitGo needs a 3-year migration path with threat model and pilot scope. Co-owned by Ahmed (HSM/MPC), CISO, and an R&D counterpart. CEO briefed and endorsed this as a strategic priority (Mar 2). Red team exercise (AI-driven, on wallet signing stack) is the near-term executable deliverable; PQC roadmap published by H1 end.

### Agentic Wallet Foundation
Ahmed is the custody-layer owner for the Agent Wallets initiative. His deliverables: monitoring/visibility dashboard (audit trail, spend tracking, circuit breaker logs) and policy guardrail enforcement (spend limits, approval gates, expiry) on all agent-initiated signing paths — these must be in place before any external launch. The MCP layer exposure (wallet primitives accessible to internal teams and pilot partners) is the connection point to Akshay's generic agentic framework. Stretch: co-define interface standards with ≥1 ecosystem partner.

---

*Last updated: 2026-03-05*
