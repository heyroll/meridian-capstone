# Approved decisions log

A running record of design/spec/plan summaries approved during this
capstone project, in the order approved. This file is for the course
record — it is not part of the client-facing wiki and is not read by
Dana Okafor or her team.

---

## Entry 1 — 2026-09-16 — Research wiki design

1. **Scope/purpose:** Built for the entire dashboard engagement — from the
   initial stakeholder interview through final submission to the client —
   not just one meeting.
2. **Audience/tone:** Written for Dana Okafor, her colleagues, and any
   successor who'd need to get up to speed cold. Full sentences, explicit
   reasoning, inline source citations, professional business tone.
3. **Data boundaries:** `docs/data-handling-checklist.md` stays where it
   is; `wiki/SCHEMA.md` restates the core NDA rule (no customer/employee
   data into any AI tool) and links to the full checklist.
4. **Structure:**
   - `raw/` — untouched source documents (client brief, later-ingested
     public articles)
   - `wiki/sources/` — summaries of ingested public sources
   - `wiki/entities/` — people/orgs (Dana Okafor, Meridian Markets, etc.)
   - `wiki/concepts/` — ideas/patterns (e.g. specialty grocer positioning)
   - `wiki/analyses/` — synthesized comparisons/conclusions
   - `wiki/customer-engagement/history.md` — single running dated log of
     meetings, calls, emails, directives, and scope changes (only 4 course
     meetings expected, so no per-meeting files unless one grows large)
   - `wiki/index.md`, `wiki/log.md` — content catalog and operation log
   - `wiki/SCHEMA.md` — the wiki's own instructions/schema, including the
     NDA rule
5. **Course record:** `docs/approved_decisions.md` (this file) — a running,
   dated log of approved summaries only, separate from the client-facing
   wiki.

Formal spec saved to `docs/superpowers/specs/2026-09-16-research-wiki-design.md`.
