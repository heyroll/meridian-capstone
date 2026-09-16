# Implementation plan: Meridian research wiki (initial build)

Spec: `docs/superpowers/specs/2026-09-16-research-wiki-design.md`
Status: Approved (plan) — 2026-09-16
Approved by: Rolland Lopez

This plan builds the initial wiki scaffold only: folders, the wiki's own
instructions, the index, and the log, with the client brief reflected as
the first content.

Execute one task at a time. Each task lists what "done" looks like and
how to check it. Task statuses below get updated to reflect what was
actually completed once the build is finished.

---

## Task 1 — Scaffold the empty wiki category folders

Status: Not started

Create a short `README.md` inside each category folder that doesn't yet
have content, so the folder structure exists in git (which doesn't track
empty folders) and is self-explanatory to anyone browsing the repo:

- `wiki/sources/README.md`
- `wiki/entities/README.md`
- `wiki/concepts/README.md`
- `wiki/analyses/README.md`

Each file states in one or two sentences what belongs in that folder and
points to `wiki/SCHEMA.md` for the full procedure.

**Done looks like:** all four files exist, each with a short, accurate
description and a pointer to `wiki/SCHEMA.md`.

**How to check:** open each file in VS Code and confirm the description
matches its folder's purpose in the spec's Structure section; confirm the
four folders are visible under `wiki/` in the Explorer.

---

## Task 2 — Write `wiki/SCHEMA.md`

Status: Not started

Write the wiki's own instructions file, covering:

- A short overview of the wiki's purpose and structure.
- The ingest procedure (how a new public source becomes a `wiki/sources/`
  summary page, which related pages get updated, and how it's logged).
- The query/answer procedure (how a question gets answered from existing
  pages with citations, and when the answer becomes a new page).
- The customer-engagement procedure (how meetings/calls/emails/directives
  get added to `wiki/customer-engagement/history.md`).
- The data-boundary rule: a direct restatement of the NDA restriction from
  `raw/client-brief.md` (no customer or employee data into any AI tool),
  and a link to `docs/data-handling-checklist.md` for the full checklist.

**Done looks like:** `wiki/SCHEMA.md` exists and covers all five items
above, matching the Source Handling and Data Boundaries sections of the
spec.

**How to check:** read `wiki/SCHEMA.md` side by side with
`docs/superpowers/specs/2026-09-16-research-wiki-design.md`; confirm every
rule described in the spec's Source Handling and Data Boundaries sections
appears here, and that the link to `docs/data-handling-checklist.md`
resolves correctly.

---

## Task 3 — Write `wiki/customer-engagement/history.md`

Status: Not started

Create the file with a short header explaining its purpose (a running,
dated log of meetings, calls, emails, directives, and scope changes with
the client). No entries yet — the first entry gets added after an actual
stakeholder interaction occurs.

**Done looks like:** the file exists with an accurate header and no
fabricated or placeholder entries.

**How to check:** open the file and confirm it explains its own purpose
clearly and contains no invented meeting content.

---

## Task 4 — Write `wiki/deprecated-conclusions.md`

Status: Not started

Create the file with a short header explaining its purpose (a running,
dated record of conclusions declined on review during the query/answer
procedure, kept rather than deleted so they can be reconsidered later).
No entries yet.

**Done looks like:** the file exists with an accurate header and no
placeholder entries.

**How to check:** open the file and confirm it explains its own purpose
clearly and matches the Conclusion review rule in `wiki/SCHEMA.md`.

---

## Task 5 — Write `wiki/index.md`

Status: Not started

Create the wiki's content catalog: one section per category
(`sources`, `entities`, `concepts`, `analyses`, `customer-engagement`,
`deprecated-conclusions`), each noting there are no entries yet, plus an
entry for the client brief in `raw/client-brief.md` as the wiki's first
piece of content, with a one-line description of what it is.

**Done looks like:** `wiki/index.md` lists all six categories and the
client brief, with working relative links.

**How to check:** open the file, click through each link, and confirm it
resolves to the right file or folder.

---

## Task 6 — Write `wiki/log.md`

Status: Not started

Create the append-only operation log with a single dated entry recording
that the initial wiki scaffold (folders, `SCHEMA.md`,
`customer-engagement/history.md`, `deprecated-conclusions.md`,
`index.md`, and the client brief as first content) was created today.

**Done looks like:** `wiki/log.md` exists with one entry, dated, in a
format that stays easy to parse as more entries are appended later.

**How to check:** open the file and confirm the entry accurately
describes what was built in Tasks 1–5.
