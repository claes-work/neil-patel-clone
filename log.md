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

## [2026-07-19] ingest | yt batch (@neilpatel, 8) — P1 long-form #2

Second real ingest batch. Stage machine (`.claude/commands/ingest-loop.md`, first-match)
selected **Stage B** (open P1 long-form rows exist). Not-taken rules: Stage S not due
(1 batch since synthesis, checkpoint at 10; no `>>> CHECKPOINT`); Stage P not stale
(the 2026-07-19 batch #1 was the documented "first run" that already resolved the
first-run persona clause — only 1 batch since, no new topic pages, P1 far from drained);
Stage A n/a (both TARGET channels enumerated). Channel @neilpatel (Neil-fronted primary
corpus, persona-first). Selection = clone's own rule: priority-ascending then
oldest-`published` first → next 8 oldest open P1 rows (2017-11 → 2018-02).

Processed: **8 ingested (L2), 0 skipped, 0 no-captions, 0 dup.** All captions fetched
clean on the first try — no rate limiting. Three rows flagged **★ L3-candidate** for the
next synthesis: `yt-k_eXA4cY53M` (origin story — 4 businesses by 28), `yt-0-77jMAF1bw`
(failure story — lost $1M at 21), `yt--p6CvtzUgk0` (TAM-governs-outcomes billion-dollar
framework). Caption garbles caught and handled in-page (not carried into paraphrase):
"vitex"→likely VTEX Day, "on page SU"→SEO / "rand"→rank (jhnNOlhPbyc), "Sam Evans"→Sam
Ovens of Consulting.com (HJUm-MwLJMg). All 8 are solo Neil videos → fully Neil-attributed;
self-reported revenue/net-worth/family claims marked as such. No contradictions.

Ledger after: L2=16, L3=0. Open long-form P1 @neilpatel 52, @MarketingSchoolPod 60
(112 total P1 remaining); P2 ~1,831; open shorts ~2,682. Ingest batches since last
synthesis: 2 (checkpoint at 10).

Synthesis notes: strong new persona/bio spine to promote at next Stage S —
(1) Biography/origin: ran an ad agency at 16 (learned marketing after being ripped off
by agencies); lost ~$1M by 21 on a failed pre-AWS cloud-computing startup that never
launched — money was *borrowed*, repaid in under a year; claims 4 multimillion-dollar
businesses by 28; Cal State Fullerton "mediocre college" self-deprecation; extreme
work-ethic lifestyle claims (80–90 hrs/week, "no home", works 24/7) — all self-reported.
(2) Entrepreneurship frameworks: **TAM governs outcomes** — pick a big-market problem;
validates market size via Google Finance market caps + Google Trends (10x vs "digital
marketing" benchmark); rare self-critical admission that Crazy Egg was capped by too-small
a problem and "I haven't built a billion-dollar company yet"; combine multiple marketing
products into one big-TAM company. Relayed mentor lines: Branson "ideas are like buses",
Brian Lee "one product, laser focus, expand when growth flatlines" (attributed as relayed).
(3) SEO: content-depth + Search Console keyword-mining to expand articles (2,500→10,000
words, traffic tripled in ~50 days); single-niche exhaustive depth (Hummingbird-era);
**brand queries as a ranking factor** (BMW vs GM via Google Trends); on-page + CTR tuning
can lift rankings "without building a single link"; 7 named free tools (Quick Sprout, Yoast,
Search Console, Google Trends, Screaming Frog, PageSpeed Insights, responsive-test).
(4) Link building: reverse-engineer a competitor's top-linked content in Ahrefs, rebuild as
a cited infographic, pitch the competitor's existing linkers. (5) Video/YouTube SEO:
end-of-video subscribe CTA "tripled" subscriber gains; upload real transcripts (not auto-
captions) to rank; emotional content + embed-outreach. (6) CRO: lead-capture pages 40%+ /
product pages ~3–10% conversion benchmarks; video can lower conversion rate but raise
customer quality/LTV — test it; "KISSmetrics = keep it simple silly" naming anecdote.
All dated 2017-11 → 2018-02.

## [2026-07-19] ingest | yt batch (@neilpatel, 8) — P1 long-form #3

Third real ingest batch. Stage machine (`.claude/commands/ingest-loop.md`, first-match)
selected **Stage B** (open P1 long-form rows exist). Not-taken rules: Stage S not due
(2 batches since synthesis, checkpoint at 10; no `>>> CHECKPOINT`, no channel/era
complete); Stage P not stale (2 batches since last synthesis/persona entry <10, no new
topic pages, P1 far from drained, and this is not the first loop run — batch #1 already
resolved the first-run persona clause); Stage A n/a (both TARGET channels enumerated).
Channel @neilpatel (Neil-fronted primary corpus, persona-first). Selection = clone's own
rule: priority-ascending then oldest-`published` first → next 8 oldest open P1 rows
(2018-04 → 2019-01).

Processed: **8 ingested (L2), 0 skipped, 0 no-captions, 0 dup.** All captions fetched
clean on the first try — no rate limiting (0 429s). Two rows flagged **★ L3-candidate**
for the next synthesis: `yt-dU4rWLHAcoo` (end-to-end automated-webinar $100K/mo digital-
product funnel with quantified benchmarks) and `yt-Q8rN3JKqUc8` (canonical start-to-finish
blog-post writing workflow). All 8 are solo Neil videos → fully Neil-attributed;
self-reported revenue/benchmark claims (e.g. "$100,000/month", ad-spend ROAS tiers) marked
as such in-page. Caption garbles caught and handled in-page (tool names verified, not
carried into paraphrase). No contradictions surfaced against existing pages.

Ledger after: L2=24, L3=0. Open long-form P1 @neilpatel 44, @MarketingSchoolPod 60
(104 total P1 remaining); P2 ~1,831; open shorts ~2,682. Ingest batches since last
synthesis: 3 (checkpoint at 10) — Stage S still 7 batches away.

Synthesis notes: two genuinely-new systems to promote at next Stage S — (1) **Automated-
webinar digital-product funnel** (`yt-dU4rWLHAcoo`, 2018-11-27): the most quantified
funnel Neil has laid out so far — ~3.6 sales per 100 registrations (split ~50/50
live-vs-followup-email), ~70% webinar show-up from short 15-minute recurring webinars,
Facebook-ad ROAS tiers ($2/$3/$5 return per $1), a $997 price anchored down from a $22K
value stack, and a named tool stack (WebinarJam, InfusionSoft, PlusThis, PicSnippets,
TurboDial). New paid-ads + email-marketing + agency-entrepreneurship material. (2) **Neil's
6 foundational free-tool stack + content-clustering rewrite workflow** (`yt-Uar2hXRrckY`,
2018-04-05): Google Analytics, Ubersuggest, Google Search Console, Crazy Egg, Subscribers,
HubSpot — plus a "one page per topic" anti-keyword-cannibalization consolidation/rewrite
tactic. Remaining six videos (100K-subs growth story, promoting a video with zero subs,
social-media beginner tips, 2019 predictions, 7 free SEO tools, blog-post workflow) mostly
reinforce already-captured YouTube-growth / SEO-tool / content-depth themes — fold in as
corroboration, not new spine. All dated 2018-04 → 2019-01.

## [2026-07-19] ingest | yt batch (@neilpatel, 8) — P1 long-form #4

Fourth real ingest batch. Stage machine (`.claude/commands/ingest-loop.md`, first-match)
selected **Stage B** (open P1 long-form rows exist). Not-taken rules: Stage S not due
(3 batches since synthesis, checkpoint at 10; no `>>> CHECKPOINT`, no channel/era
complete); Stage P not stale (3 batches since last synthesis/persona entry <10, no new
topic pages beyond the bootstrap hubs, P1 far from drained, and this is not the first loop
run); Stage A n/a (both TARGET channels enumerated). Channel @neilpatel (Neil-fronted
primary corpus, persona-first). Selection = clone's own rule: priority-ascending then
oldest-`published` first → next 8 oldest open P1 rows (2019-01-26 → 2019-07-22).

Processed: **8 ingested (L2), 0 skipped, 0 no-captions, 0 dup.** All captions fetched
clean on the first try — no rate limiting (0 429s). Four rows flagged **★ L3-candidate**
for the next synthesis: `yt-DoLzQN1m7sU` (start-a-digital-marketing-career framework),
`yt-zK4oTuiFV1E` (long-tail expansion workflow), `yt-JiqNIUQNQ7I` (WordPress SEO plugin
setup), `yt-MjO8lIQ68-8` (canonical no-pay backlink/skyscraper playbook). All 8 are solo
Neil videos → fully Neil-attributed; self-reported traffic/benchmark claims (e.g. "4M
visits/month", "90% of top sites have SSL", "30-40% share rate") marked as such in-page.
Caption garbles caught and handled in-page (WordPress plugin + tool names verified against
plausible real products; one "XE of Google" garble kept verbatim with a flag). No
contradictions surfaced against existing pages.

Ledger after: L2=32, L3=0. Open long-form P1 @neilpatel 36, @MarketingSchoolPod 60
(96 total P1 remaining); P2 ~1,831; open shorts ~2,682. Ingest batches since last
synthesis: 4 (checkpoint at 10) — Stage S still 6 batches away.

Synthesis notes: several genuinely-new tactical systems to promote at next Stage S —
(1) **Content-refresh playbook** (`yt-fGOv5oU5vww`, 2019-01-26): GSC → Ubersuggest
long-tail mining → rewrite the ranking page deeper (not keyword-stuff) → tighten
title/meta → link-out outreach; 9k→17k monthly-visitor case study on his digital-marketing
guide. (2) **Long-tail expansion workflow** (`yt-zK4oTuiFV1E`, 2019-06-10): Ubersuggest
Top Pages + GSC → Keyword Ideas report → rewrite existing ranking pages, ~30-day payoff —
tightly overlaps (1); fold both into one seo/ "expand what already ranks" concept.
(3) **Start-a-digital-marketing-career framework** (`yt-DoLzQN1m7sU`, 2019-04-22): DIY site
→ Ubersuggest competitor research → beat top pages → link/social outreach → email + push →
sell → A/B test, with a "high volume + high CPC + low difficulty" keyword-priority
heuristic and a ~7-visits-to-build-a-brand rule. (4) **No-pay backlink / skyscraper
outreach** (`yt-MjO8lIQ68-8`, 2019-07-15): find a competitor's linked pages → write a
demonstrably deeper article → custom (non-templated) outreach to their linkers; Neil names
content quality as the single most important step. New standalone data points worth a line
each: **90% of top-ranking sites have SSL** and **AMP gave little US mobile lift but a
large boost in weaker-infrastructure markets like Brazil** (`yt-JiqNIUQNQ7I`, 2019-07-04);
**~1% of first-time visitors return after 3 months / 30-40% share rate on featured-content
asks** (`yt-LdnWx49LUJc`, 2019-07-22). One dated/stale tactic to capture-but-flag:
**Facebook Messenger "blast" marketing via MobileMonkey** (`yt-3UNBH439N38`, 2019-04-13) —
auto-subscribe list + ask-for-like/comment, comments cited as the top FB algorithm signal;
tool and "free" status are 2019-specific. The eCommerce product-page CRO video
(`yt-GkOM7q9BYGQ`) restates Neil's standard benefit-led-copy/reviews/checkout playbook —
corroboration, not new spine. All dated 2019-01 → 2019-07.

## [2026-07-19] ingest | yt batch (@neilpatel, 8) — P1 long-form #5

Fifth real ingest batch. Stage machine (`.claude/commands/ingest-loop.md`, first-match)
selected **Stage B** (open P1 long-form rows exist). Not-taken rules: Stage S not due
(4 batches since last synthesis, checkpoint at 10; no `>>> CHECKPOINT`, no channel/era
complete); Stage P not stale (4 batches since last synthesis/persona entry <10, no new
topic pages beyond the bootstrap hubs, P1 far from drained, not the first loop run);
Stage A n/a (both TARGET channels enumerated). Channel @neilpatel (Neil-fronted primary
corpus, persona-first). Selection = clone's own rule: priority-ascending then
oldest-`published` first → next 8 oldest open P1 rows (2019-08-17 → 2020-04-16).

Processed: **8 ingested (L2), 0 skipped, 0 no-captions, 0 dup.** All captions fetched
clean on the first try — no rate limiting (0 429s). Three rows flagged **★ L3-candidate**
for the next synthesis: `yt-_ve9cmRaem0` (definitive Ubersuggest walkthrough — canonical
tool reference), `yt-wc_uo1prLg8` (the "how long does SEO take" 6-month traction rule —
his self-described most-asked question), `yt-S-hn2ThmQEw` (the corpus's FIRST substantive
paid-ads page — 7 Google Ads scaling hacks). All 8 are solo Neil videos → fully
Neil-attributed; self-reported benchmark claims (e.g. "47.6% more traffic on fresh vs
regurgitated content", "remarketing ~10x CTR", GetResponse "16% lift") marked as such
in-page. One caption garble caught (`yt-8KvyKt1c9ao`: "Gary Aviv" → Gary Vaynerchuk,
corrected only in paraphrase). The funnels/GetResponse video (`yt-p1ChsIfhu2Q`) carries a
`> ⚠️ CONTRADICTION:` callout in-page (clickbait "STOP building funnels" hook vs the body,
which insists every seller needs a funnel — the real message is stop stitching tools, not
stop funneling).

Ledger after: L2=40, L3=0. Open long-form P1 @neilpatel 28, @MarketingSchoolPod 60
(88 total P1 remaining); P2 ~1,831; open shorts ~2,682. Ingest batches since last
synthesis: 5 (checkpoint at 10) — Stage S still 5 batches away.

Synthesis notes: new tactical spine to promote at next Stage S — (1) **Ubersuggest master
workflow** (`yt-_ve9cmRaem0`, 2020-03-02): the full feature-by-feature tour (Keyword
Overview → Keyword/Content Ideas → Traffic Analyzer → Site Audit → Backlinks → Dashboard);
two reusable heuristics inside it — the Content Ideas → Skyscraper loop (sort competitors'
posts by shares/backlinks/traffic, mine their ranking keywords + link anchors, build
something "10x better") and the Site Audit prioritization rule (fixes ordered
highest-impact + easiest-first). This is the canonical Ubersuggest reference other tool
mentions should defer to. (2) **SEO-timeline position** (`yt-wc_uo1prLg8`, 2020-03-26):
the ~6-month "traction" rule with an explicit traction-vs-top-ranking distinction and a
long-tail-first path to early wins; data points 47.6% more traffic on fresh vs regurgitated
content and Forbes' 4–6-month figure — a durable persona belief worth its own seo/ page.
(3) **Paid-ads thesis, first entry** (`yt-S-hn2ThmQEw`, 2020-04-16): precision targeting
over broad reach — remarketing (~10x CTR), long-tail keywords, negative/exclusion lists,
location testing, ad extensions (+10–15% CTR), UTM tracking, competitor-keyword bidding;
establishes the paid-ads/ hub spine. (4) **6-step personal-brand framework**
(`yt-8KvyKt1c9ao`, 2019-09-28): single-channel-by-strength → document the journey →
research topics → engage commenters → podcast/interview tour → interview authorities to
borrow credibility; plus a bio datapoint — Neil states **LinkedIn is his highest-revenue
social platform** (attributed to his B2B focus). New standalone CRO primitives worth a line
each (`yt-hcPxMuxh5Tc`, 2019-09-02): the "8/10 read the headline, 2/10 read the body" ratio
and reframing CRO success as **completions, not clicks**; the underlying 7-part landing-page
anatomy (value-prop headline, single visual, benefits>features, one CTA, testimonials,
guarantee, storytelling) is direct-response canon — corroboration. Two smaller items:
**annual up-front billing as a growth-financing lever** (`yt-p1ChsIfhu2Q`, 2019-11-14 —
pull cash forward to reinvest in ad spend, not just churn reduction) and a **50% promotion
floor for detailed guides** (`yt-Y772PSqmudo`, 2019-08-17 — a deliberate exception to
Neil's usual 80/20 promote-vs-create rule; worth watching as a soft contradiction). The
free-courses roundup (`yt-SgDDfVCAkfk`, 2020-02-08) is a dated resource list — no new spine.
All dated 2019-08 → 2020-04.
