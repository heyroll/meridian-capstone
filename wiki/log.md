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

## [2026-09-16] ingest | Sprouts Farmers Market Expanding to Pasadena and Highland Park

Ingested the article at
https://www.coloradoboulevard.net/sprouts-farmers-market-expanding-to-pasadena-and-highland-park/
(published March 11, 2026). Created
`wiki/sources/sprouts-pasadena-expansion-2026.md`, summarizing Sprouts'
pending Pasadena location, existing nearby East Pasadena store, planned
Highland Park location, and nationwide 2026 expansion plans. The page
includes one AI-generated conclusion connecting Sprouts' Pasadena move to
Meridian's own Pasadena decision, marked NEEDS REVIEW pending the user's
decision. No existing entity or concept pages required updates, since
none exist yet.

## [2026-09-16] ingest | Pavilions at California and Lake to Close After Decades Serving Pasadena Community

Ingested the article at
https://www.coloradoboulevard.net/updated-pavilions-at-california-and-lake-to-close-after-decades-serving-pasadena-community/
(published July 8, 2026). Created
`wiki/sources/pavilions-california-lake-closure-2026.md`, summarizing the
closure of Pavilions store #2224 at 845 E. California Blvd (effective
September 5, 2026), the stated lease-expiration/underperformance
reasons, and the open question about restrictive covenants on the
vacated space. The page includes one AI-generated conclusion weighing
this closure against the concurrent Sprouts expansion signal, marked
NEEDS REVIEW pending the user's decision. No existing entity or concept
pages required updates, since none exist yet.

## [2026-09-16] ingest | Amazon Fresh and Amazon Go Stores Closing in California

Ingested the article at
https://www.abc10.com/article/news/local/california/amazon-fresh-stores-california-are-set-to-close-full-list/103-c32e940b-6e46-4e3f-9d50-75d74de04735
(published January 27, 2026; text supplied directly by the user after the
fetch tool was blocked by the site with an HTTP 403). Created
`wiki/sources/amazon-fresh-california-closures-2026.md`, summarizing the
closure of all 22 California Amazon Fresh/Go stores, the planned
conversion of some to Whole Foods, and the inclusion of the Pasadena
location (3425 E Colorado Blvd) on the closure list. The page includes
one AI-generated conclusion weighing this closure, as a third Pasadena
grocery signal, against the Sprouts and Pavilions sources, marked NEEDS
REVIEW pending the user's decision. No existing entity or concept pages
required updates, since none exist yet.

## [2026-09-16] ingest | Amazon Fresh Pasadena — Yelp Reviews

Ingested two Yelp reviews of the Amazon Fresh Pasadena location
(https://www.yelp.com/biz/amazon-fresh-pasadena), text supplied directly
by the user per their "do not read the article, I will copy and paste"
instruction. Public third-party review content about a competitor's
store; confirmed against `docs/data-handling-checklist.md` that this is
not Meridian's own customer/employee data. Created
`wiki/sources/yelp-amazon-fresh-pasadena-reviews-2026.md`, summarizing
the two reviews and using their dates to establish the Pasadena Amazon
Fresh was closed by at least March 16, 2026, with a reviewer-reported
(unconfirmed) last day of March 13, 2026, narrowing the open closure-date
question from `wiki/sources/amazon-fresh-california-closures-2026.md`.
The page includes one AI-generated conclusion marked NEEDS REVIEW
pending the user's decision. No existing entity or concept pages
required updates, since none exist yet.

## [2026-09-16] ingest | 3405–3425 E Colorado Blvd, Pasadena — LoopNet Listing

Ingested a LoopNet sublease listing
(https://www.loopnet.com/Listing/3405-3425-E-Colorado-Blvd-Pasadena-CA/40060500/),
text supplied directly by the user after the fetch tool was blocked by
the site with an HTTP 403. Created
`wiki/sources/loopnet-3405-3425-colorado-blvd-listing-2026.md`,
summarizing the property facts (41,990 SF available, 44,204 SF gross
leasable area, 3.80 acres, built 1971, sublease structure) and select
center tenants for the site at 3405–3425 E Colorado Blvd — the same
address as the closed Amazon Fresh covered in
`wiki/sources/amazon-fresh-california-closures-2026.md` and
`wiki/sources/yelp-amazon-fresh-pasadena-reviews-2026.md`. The page
includes one AI-generated conclusion marked NEEDS REVIEW pending the
user's decision. No existing entity or concept pages required updates,
since none exist yet.

## [2026-09-16] edit | Reorganized the Sources section of wiki/index.md

At the user's request, grouped the Sources section in `wiki/index.md`
under three headers: CLOSURES (Amazon Fresh California closures, the
Yelp reviews, the LoopNet listing, and the Pavilions closure — the three
Amazon-related sources grouped together as asked), EXPANSIONS (the
Sprouts source), and INDUSTRY TRENDS (the ICSC source). No source pages
themselves were changed, only their ordering and grouping in the index.
