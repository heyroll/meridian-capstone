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

## [2026-09-17] ingest | Census QuickFacts — Pasadena Population

Ingested population figures from the U.S. Census Bureau's QuickFacts
page for Pasadena city, California
(https://www.census.gov/quickfacts/fact/table/pasadenacitycalifornia/PST040225),
text supplied directly by the user after the fetch tool was blocked by
the site with an HTTP 403. Created
`wiki/sources/census-quickfacts-pasadena-population-2026.md`, stating
four figures: the 2010 and 2020 decennial census counts (137,122 and
138,699), the 2020 Vintage 2025 estimates base (139,618, a revised
figure distinct from the raw 2020 count), and the July 1, 2025 estimate
(135,804). The page flags the reversal from slow growth (2010→2020) to
decline (2020→2025) as a notable pattern, per the user's explicit
instruction to draw attention to the estimate change without drawing a
conclusion about its cause or implications. Unlike prior source pages,
this page has no "Relevance to Meridian" section and contains no
AI-generated conclusion. Added to the Sources section of
`wiki/index.md` under a new "Demographics" subheading. No existing
entity, concept, or analysis pages required updates.

## [2026-09-17] edit | Changed Sources link display text in wiki/index.md

At the user's request, changed how each entry in the Sources section of
`wiki/index.md` displays its link: instead of showing the file path
(e.g. `wiki/sources/amazon-fresh-california-closures-2026.md`) as the
visible text, each link now displays that page's own title (its `# `
heading), e.g. "Amazon Fresh and Amazon Go Stores Closing in
California." The link targets themselves are unchanged. The "First
content" entry for `raw/client-brief.md` was left as-is, since the
request was scoped to the Sources section.

## [2026-09-17] ingest | Councilmember Confirms Sprouts Will Fill Vacant Rite Aid on Hill Avenue

Ingested the article at
https://pasadenanow.com/main/councilmember-says-sprouts-will-soon-fill-the-vacant-rite-aid-on-hill-avenue
(published September 9, 2026). Created
`wiki/sources/sprouts-hill-avenue-confirmation-2026.md`, recording
District 2 Councilmember Rick Cole's public confirmation that Sprouts
will fill the former Rite Aid on Hill Avenue — the same location (1421
E. Washington Blvd) already tracked in
`wiki/sources/sprouts-pasadena-expansion-2026.md` as a pending, unconfirmed
permit application from March 2026. No firm opening date is given. The
page includes one AI-generated conclusion marked NEEDS REVIEW noting
this upgrades the certainty of that expansion from "pending filing" to
"publicly confirmed." Restructured the Pasadena Expansions section of
`wiki/index.md` to add a "Sprouts" subheading (mirroring the existing
Amazon Fresh subheading under Pasadena Closures) grouping both the March
source and this new confirmation source together.

## [2026-09-17] ingest | Census QuickFacts — Pasadena Income

Ingested two income figures from the same U.S. Census Bureau QuickFacts
page for Pasadena city, California used for the population source
(https://www.census.gov/quickfacts/fact/table/pasadenacitycalifornia/PST040225),
figures supplied directly by the user. Created
`wiki/sources/census-quickfacts-pasadena-income-2026.md`, stating median
household income (in 2024 dollars), 2020-2024 ($105,192) and per capita
income in the past 12 months (in 2024 dollars), 2020-2024 ($65,304).
Kept as a separate page from the population source since it covers a
different topic from the same table. Matching the population page, this
page states facts only, with no "Relevance to Meridian" section and no
AI-generated conclusion. Added to the Demographics subheading of the
Sources section in `wiki/index.md`. No existing entity, concept, or
analysis pages required updates.

## [2026-09-17] edit | Consolidated the two Census QuickFacts source pages

At the user's request, merged `wiki/sources/census-quickfacts-pasadena-population-2026.md`
and `wiki/sources/census-quickfacts-pasadena-income-2026.md` into a
single new page, `wiki/sources/census-quickfacts-pasadena-population-income-2026.md`,
under the title "Census QuickFacts: Pasadena, California — Population &
Income," with a "Population" section and an "Income" section carrying
over the same facts and notes unchanged. This reverses the prior
decision (recorded in the two entries above) to keep them as separate
pages. Deleted the two old source files and updated the Demographics
subheading of the Sources section in `wiki/index.md` to a single entry
pointing at the merged page, using that title as its link text. No
existing entity, concept, or analysis pages required updates.

## [2026-09-17] ingest | FMI — Study Highlights Grocery Stores' Expanding Role in Convenient, Affordable Dining

Ingested the FMI press release at
https://www.fmi.org/newsroom/news-archive/view/2025/10/07/study-highlights-grocery-stores--expanding-role-in-convenient--affordable-dining
(published October 7, 2025; a separate URL for a Restaurant Business
Online article on the same topic was initially requested but abandoned
by the user after WebFetch was blocked with an HTTP 403). Fetched via
WebFetch, then verified all four cited statistics and three named
quotes against the raw HTML (downloaded to the scratchpad directory)
before writing anything. Created
`wiki/sources/fmi-deli-restaurant-competitor-2025.md`, summarizing the
report's finding that deli-prepared food preference over restaurant
meals rose from 12% (2017) to 28% (2025), the 53% hybrid-meal stat, the
1.6% retail foodservice sales growth to $52.1 billion, the noon–5 p.m.
peak purchase window, and quotes from three named FMI staff. The page
flags that the source is FMI's own promotional press release for a
report it sells, and includes one AI-generated conclusion connecting
the prepared-foods trend to Meridian's stated strategy, marked NEEDS
REVIEW pending the user's decision. Added to the Industry Trends
subheading of the Sources section in `wiki/index.md`. No existing
entity, concept, or analysis pages required updates.

## [2026-09-17] edit | Approved the NEEDS REVIEW conclusion on the FMI source page

At the user's request, approved the AI-generated conclusion in the
"Relevance to Meridian" section of
`wiki/sources/fmi-deli-restaurant-competitor-2025.md`: removed the
**NEEDS REVIEW** mark, keeping the conclusion text itself unchanged as
accepted content. Removed the corresponding "Contains one AI-generated
conclusion marked NEEDS REVIEW" note from that source's entry in the
Industry Trends subheading of `wiki/index.md`.

## [2026-09-17] edit | Approved the NEEDS REVIEW conclusion on the ICSC source page

At the user's request, approved the AI-generated conclusion in the
"Relevance to Meridian" section of
`wiki/sources/icsc-grocery-formats-2026.md`: removed the **NEEDS
REVIEW** mark, keeping the conclusion text itself unchanged as accepted
content. Removed the corresponding "Contains one AI-generated
conclusion marked NEEDS REVIEW" note from that source's entry in the
Industry Trends subheading of `wiki/index.md`.

## [2026-09-17] edit | Approved the NEEDS REVIEW conclusion on the Sprouts Hill Avenue confirmation page

At the user's request, approved the AI-generated conclusion in the
"Relevance to Meridian" section of
`wiki/sources/sprouts-hill-avenue-confirmation-2026.md`: removed the
**NEEDS REVIEW** mark, keeping the conclusion text itself unchanged as
accepted content. Removed the corresponding "Contains one AI-generated
conclusion marked NEEDS REVIEW" note from that source's entry under the
Sprouts subheading of the Pasadena Expansions section in
`wiki/index.md`. The page's separate "PAGE STATUS: NEEDS CLEANUP" note
(on redundant content in the Key facts section) was left untouched, as
it is unrelated to this request.

## [2026-09-17] edit | Resolved redundancy and removed cleanup flag on the Sprouts Hill Avenue confirmation page

At the user's request, rewrote bullet 4 under "Key facts from the
article" in `wiki/sources/sprouts-hill-avenue-confirmation-2026.md` to
the user's supplied wording on Cole's store-count comparison (Sprouts'
~500 stores nationwide vs. ~2,200 for Albertsons/Vons and ~2,700 for
Kroger/Ralphs, and the "giants" taking "an ever-growing share of
grocery sales"), verified against the article's raw text via WebFetch
before writing. This removed the overlap with bullet 5's zoning-code
quote that the page's "PAGE STATUS: NEEDS CLEANUP" note had flagged, so
that note was removed at the user's request.

## [2026-09-17] edit | Approved the NEEDS REVIEW conclusion on the Sprouts Pasadena expansion page

At the user's request, approved the AI-generated conclusion in the
"Relevance to Meridian" section of
`wiki/sources/sprouts-pasadena-expansion-2026.md`: removed the **NEEDS
REVIEW** mark, keeping the conclusion text itself unchanged as accepted
content. Removed the corresponding "Contains one AI-generated
conclusion marked NEEDS REVIEW" note from that source's entry under the
Sprouts subheading of the Pasadena Expansions section in
`wiki/index.md`.

## [2026-09-17] edit | Approved the NEEDS REVIEW conclusion on the Pavilions closure page, and activated a cross-reference link

At the user's request, approved the AI-generated conclusion in the
"Relevance to Meridian" section of
`wiki/sources/pavilions-california-lake-closure-2026.md`: removed the
**NEEDS REVIEW** mark, keeping the conclusion text itself unchanged as
accepted content. Removed the corresponding "Contains one AI-generated
conclusion marked NEEDS REVIEW" note from that source's entry under the
Pasadena Closures section in `wiki/index.md`. Also, in that same
"Relevance to Meridian" paragraph, turned the plain-text reference to
`wiki/sources/sprouts-pasadena-expansion-2026.md` into an active
markdown link ("Sprouts expansion").

## [2026-09-17] edit | Approved the NEEDS REVIEW conclusion on the LoopNet listing page

At the user's request, approved the AI-generated conclusion in the
"Relevance to Meridian" section of
`wiki/sources/loopnet-3405-3425-colorado-blvd-listing-2026.md`: removed
the **NEEDS REVIEW** mark, keeping the conclusion text itself unchanged
as accepted content. Removed the corresponding "Contains one
AI-generated conclusion marked NEEDS REVIEW" note from that source's
entry under the Amazon Fresh subheading of the Pasadena Closures
section in `wiki/index.md`.

## [2026-09-18] edit | Approved the NEEDS REVIEW conclusion on the Yelp reviews page, and fixed link display text

At the user's request, approved the AI-generated conclusion in the
"Relevance to Meridian" section of
`wiki/sources/yelp-amazon-fresh-pasadena-reviews-2026.md`: removed the
**NEEDS REVIEW** mark, keeping the conclusion text itself unchanged as
accepted content. Removed the corresponding "Contains one AI-generated
conclusion marked NEEDS REVIEW" note from that source's entry under the
Amazon Fresh subheading of the Pasadena Closures section in
`wiki/index.md`. Also changed both links on that page pointing to
`wiki/sources/amazon-fresh-california-closures-2026.md` (in the Key
facts and Relevance to Meridian sections) to display that page's title,
"Amazon Fresh and Amazon Go Stores Closing in California," instead of
the raw file path.

## [2026-09-18] edit | Trimmed the Relevance to Meridian paragraph on the Amazon Fresh closures page

At the user's request, edited the "Relevance to Meridian" paragraph on
`wiki/sources/amazon-fresh-california-closures-2026.md`: removed its
first sentence (which framed this as "the third Pasadena-area grocery
signal in the wiki," cross-referencing the Sprouts and Pavilions
source pages), and changed the opening of the following sentence from
"Unlike the Pavilions closure, this one" to "This article." The
paragraph's substance — that this is a blanket, nationwide-strategy
closure rather than Pasadena-specific evidence — is otherwise
unchanged. The conclusion remains marked NEEDS REVIEW.

## [2026-09-18] edit | Approved the NEEDS REVIEW conclusion on the Amazon Fresh closures page

At the user's request, approved the AI-generated conclusion in the
"Relevance to Meridian" section of
`wiki/sources/amazon-fresh-california-closures-2026.md`: removed the
**NEEDS REVIEW** mark, keeping the conclusion text itself unchanged as
accepted content. Removed the corresponding "Contains one AI-generated
conclusion marked NEEDS REVIEW" note from that source's entry under the
Amazon Fresh subheading of the Pasadena Closures section in
`wiki/index.md`.

## [2026-09-18] ingest | JLL — Grocery Tracker (2025 Grocery Report)

Ingested the JLL market-research report at
https://www.jll.com/en-us/insights/market-perspectives/grocery-tracker
(published February 18, 2025; updated March 24, 2025). Verified the
large majority of its cited statistics against the raw page HTML
(downloaded to the scratchpad directory) before writing anything,
including figures that WebFetch had surfaced from JS-rendered Flourish
chart embeds — located the matching editorial-text paragraphs stating
the same figures directly so they could be confirmed too. Created
`wiki/sources/jll-grocery-tracker-2025.md`, covering the full report per
the user's request: the dining-out-vs-grocery spending gap and foot
traffic trends, grocery-anchored real estate fundamentals (3.5%
vacancy, minimal new supply, rent growth, record price/sq ft),
investment activity, 2024 grocer-by-grocer expansion figures (Aldi,
Publix, H-E-B, Sprouts, Trader Joe's, Fresh Market, Amazon Fresh),
notable 2024 M&A activity (including the FTC blocking Kroger-Albertsons
in December 2024), private-label growth, and SNAP/e-commerce/retail-media
stats. The page flags the source as JLL's own commercial market
research. Includes one AI-generated conclusion connecting the national
real-estate fundamentals and Sprouts' smaller-footprint growth data to
Meridian's situation, marked NEEDS REVIEW pending the user's decision.
Added to the Industry Trends subheading of the Sources section in
`wiki/index.md`. No existing entity, concept, or analysis pages
required updates.

## [2026-09-18] edit | Various user-requested wording edits on the JLL source page

At the user's request, made a series of small wording edits to
`wiki/sources/jll-grocery-tracker-2025.md`: added "(Restaurant & Bars >
Grocery Stores)" to the dining-vs-grocery spending gap bullet; added
"(real estate demand)" after "net absorption" and "(real estate
supply)" after "net deliveries"; changed "and grocery operators" to ",
while grocery operators" and "became more active" to "instead became
more active" in the investment-activity bullet (flagged to the user
that this leaves the REITs clause without its own verb; not yet
resolved); removed the Canadian grocers section entirely; expanded "per
PLMA" to "per the Private Label Manufacturer Association (PLMA)";
changed "GO Brands" to "Go Brands" (the source's own data table,
unlike its narrative text, already spells it this way); removed
boldface from the Real Root mention; and, after explaining that the
private-label launches bullet only reflected the article's narrative
paragraph rather than its full data table, added three more launches
from that table at the user's request: Albertsons' "Overjoyed," Giant
Food Holdings' "New Coast Foraging Company," and SpartanNash's "Finest
Reserve." Also moved "(over 12% of the U.S. population)" earlier in the
SNAP bullet, and changed "This report gives the wiki its first hard"
to "This report contains hard" in the Relevance to Meridian paragraph.

## [2026-09-18] edit | Approved the NEEDS REVIEW conclusion on the JLL source page

At the user's request, approved the AI-generated conclusion in the
"Relevance to Meridian" section of
`wiki/sources/jll-grocery-tracker-2025.md`: removed the **NEEDS
REVIEW** mark, keeping the conclusion text itself unchanged as accepted
content. Removed the corresponding "Contains one AI-generated
conclusion marked NEEDS REVIEW" note from that source's entry under the
Industry Trends subheading of `wiki/index.md`.

## [2026-09-18] ingest | Grocery Dive — Why Specialty Grocers Are Thriving Post-Pandemic

Ingested the article at
https://www.grocerydive.com/news/specialty-grocers-post-covid-pandemic-inflation-health-wellness-Sprouts-Farmers-Market-Whole-Foods/808272/
(published December 18, 2025, by Peyton Bigora). Verified all cited
statistics and quotes against the raw page HTML (downloaded to the
scratchpad directory) before writing anything. Created
`wiki/sources/grocerydive-specialty-grocers-thriving-2025.md`,
summarizing the article's explanation for specialty grocers'
post-pandemic outperformance: Placer.ai foot-traffic data, Sprouts'
2020–2022 comp-sales dip and recovery, and named-source commentary
(Errol Schweizer, James Ren, Stewart Samuel) on price inflation, wealth
bifurcation, organic price-gap narrowing, private label, loyalty-program
personalization, and curated assortment. Includes one AI-generated
conclusion connecting these growth drivers to Meridian's stated
strategy and flagging the NDA boundary on checking wealth-bifurcation
claims against Meridian's own customer data, marked NEEDS REVIEW
pending the user's decision. Added to the Industry Trends subheading of
the Sources section in `wiki/index.md`. No existing entity, concept, or
analysis pages required updates.

## [2026-09-18] edit | Wording edits on the Grocery Dive source page

At the user's request, made several wording edits to
`wiki/sources/grocerydive-specialty-grocers-thriving-2025.md`: moved
the "Private label as a value signal" bullet to directly after "Price
inflation's role"; removed "disposable-" from the wealth-bifurcation
bullet; moved the wealth-bifurcation bullet to before "Price inflation's
role" (updating its internal cross-reference from "above" to "below"
accordingly); changed "per Ren" to "According to the article, per Ren,"
in the health/wellness bullet; and changed "This article gives the wiki
its first sourced explanation of *why*" to "This article gives an
explanation of *why*" in the Relevance to Meridian paragraph.

## [2026-09-18] edit | Approved the NEEDS REVIEW conclusion on the Grocery Dive source page

At the user's request, approved the AI-generated conclusion in the
"Relevance to Meridian" section of
`wiki/sources/grocerydive-specialty-grocers-thriving-2025.md`: removed
the **NEEDS REVIEW** mark, keeping the conclusion text itself unchanged
as accepted content. Removed the corresponding "Contains one
AI-generated conclusion marked NEEDS REVIEW" note from that source's
entry under the Industry Trends subheading of `wiki/index.md`.
