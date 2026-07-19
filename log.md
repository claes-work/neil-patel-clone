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

## [2026-07-19] ingest | yt batch (@neilpatel, 8) — first L2 batch

First real ingest batch. Stage machine (`.claude/commands/ingest-loop.md`, first-match)
selected **Stage B** (open P1 long-form rows exist); Stage S not due (0 batches since
synthesis, checkpoint at 10) and Stage P skipped (nothing ingested yet to refine the
persona from — the "first-run persona-stale" clause has no material until L2 exists).
Channel @neilpatel (Neil-fronted primary corpus, persona-first). Selection = clone's own
rule: priority-ascending then oldest-`published` first → 8 oldest P1 rows (2016–2017).
The 4 roster fresh-upload P1 rows are the *newest* P1, so oldest-first did not surface
them (and prepare is single-channel / no cherry-pick); left for a later batch.

Processed: 8 ingested (L2), 0 skipped, 0 no-captions, 0 dup. All captions fetched clean
on the first try — no rate limiting. One ledger title mismatch found: `yt-KsZIVpkpte0`
"Get More Visitors And Sales - Free Webinar" is actually a Domain-Authority-vs-PageRank
SEO lesson — page + index reflect the real content, ledger row noted. Two rows flagged
★ L3-candidate for the next synthesis: `yt-BkR7L41SroU` (backlinks explainer) and
`yt-wWiSShEGyHA` (competitive-SEO-with-no-budget framework).

Ledger after: L2=8, L3=0. Open long-form P1 @neilpatel 60, @MarketingSchoolPod 60
(120 total P1 remaining); P2 ~1,831; open shorts ~2,682. Ingest batches since last
synthesis: 1 (checkpoint at 10).

Synthesis notes: several genuinely-new persona signals (promote at next Stage S) —
(1) biographical spine from the "5 minutes a day" about-video: first website at 16 funded
with amusement-park money, an early failed marketing-firm hire pushing him to self-teach,
first client a power-supply maker he claims he helped add $25M in sales; recurring thesis
"marketing isn't expensive or hard, there's a formula anyone can follow." (2) SEO mental
model: rising domain authority as a *leading indicator* that precedes ranking/traffic
gains (which lag 6–18 months); prefers a frequently-updated backlink index (Ahrefs) over
Moz/PageRank. (3) Competitive-SEO no-budget framework: roundup posts for fast links →
keyword-density/content-depth research → title/meta CTR optimization (CTR-drives-rankings).
(4) Blog-writing template: intro → 3–7 body headings → conclusion → fill; ≤6-line
paragraphs, conversational "you and I", 6–7+ images. (5) Distribution tactic: republish
full posts on LinkedIn with a "continue reading" cutoff back to the owned site; physical
insert-cards in shipped products to prompt Instagram tag-and-post. All dated 2016–2017.
