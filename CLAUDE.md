# BitGo PM Intelligence — Orchestration Instructions

This is a shared knowledge base for BitGo Product Managers. Claude reads this file to understand how to orchestrate queries, onboard new team members, and update knowledge across all verticals.

---

## Step 0 — PM Identity Check (ALWAYS RUN FIRST)

Before loading any knowledge, read `config.yaml` and check `user.name`.

**If `user.name` is empty or missing → First-Time Setup:**
1. Say: "Welcome to BitGo PM Intelligence. Let's get you set up — this takes 2 minutes."
2. Ask: "What's your full name and BitGo email?"
3. Ask: "Which vertical are you joining? (ecosystem / custody-platform / prime / caas / scaas)"
4. Write their answers into `config.yaml` under the `user:` block (name, email, vertical, brain_file: `pms/{firstname}-{lastname}.md`)
5. Check if their brain file exists at `pms/{firstname}-{lastname}.md`:
   - **If it doesn't exist**: Copy `framework/templates/brain.md` to `pms/{firstname}-{lastname}.md` and say "I've created your brain file. Let's fill in the basics — tell me about your vertical and current priorities."
   - **If it exists**: Load it and continue to session start
6. Add them to `pms/_index.md` if not already listed
7. Tell them: "You're set up. Run `pm-onboard` anytime for a full vertical walkthrough."

**If `user.name` is filled → Returning PM:**
- Silently note who they are (e.g. `name: Akshay Thakur`, `vertical: ecosystem`)
- Load their brain file (`pms/{brain_file}`) as part of the auto-load below
- Continue to session start

> **Jarvis vs PM Intelligence**: Private context (todos, personal notes, partner specifics, sensitive discussions) lives in your personal Jarvis workspace (`~/{your-folder}/.jarvis/`). This repo is for *shared team knowledge* — OKRs, vertical status, cross-PM context. If you need to look up something personal mid-session, say "switch to Jarvis context."

---

## Auto-Load on Session Start

At the start of every session, load in this order:

1. `knowledge/shared/snapshot.md` — company-wide hot items
2. `knowledge/shared/okrs.md` — all vertical OKR table
3. `knowledge/shared/org-chart.md` — who owns what
4. `pms/_index.md` — list of all PM brain files
5. `pms/{current-pm-brain-file}` — the current PM's personal context (from config.yaml)

Then greet the user with:
- Today's date
- Any slipped OKR deadlines or stale targets (compare target dates to today)
- A one-line status per vertical from snapshot.md
- One-line summary of the current PM's top open items (from their brain file)
- Ask: "What would you like to work on today?"

---

## Query Routing Logic

Use this table to decide which files to load for a given query:

| Query Type | Files to Load |
|------------|---------------|
| Vertical status ("is ecosystem on track?") | `knowledge/verticals/{vertical}/_index.md` + `roadmap.md` + `deals.md` |
| OKR / revenue question | `knowledge/shared/okrs.md` + relevant vertical `roadmap.md` |
| Partner / deal question | `knowledge/verticals/{vertical}/deals.md` + `partners/{slug}.md` |
| Technical / architecture question | `knowledge/shared/product-stack.md` + `knowledge/verticals/{vertical}/technical.md` |
| People / team question | `knowledge/shared/org-chart.md` + `knowledge/verticals/{vertical}/team.md` + `pms/{name}.md` |
| Cross-vertical question | Load `_index.md` from all relevant verticals |
| Onboarding question | `knowledge/shared/product-stack.md` + `knowledge/shared/glossary.md` + relevant vertical |
| "What is [term]?" | `knowledge/shared/glossary.md` → if not found, load `product-stack.md` |
| Meeting prep | Relevant partner record + team + recent meeting notes |

For broad queries ("what's happening this week"), load:
- `knowledge/shared/snapshot.md`
- All vertical `_index.md` files
- `knowledge/shared/okrs.md`

---

## Onboarding Mode

When a new joinee asks to get up to speed, run `pm-onboard` skill:

1. Ask which vertical they're joining
2. Load `knowledge/shared/product-stack.md` first (full BitGo product map)
3. Load `knowledge/shared/glossary.md`
4. Load their vertical's `_index.md` + `technical.md` + `team.md`
5. Walk through `framework/templates/onboarding-checklist.md`
6. Offer to drill into specific areas

---

## Knowledge Update Protocol

When a PM shares new information (meeting transcript, decision, update):

1. Parse for: decisions, action items, status changes, new entities
2. **Low-risk updates** (dates, attendees, minor status): apply automatically
3. **High-risk updates** (OKR changes, new partners, deadline shifts): show diff and ask for confirmation before writing
4. Update the relevant PM brain file + vertical domain file
5. Update `knowledge/shared/snapshot.md` if company-wide significance
6. Always prompt: "Want me to commit and push these changes so the team sees them?"
7. If yes — stage, commit with message `"[date] [PM name]: [brief description of changes]"`, then push to `origin main`

---

## Cross-Vertical Synthesis

For questions that span verticals (e.g., "which verticals are blocked on legal/OC?"):

1. Load all vertical `_index.md` files in parallel
2. Scan for the relevant dimension (blockers, legal flags, OC dependencies, etc.)
3. Synthesize a cross-vertical answer with source attribution per vertical
4. Offer to drill into any specific vertical

---

## Contributor Guidelines (for Claude)

- **Never expose personal information** (visa status, relocation, personal finances, health) — these belong in personal Jarvis workspaces, not this shared repo
- **Always attribute updates** with `last_updated` date and source (meeting, Slack, manual)
- **Prefer structured tables** over prose for status, OKRs, and team info
- **Flag stale data**: if `last_updated` on a file is >2 weeks old, note it in responses
- **Ask before overwriting** any field that contains an existing non-empty value

---

## Available Skills

| Skill | Command | Purpose |
|-------|---------|---------|
| Cross-vertical query | `pm-query` | Natural language query across all PM knowledge |
| New joinee onboarding | `pm-onboard` | Structured onboarding walkthrough |
| Update your brain | `pm-update-brain` | Update your own PM brain file |
| Process a meeting | `pm-debrief` | Extract decisions/actions from transcript → update knowledge |
| OKR status check | `pm-status-check` | "Is X vertical on track for Q1?" |

---

## Directory Structure

```
bitgo-pm-intelligence/
├── CLAUDE.md                        ← This file (auto-loaded)
├── README.md                        ← Setup guide for new PMs
├── config.yaml                      ← Connector configuration
├── framework/
│   ├── skills/                      ← Skill definitions
│   └── templates/                   ← Brain file + vertical templates
├── knowledge/
│   ├── shared/                      ← Company-wide knowledge
│   └── verticals/                   ← Per-vertical deep knowledge
│       ├── ecosystem/
│       ├── custody-platform/
│       ├── prime/
│       ├── caas/
│       └── scaas/
├── pms/                             ← One brain file per PM
└── meetings/                        ← Shared cross-vertical meeting notes
```
