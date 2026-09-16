# Wiki schema and instructions

This file explains how this research wiki is organized and how to work in
it — for any human or AI picking it up, at any point in the engagement.

## Purpose and structure

This wiki supports the Meridian Markets dashboard engagement from the
initial stakeholder interview through final submission to the client. It
is written for Dana Okafor, her colleagues, and any successor who might
need to get up to speed without shared context — pages use full sentences
and explicit reasoning, and state their source inline.

- [`wiki/sources/`](sources/README.md) — one summary page per ingested
  public source.
- [`wiki/entities/`](entities/README.md) — pages on people and
  organizations.
- [`wiki/concepts/`](concepts/README.md) — pages on ideas and patterns
  relevant to the analysis.
- [`wiki/analyses/`](analyses/README.md) — synthesized comparisons and
  conclusions.
- [`wiki/customer-engagement/history.md`](customer-engagement/history.md)
  — a running, dated log of meetings, calls, emails, directives, and
  scope changes with the client.
- [`wiki/index.md`](index.md) — a catalog of every page in this wiki,
  with a one-line summary each.
- [`wiki/log.md`](log.md) — an append-only chronological record of wiki
  operations (ingests, queries, edits), separate from
  [`customer-engagement/history.md`](customer-engagement/history.md).
- [`wiki/deprecated-conclusions.md`](deprecated-conclusions.md) — a
  running, dated record of conclusions that were declined on review (see
  the Query and answer procedure below), kept so they can be reconsidered
  later rather than lost.

## Ingest procedure

When a new public source is added to [`raw/`](../raw/):

1. Read it and discuss the key takeaways with the user before writing
   anything.
2. Write a summary page in [`wiki/sources/`](sources/README.md).
3. Update any related entity, concept, or analysis pages the source
   touches.
4. Add or update the corresponding entries in [`wiki/index.md`](index.md).
5. Append an entry to [`wiki/log.md`](log.md) recording the ingest.

## Query and answer procedure

When asked a question against the wiki:

1. Read [`wiki/index.md`](index.md) to find the relevant pages.
2. Synthesize an answer from those pages, citing the source page (or
   original URL) for every claim.
3. Label any conclusion that isn't directly stated in a source as a
   conclusion added by whoever synthesized it (e.g. "AI-generated
   conclusion, not stated in the source" or "Rolland's conclusion, not
   stated in the source"), and mark it **NEEDS REVIEW** directly on the
   page — never blended in as if it were a sourced claim.
4. Present the answer, including any NEEDS REVIEW conclusions, for
   review. The user decides the outcome of each such conclusion:
   - **Approved** — remove the NEEDS REVIEW mark; the conclusion stays on
     the page as accepted content.
   - **Declined** — remove the conclusion from the page and move it,
     along with its original context (which page it was on, its citation
     trail, the date added, and the date declined), to
     [`wiki/deprecated-conclusions.md`](deprecated-conclusions.md). It is
     never deleted outright, so it can be reconsidered later — a
     conclusion rejected today may turn out to have been right once more
     evidence exists.
5. If the user decides the answer as a whole is worth keeping as its own
   page, file it (typically under [`wiki/analyses/`](analyses/README.md))
   with its citations, and add it to [`wiki/index.md`](index.md) and
   [`wiki/log.md`](log.md) — only when the user asks for it to be filed,
   not automatically.

## Customer engagement procedure

Meetings, calls, emails, and directives from Dana or her team are not
"sources" — they go directly into
[`wiki/customer-engagement/history.md`](customer-engagement/history.md)
as a new dated entry, including any scope changes or new directives they
contain. This file does not require an index or log update on its own.

## Data boundary — read this before ingesting or citing anything

Per the NDA terms in [`raw/client-brief.md`](../raw/client-brief.md):
**customer records and
employee data — including loyalty program data, labor schedules, and any
excerpts of them — must never be entered into this wiki or any AI tool.**
Only aggregated sales totals by store and week, and store attributes
(square footage, opening date, lease terms), are cleared for that use.

Before ingesting or citing anything, run the pre-flight check in
[`docs/data-handling-checklist.md`](../docs/data-handling-checklist.md),
which has the full data classification table and guidance on derived and
aggregated data. If a dataset isn't already classified there, treat it as
restricted until it is — don't guess in the moment.
