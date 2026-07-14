# Log

_Append-only change record. Entry format: `## [YYYY-MM-DD] <type> | <title>` with_
_`<type>` ∈ `setup | plan | ingest | query | lint | persona-qa`._
_Ingest entries end with a synthesis-notes line (the synthesis-debt trail)._

## [2026-07-14] setup | research: biography dossier

Phase-2 web research → `wiki/sources/2026-07-14-research-biography-dossier.md` +
`persona/biography.md` v1. Neil Patel: born 1985 in England to Indian immigrant parents,
raised in Orange County, CA. Registry-verified anchors: NP Digital (CA entity formed
2016-12-29), Ubersuggest acquired 2017-02-13 for $120K, KISSmetrics "supercookie"
settlement (2011–12). Origin arc: teenage hustles → Advice Monkey (failed) → ~$2–3M lost
with Hiten Shah → Crazy Egg (~2005–06) + KISSmetrics (2008); Marketing School podcast
with Eric Siu (2016); NYT-bestseller *Hustle* (2016, co-authored). Flagged self-reported:
Obama/UN "top-100" recognitions (no primary doc found), $100M revenue/net-worth. Open:
exact DOB, CSU Fullerton degree, wife/children names (kept name-free).

## [2026-07-14] setup | research: media inventory dossier

Phase-2 web research → `wiki/sources/2026-07-14-research-media-inventory-dossier.md`.
Two TARGET channels: @neilpatel (UCl-Zrl0QhF66lu1aGXaTbfw, 1.59M subs) and
@MarketingSchoolPod (UCTJmkA2-u7Kyblm5_P6tKdA, co-hosted with Eric Siu → attribution-gated).
Excluded: NP Digital Brasil (Portuguese company channel), dormant @marketingschool
handle-squat, corporate @npdigital, "Neil Patel MD" (different person). Podcast Marketing
School (Apple id1138869817), book *Hustle*, tools Ubersuggest/AnswerThePublic/Hello Bar.

## [2026-07-14] setup | research: entity pages

Phase-2 research → 9 pages in `wiki/entities/` (np-digital, ubersuggest, crazy-egg,
kissmetrics, hello-bar-quick-sprout, marketing-school; context people eric-siu, mike-kamo,
hiten-shah). Revenue/valuation figures flagged self-reported; FTX ~$55M clawback suit
(Nov 2024, Delaware) noted as court-documented and unresolved.

## [2026-07-14] setup | bootstrap: Neil Patel

Repo initialized for Neil Patel — identity user-confirmed 2026-07-14. SUBJECT.md written;
8-domain taxonomy (seo, content-marketing, paid-ads, analytics-cro, social-media,
email-marketing, ai-marketing, agency-entrepreneurship) confirmed, hubs created;
/neilpatel persona alias created; P1/P3 markers added to merge_staging.py. Corpus
enumerated: **4,675 ledger rows, all L0** — @neilpatel 2,461 (1,178 videos + 1,283
shorts), @MarketingSchoolPod 2,214 (827 videos + 1,387 shorts). Priorities: 124 P1 /
1,832 P2 / 2,719 P3; dates+views backfilled for all 2,004 long-form videos, top-50 by
views per channel promoted to P1. One malformed ledger row (comma-in-title) repaired.
Next: /loop /ingest-loop (persona mode only gets good after the first synthesis pass).
