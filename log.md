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

## [2026-07-19] ingest | yt batch (@neilpatel, 8) — P1 long-form #6

Sixth @neilpatel P1 batch, 8 videos (2020-05 → 2020-10), all L2. Eight OK captions,
0 no-captions, 0 skipped, 0 dups, 0 yt-dlp failures (no rate-limiting). One subagent per
video wrote its own `wiki/sources/` page; coordinator did all ledger/index/log updates.
This batch is dominated by Neil's free "Unlocked" course franchise (SEO Unlocked, Instagram
Unlocked, YouTube Unlocked) plus two Ubersuggest Chrome-extension tutorials — all Neil solo,
so fully subject-attributed. Videos:
- `yt-Q_lySNxCag0` (2020-05-02) SEO Unlocked course intro ★ — transcript is ONLY the
  welcome/intro segment despite the "4+ HOURS" title (lessons previewed, not taught; noted
  in-page, no fabricated coverage).
- `yt-pIbQfOcsEsE` (2020-05-04) "The ONLY Video You Need To Understand SEO" ★ — SEO
  fundamentals primer (5 myths + core ranking factors).
- `yt-PXDPqXHLSOY` (2020-05-11) On-page & Technical SEO Part 1 (SEO Unlocked wk2) ★ —
  ~10-element on-page checklist + title/headline formulas.
- `yt-k04rHijEPSw` (2020-05-16) SEO site audit via Ubersuggest (On-page Part 3).
- `yt-eXBgXnKGTAw` (2020-06-20) & `yt-zHDATkRygTE` (2020-09-05) Ubersuggest Chrome extension
  (SERP keyword insights / SEO-traffic + backlink outreach) — both overlap the master
  Ubersuggest guide (`yt-_ve9cmRaem0`, 2020-03-02); kept as distinct feature-focused videos,
  NOT marked dup.
- `yt-eJ2NNy1F6y4` (2020-09-14) Instagram Unlocked welcome — low-signal framing, no tactics.
- `yt-BJhTePXFvGo` (2020-10-05) YouTube Unlocked M1 L1 — roadmap intro, framing.

Caption garbles caught & corrected in paraphrase only (quotes left verbatim): "adolf dassler"
→ Adolf "Adi" Dassler and "gary burrell" → Gary Burrell (Q_lySNxCag0); "nielpatel.com" →
neilpatel.com (k04rHijEPSw); Zuckerberg quote "Mozart grand era symphony" → "Mozart's grand
opera" (eJ2NNy1F6y4); "scores"→course, "account"→count (eJ2NNy1F6y4). No contradictions
flagged this batch. Several later course modules (SEO/Instagram/YouTube Unlocked) remain open
in the ledger for future batches.

Ledger after: L2=48, L3=0. Open long-form P1 @neilpatel 20, @MarketingSchoolPod 60
(80 total P1 remaining); P2 ~1,831; open shorts ~2,682. Ingest batches since last synthesis:
6 (checkpoint at 10) — Stage S ~4 batches away.

Synthesis notes: strong SEO teaching spine + persona/voice signals to promote at next Stage S —
(1) **SEO-mindset framework** (`yt-Q_lySNxCag0`): anticipate failure, delegate, keep learning,
ask for feedback, "give give give before you ask," know your "why"; plus the signature phrase
**"get loved by Google"** (recurs in `yt-eXBgXnKGTAw`) — both voice/persona-defining and L3
persona candidates; recurring self-cited numbers (6M+ monthly visits / 4M+ from search, "200+
ranking factors", team 100+) are persona-consistency anchors. (2) **SEO fundamentals scaffold**
(`yt-pIbQfOcsEsE`): the "Fact or Fiction" 5-myth intro + "SEO is a 24-hour salesman" metaphor +
core ranking-factor list; datable 2020 stats (93% of online experiences start with search;
31.7% CTR at position 1 per Advanced Web Ranking; 7% conversion drop per second of page-speed
delay per HubSpot). (3) **On-page formulas** (`yt-PXDPqXHLSOY`): title-tag formula (keyword-front
+ modifier-end; modifiers = buy/guide/review/online/offers/cheap/year), headline formula
(number/trigger → adjective → keyword → promise), the "8 of 10 read the headline, 2 of 10 click"
ratio + Ogilvy "80 cents of the dollar in the headline"; personal result — **removing dates from
neilpatel.com URLs boosted SEO traffic ~50% in ~30 days**. (4) **Site-audit error-prioritization
heuristic** (`yt-k04rHijEPSw`): fix critical errors → warnings → recommendations, biggest-bang +
easiest-first; 301-vs-302 / redirect-loop stance. (5) **Ubersuggest extension heuristics**
(`yt-eXBgXnKGTAw`, `yt-zHDATkRygTE`): no-click share as a traffic-potential filter, searcher
age-range as a commercial-intent proxy, domain-score 0–100 definition, and competitor-backlink
outreach as his favorite move — consolidate with the existing master Ubersuggest guide rather
than duplicating. Course-intro videos (`yt-eJ2NNy1F6y4`, `yt-BJhTePXFvGo`) are framing-only; the
one reusable signal is Neil's stated preference for **SEO-optimizing videos over relying on
YouTube's suggested engine** for consistent traffic. All dated 2020-05 → 2020-10.

## [2026-07-19] ingest | yt batch (@neilpatel, 8) — P1 long-form #7

Seventh @neilpatel P1 batch, 8 videos (2021-01 → 2022-06), all L2. Eight OK captions,
0 no-captions, 0 skipped, 0 dups, 0 yt-dlp failures (no rate-limiting). One subagent per
video wrote its own `wiki/sources/` page; coordinator did all ledger/index/log updates.
This batch broadens beyond the SEO/course spine into email, CRO/landing pages, the
Crazy Egg tool, an entrepreneurship how-to, an omnichannel future-of-marketing thesis, and
Instagram/backlink tactics — all Neil solo, fully subject-attributed. Videos:
- `yt-Gxd4NeKQg58` (2021-01-25) Email Marketing Unlocked — 0 to 50k subscribers (send-timing
  cadences, Semantics FM case study).
- `yt-SbJnXHfDJPg` (2021-02-25) 7 Landing Page Hacks Part 1 ★ — dense quantified-CRO playbook
  with per-tactic tested lift figures + named case studies.
- `yt-H_AUV7Iq2Ec` (2021-03-04) Turn Your Idea Into a Real Business ★ — 10-step idea→business
  guide carrying rich first-party Crazy Egg / QuickSprout origin detail.
- `yt-RVamsWm_TDg` (2021-05-01) How to Use Crazy Egg — CRO Unlocked (heatmap/scrollmap/confetti
  report walkthrough of his own former company's tool; taught as instructor, no ownership claim
  in-transcript — no contradiction flagged).
- `yt-g2AJYuOfBXI` (2021-06-28) The Future of Digital Marketing ★ — "five facts" omnichannel/CRO
  thesis talk; strongest persona/worldview signal of the batch.
- `yt-NT9pucaSoXw` (2022-03-31) Instagram Content Strategy 101 — 0 to 300k followers (partnerships,
  Reels).
- `yt-yUvEB7yiBFk` (2022-04-25) Easiest Way To Build Backlinks FAST (free-tool link magnet;
  Ubersuggest backlink-opportunity report).
- `yt-4JQnnxJ6zrw` (2022-06-16) Learn SEO in Just 5 Minutes a Day — signature habit-loop format,
  heavily self-promotional.

Caption garbles caught & corrected in paraphrase only (quotes left verbatim): "Uber-Suez" →
Ubersuggest and "Dodge Coin" → Dogecoin (`yt-H_AUV7Iq2Ec`). No contradictions flagged this batch
(the friction-as-conversion tactic in `yt-SbJnXHfDJPg` is noted as a conditional nuance vs. the
usual reduce-friction advice, not a hard contradiction — flag for reconciliation at synthesis).

Ledger after: L2=56, L3=0. Open long-form P1 @neilpatel 12, @MarketingSchoolPod 60
(72 total P1 remaining); P2 ~1,831; open shorts ~2,682. Ingest batches since last synthesis:
7 (checkpoint at 10) — Stage S ~3 batches away.

Synthesis notes: broad new tactical + persona spine to promote at next Stage S —
(1) **Quantified CRO/landing-page playbook** (`yt-SbJnXHfDJPg`, L3-candidate): engage-first
quizzes/sliders (+108%), GIF exit pop-ups, GeoIP targeting (+52.11%), checkout order bumps,
**friction-as-conversion** (qualifying hoops / Instant Checkmate roadblocks) — a counterintuitive
lever to reconcile against the usual reduce-friction rule; plus headline economics (odd numbers,
six-word / <65-char headlines, 8-of-10 read only the headline) and fear-based IP copy. Case
studies: Nutrition Secrets, Hello Bar, Instant Checkmate, Babbel, Expedia. (2) **Crazy Egg /
QuickSprout origin detail** (`yt-H_AUV7Iq2Ec`, L3-candidate — bio): Crazy Egg go-to-market
(prototype → user-feedback → marketers-vs-designers messaging pivot → CSS-gallery banner ads →
10,000+ pre-launch beta signups → 100,000 users; free-account seeding to TechCrunch/Mashable for
PR); the QuickSprout "100K challenge" (Nutrition Secrets fronted by friend "Mike", supplements +
Amazon, email list to lift Amazon fish-oil rankings; revenue-not-profit admission); "journey"
opt-in adapted from Groove HQ; self-reported ~7M (up to 9M) monthly visitors (2021); recurring
**"give nine, ask once"** value ratio and "YouTube fast time-to-view vs. Google slow-and-steady"
+ LinkedIn "ask for feedback, not a pitch" + "comments beat likes" reach heuristics. (3)
**Future-of-marketing thesis** (`yt-g2AJYuOfBXI`, L3-candidate — persona/worldview): the
**"traffic + conversions³ = success"** formula; "personalization is the new CRO"; Eric Schmidt
"brands sort out the cesspool" frame; "comments are the #1 virality signal"; the **Kissmetrics vs.
Mixpanel** proof-by-failure (out-trafficked ~3:1 yet valued ~1/15–1/20 of Mixpanel's $865M — origin
of his "traffic isn't everything" conviction); the "I see every side of the table" (paid by Google
& Facebook) authority frame; a dated ~12-month prediction worth later scoring. (4) **Email
send-timing heuristic** (`yt-Gxd4NeKQg58`): contrarian avoid-Tue/Wed/Thu, prefer Mon/Fri/Sun;
abandoned-cart 4h/16h/2d and nurture immediate/+2d/+4d cadences; Semantics FM case ($4.5M / 10
launches, 29% of revenue from email); "digital ATM" (John Reese) and "you don't need a fortune to
be fortunate" voice anchors. (5) **CRO scroll/engagement nuance** (`yt-RVamsWm_TDg`): engaged time
often peaks just below the fold → don't reflexively put CTAs above the fold. (6) **Link/social
nuggets**: "free tool as a link magnet" + white-label CodeCanyon tool ($10–30) and "link to three
competitors = not loyal, they'll link to you" (`yt-yUvEB7yiBFk`); staged Instagram partnership
evolution — reciprocal lives while small → one-way appearances once large, to avoid own-audience
live fatigue (`yt-NT9pucaSoXw`); the "5 minutes a day" habit-loop packaging + SEO-vs-ads cost
argument (`yt-4JQnnxJ6zrw`). All dated 2021-01 → 2022-06.

## [2026-07-19] ingest | yt batch (@neilpatel, 8) — P1 long-form #8

Eighth @neilpatel P1 batch, 8 videos (2022-08 → 2025-05), all L2. Eight OK captions,
0 no-captions, 0 skipped, 0 dups, 0 yt-dlp failures (no rate-limiting). One subagent per
video wrote its own `wiki/sources/` page; coordinator did all ledger/index/log updates.
This batch pushes the corpus into Neil's 2025 material — AI-era money-making, a full social
strategy, LinkedIn organic growth, plus two older business landmarks (the Answer The Public
acquisition and a Zero-to-$10M scaling talk). All Neil solo except the $10M talk, which is an
interview where Neil is the guest (host framing excluded from persona data). Videos:
- `yt-DhBeyS-C8VQ` (2022-08-06) Why we Acquired Answer the Public ★ — first-person acquisition
  origin story + "grow by acquisition, not only marketing" framework; freemium → premium and
  tool → agency funnel logic. New company facts: NP Digital "700+ employees globally"; Ubersuggest
  drives ~30% of NP Digital's agency customers.
- `yt-7mMFfJE8cEc` (2023-01-21) How I Built a Website to 4M Visitors/Month — long-tail keywords as
  the single lever; names an SMB division "NPD Accelerate"; long-tail ~2–3x faster than head terms.
- `yt-f9MnUdKVBHs` (2023-07-03) Taking Your Business From Zero to $10 Million — stage-by-stage
  scaling (TAM over niche, poach promoted-at-competitor hires, free-software → services funnel with
  the rationale that services markets are ~10x larger than software markets). Interview; Neil = guest.
- `yt-IaJKo9CxxXA` (2025-02-18) How to Get Rich in the New Era of A.I. — five AI-service business
  models (agents, translation, podcasts, infographics, websites) with a named tool stack (CrewAI,
  ElevenLabs, Opus, Piktochart-style, 10Web) and a "brain vs. body" models-vs-agents framing.
- `yt-6RNJpItArSQ` (2025-03-25) Learn Digital Marketing in 13 Minutes — beginner-to-expert roadmap
  (test on X → repost winners; Ubersuggest blogging + backlink outreach; Crazy Egg heatmaps/A-B;
  AI+humans; masterminds). Notable: KISSmetrics "Sign in with Google" +90% conversion, later
  dropped over privacy — a "what works now won't work forever" datapoint.
- `yt-E6ZSIZ89Ekg` (2025-04-01) How to Master Social Media in 2025 ★ — end-to-end social framework
  (algorithm/hook model → X as a penalty-free test bed → "search has moved to the social web"
  social-SEO → copy-the-mechanism remix → repurpose at scale → email-list backstop).
- `yt-ybttlXsLPXc` (2025-04-29) If I Wanted to Become a Millionaire in 12 Months ★ — canonical
  own-your-audience wealth blueprint; monetize 1% of traffic; visitor → email → recurring-revenue
  math; competitor-agnostic backlink outreach; Toyota+Ferrari multi-price-point monetization.
- `yt-zBlvV0W4bDc` (2025-05-23) The Best LinkedIn Growth Strategy For 2025 — "LinkedIn is starving
  for content" (9B weekly impressions, ~1% posting); reverse Dream 100 (connect with a target's
  network), hook → curiosity → question post structure, engage-before-you-post, "see more" as an
  explicit algorithmic signal.

Caption garbles caught & corrected in paraphrase only (quotes left verbatim): CrewAI / ElevenLabs /
Opus / Piktochart / 10Web / Grok / Crunchbase (`yt-IaJKo9CxxXA`); Ubersuggest, KISSmetrics, ChatGPT,
WYSIWYG (`yt-6RNJpItArSQ`); Cristiano Ronaldo, Adweek, neilpatel.com (`yt-ybttlXsLPXc`); Omnicom/WPP
and a garbled HubSpot revenue figure paraphrased to intent, no quote used (`yt-f9MnUdKVBHs`). No hard
contradictions flagged.

Ledger after: L2=64, L3=0. Open long-form P1 @neilpatel 4, @MarketingSchoolPod 60 (64 total P1
remaining); P2 ~1,831; open shorts ~2,682. Ingest batches since last synthesis: 8 (checkpoint at 10)
— Stage S ~2 batches away (P1 will fully drain on @neilpatel next batch, then move to
@MarketingSchoolPod P1 with attribution-gating).

Synthesis notes: strong 2025 + business-model spine to promote at next Stage S —
(1) **Acquisition-as-growth-channel** framework (`yt-DhBeyS-C8VQ`, L3-candidate) + the
**free-software → high-margin-services funnel** with the "services markets ~10x software markets"
rationale (`yt-f9MnUdKVBHs`) — a reusable business-model pattern that reframes the Ubersuggest /
Answer The Public / NP Accelerate giveaways as deliberate lead-capture, not just SEO plays.
(2) **X as a penalty-free testing bed** + "test on X → repost top 10–20% winners elsewhere" and
**"search has moved to the social web"** social-SEO thesis with split figures (`yt-E6ZSIZ89Ekg`,
`yt-6RNJpItArSQ`; L3-candidate) — extends the long-tail/AnswerThePublic keyword doctrine onto social.
(3) **Own-your-audience millionaire model** (`yt-ybttlXsLPXc`, L3-candidate): 1M visitors × 1% ×
$30/mo math (arithmetic is aspirational/garbled — paraphrased faithfully, not endorsed),
competitor-agnostic backlink outreach, Toyota+Ferrari price-laddering.
(4) **AI-service business models + endorsed 2025 tool stack** (`yt-IaJKo9CxxXA`): CrewAI, ElevenLabs,
Opus, Piktochart-style, 10Web; "brain vs. body" models-vs-agents framing — new ai-marketing material.
(5) **New entity + company facts** for entities pages: Answer The Public (acquisition origin source),
NP Digital "700+ employees", Ubersuggest → ~30% of agency customers, NPD Accelerate SMB division.
(6) Persona-scale markers (2025): Neil now claims 1M+ followers per network. All dated 2022-08 → 2025-05.
