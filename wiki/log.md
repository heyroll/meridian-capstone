# Wiki log

An append-only, chronological record of operations on this wiki (builds,
ingests, queries). Newest entries go at the bottom. See
[`wiki/SCHEMA.md`](SCHEMA.md) for the procedures these entries follow.

Entries this file does not cover: the client relationship itself, which
is recorded separately in
[`wiki/customer-engagement/history.md`](customer-engagement/history.md).

---

## [2026-09-16] build | Initial wiki scaffold created

Created the initial wiki structure: the `sources/`, `entities/`,
`concepts/`, and `analyses/` category folders (each with a short README);
`wiki/SCHEMA.md` with the ingest, query/answer, and customer-engagement
procedures plus the NDA data-boundary rule; `wiki/customer-engagement/history.md`
and `wiki/deprecated-conclusions.md` as empty running logs; and
`wiki/index.md` cataloging all of the above along with `raw/client-brief.md`
as the wiki's first content. No public sources have been ingested and no
questions have been answered yet.

## [2026-09-16] ingest | ICSC — Grocery Strategies Shift: New Formats, Store Growth and Investment

Ingested the article at
https://www.icsc.com/news-and-views/icsc-exchange/new-grocery-formats-store-growth-and-investment-signal-sector-in-motion
(published April 24, 2026). Created `wiki/sources/icsc-grocery-formats-2026.md`,
summarizing its key facts on specialty grocer performance, smaller-footprint
formats, and grocery-anchored real estate investment. The page includes
one AI-generated conclusion connecting these trends to Meridian's
positioning, marked NEEDS REVIEW pending the user's decision. No existing
entity or concept pages required updates, since none exist yet.
