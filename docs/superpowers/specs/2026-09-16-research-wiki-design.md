# Spec: Meridian research wiki

Status: Approved (design) — 2026-09-16
Approved by: Rolland Lopez

## Purpose

A research wiki that supports the full Meridian Markets dashboard engagement —
from the initial stakeholder interview through final submission to the
client — not a one-time interview-prep document. It accumulates research,
client-interaction history, and analysis over the life of the project so
that knowledge compounds instead of being re-derived each time it's needed.

## Audience and tone

The wiki is written for Dana Okafor (VP of Operations, primary stakeholder),
her colleagues, and any successor who might need to pick up this project
without shared context. Every page uses full sentences and explicit
reasoning — not shorthand — and states its source inline rather than
assuming the reader already knows where a fact came from. Tone is
professional/consulting, not academic or casual.

## Structure

- [`raw/`](../../../raw/) — source documents, unmodified. Currently
  [`client-brief.md`](../../../raw/client-brief.md).
- [`wiki/sources/`](../../../wiki/sources/README.md) — one summary page
  per ingested public source.
- [`wiki/entities/`](../../../wiki/entities/README.md) — pages on people
  and organizations (e.g. Dana Okafor, Meridian Markets).
- [`wiki/concepts/`](../../../wiki/concepts/README.md) — pages on
  ideas/patterns relevant to the analysis (e.g. specialty grocer
  positioning).
- [`wiki/analyses/`](../../../wiki/analyses/README.md) — synthesized
  comparisons and conclusions that draw on multiple
  sources/entities/concepts.
- [`wiki/customer-engagement/history.md`](../../../wiki/customer-engagement/history.md)
  — a single running, dated log of meetings, calls, emails, directives,
  and scope changes with the client. Kept as one file rather than one
  file per interaction; a specific entry can be split into its own file
  later if it grows large enough to warrant it.
- [`wiki/index.md`](../../../wiki/index.md) — a catalog of every wiki
  page with a one-line summary each, updated whenever a page is added or
  changed.
- [`wiki/log.md`](../../../wiki/log.md) — an append-only chronological
  record of wiki operations (ingests, queries, lint passes), independent
  of `customer-engagement/history.md`, which records the client
  relationship rather than wiki maintenance.
- [`wiki/deprecated-conclusions.md`](../../../wiki/deprecated-conclusions.md)
  — a single running, dated record of conclusions declined on review (see
  Source handling below), kept rather than deleted so they can be
  reconsidered later.
- [`wiki/SCHEMA.md`](../../../wiki/SCHEMA.md) — instructions for whoever
  (human or AI) works on the wiki: its structure, conventions, the
  ingest/answer procedures, and the data-boundary rule below.

## Source handling

- **Ingest:** when a new public source is added to
  [`raw/`](../../../raw/), it is read and discussed with the user before
  a summary page is written to
  [`wiki/sources/`](../../../wiki/sources/README.md). The summary page,
  any related entity/concept pages it touches,
  [`wiki/index.md`](../../../wiki/index.md), and
  [`wiki/log.md`](../../../wiki/log.md) are all updated as part of the
  same ingest.
- **Citation:** any claim in the wiki drawn from a source must cite that
  source (link to its [`wiki/sources/`](../../../wiki/sources/README.md)
  page or the original URL). A claim that is a conclusion rather than
  something a source states must be labeled as such and attributed to
  whoever added it (the AI assistant or the user), never blended in
  silently as if it were sourced.
- **Conclusion review:** any new conclusion is marked NEEDS REVIEW
  directly on the page where it's added. The user decides, per
  conclusion, whether to approve it (the mark is removed and it stays as
  accepted content) or decline it (it is moved, with its original context
  and citation trail, to
  [`wiki/deprecated-conclusions.md`](../../../wiki/deprecated-conclusions.md)
  rather than deleted, so it can be reconsidered later).
- **Query/answer:** when the user asks a question against the wiki, the
  answer is synthesized from existing pages with citations, following the
  citation and conclusion-review rules above. If the user decides the
  answer is worth keeping as its own page, it is filed (e.g. under
  [`wiki/analyses/`](../../../wiki/analyses/README.md)) with its
  citations, and added to [`wiki/index.md`](../../../wiki/index.md) and
  logged in [`wiki/log.md`](../../../wiki/log.md) — only when the user
  asks for it to be filed, not automatically.
- **Customer engagement:** meetings, calls, emails, and directives from
  Dana or her team are not "sources" in the above sense — they are added
  as dated entries directly to
  [`wiki/customer-engagement/history.md`](../../../wiki/customer-engagement/history.md),
  including any scope changes or new directives they contain.

## Data boundaries

Per the NDA terms in [`raw/client-brief.md`](../../../raw/client-brief.md),
customer records and employee data (loyalty program data, labor
schedules, and any excerpts of them) must never be entered into this wiki
or any AI tool. Only aggregated sales totals by store and week, and store
attributes (square footage, opening date, lease terms), are cleared for
that use. The full classification and pre-flight checklist live in
[`docs/data-handling-checklist.md`](../../data-handling-checklist.md),
which stays in place; [`wiki/SCHEMA.md`](../../../wiki/SCHEMA.md)
restates this core rule directly and links to the full checklist, so it
cannot be missed by anyone (human or AI) working in the wiki without
first opening a separate document.

## Proposed result

At the end of the initial build, the wiki consists of: the folder
structure above, [`wiki/SCHEMA.md`](../../../wiki/SCHEMA.md) with the
ingest/answer procedures and the data-boundary rule,
[`wiki/index.md`](../../../wiki/index.md) and
[`wiki/log.md`](../../../wiki/log.md), and the client brief present in
[`raw/`](../../../raw/) as the wiki's first content, reflected in
[`wiki/index.md`](../../../wiki/index.md).
