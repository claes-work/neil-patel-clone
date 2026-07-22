# Synthesis state

_Tracks the synthesis **high-water mark** so the synthesis loop never misses material and never
re-does work. Companion to the ingest ledger (`ledger.csv`). The detailed debt lives in `log.md`
as `Synthesis notes:` lines (every ingest batch appends one). See `tools/SYNTHESIS.md` for the loop
and `tools/synthesis_batch.py` for the driver._

## High-water mark
Synthesized through: **@neilpatel 2023-06 → 2023-12 P2 tactical + co-hosted era complete — all 1,156 L2 sources, ingest batches #1–#147 (2016-11 → 2023-12/2025-05)**, via synthesis pass 15 (2026-07-22). The mark did NOT advance at pass 16 (2026-07-22, no-op checkpoint — see below): batches #148–#156 (log cont. 117–126) ingested **zero** new L2 sources — every one of those ten batches hit the environment-wide yt-dlp PO-token caption-fetch gap (confirmed via direct `--list-subs` diagnostics at cont. 125/126) and was auto-marked `no-captions` by the driver. There is no new L2 material to promote; the mark stays at batch #147 until real ingest resumes. **Operator action needed**: install a PO-token provider plugin (e.g. `bgutil-ytdlp-pot-provider`) or configure `--cookies-from-browser` for `tools/ingest_batch.py`'s yt-dlp invocation — until then, further ingest batches on either channel (and all 2,688 open shorts) are expected to keep yielding zero new sources.

## Pending checkpoints
_(oldest first; the synthesis loop drains these top-down)_
_(none — caught up through batch #147; @neilpatel 2023-06→2023-12 P2 tactical + co-hosted era fully synthesized; the #148–#156 debt was a no-op, see pass 16 below)_

## Done checkpoints
- [x] 2026-07-22 — **synthesis pass 16 (no-op checkpoint)** — triggered by the 10-ingest-batch debt
  counter (batches #148–#156 / log cont. 117–126) reaching the checkpoint threshold, per
  `tools/ingest_batch.py status`'s `SYNTHESIS DUE` flag. Ran `python tools/synthesis_batch.py
  status`/`prepare` and cross-checked the 10 `Synthesis notes:` lines in `log.md` (cont. 117–126):
  all ten read "Synthesis notes: none (nothing ingested this batch)" — every batch in the window
  was 0/8 captions fetched, auto-marked `no-captions` by the driver, root-caused (cont. 120, 125,
  126) to an environment-wide yt-dlp PO-token caption-fetch gap, not a real absence of captions.
  **Zero new L2 sources exist since pass 15 (still 1,156 total, batch #147)** — nothing to promote
  into `wiki/topics/` or `persona/`; no topic/persona file touched; `persona/system-prompt.md` NOT
  recompiled (unchanged, still v16 / compiled_from_sources 1156 from pass 15). This entry exists
  purely to log the checkpoint bookkeeping and reset the ingest loop's
  debt counter (`tools/ingest_batch.py`'s `batches_since_synthesis()` resets on any log line
  containing "synthesis") so the next iterations don't re-flag `SYNTHESIS DUE` on zero-yield
  batches. High-water mark unchanged (still batch #147). **Recommend an operator session fix the
  yt-dlp PO-token gap before further ingest dispatches** — see the high-water mark note above and
  the repeated flags at log.md cont. 120–126.
- [x] 2026-07-22 — **synthesis pass 15** — @neilpatel 2023-06 → 2023-12 P2 tactical + co-hosted era
  complete (1,156 L2 sources total, batches #138–#147 / log cont. 107–116, 2023-06-24→2023-12-07 run
  plus one empty batch, cont. 116, 8/8 no-captions). Drained the 10 accumulated `Synthesis notes:`
  lines. Promotions (quality-over-volume; pure repeats/reinforcements dropped): **seo** (the
  five-factor Google ranking framework — brand/content/backlinks/code/time — from a 900M-domain
  analysis ★; a black-hat LinkedIn comment-seeding tactic (playerup.com), explicitly self-disclaimed,
  plus a white-hat engagement-pod counterpart ★; the quarterly money-page-refresh rule + a
  three-part growth-strategy list — free tools / buy underutilized traffic (AnswerThePublic $8.6M) /
  buy a defunct competitor's domain (a ~$500K personal offer for the KISSmetrics domain) ★),
  **social-media** (per-platform first-hours growth mechanics from the same 900M-domain/900-page
  analysis ★; the same black-hat LinkedIn disclosure cross-linked; Nike/Disney/Timberland
  true-omnichannel examples + the Ryan Reynolds/MNTN equity-influencer case; the Threads-vs-Twitter
  8.3x engagement experiment ★), **agency-entrepreneurship** (NP Digital's international-expansion
  detail — 74% YoY growth, a Germany-division closure, eight new regions in ~5 months ★; a
  going-private rationale — "I'm not a CEO, I would be a terrible CEO," patient-capital-only ★; the
  NP Digital naming origin — a year-and-a-half domain-acquisition delay; a wealth-as-investment
  philosophy + explicit remote-first company policy ★; the candid Hustle/NYT-bestseller-list
  mechanics (Result Source, corporate bulk pre-orders) + a paid-speaking-fee trajectory ($5-10K →
  $50-100K/talk → "fishing with dynamite" free-speaking pivot) ★; the course-selling walk-away
  ($600K/mo peak, the Mike Kamo free-call anecdote) ★; an agency-acquisition diligence checklist
  ("kiss a lot of frogs," 4-year retention bar) ★; a refund-policy brand-protection value
  ("penny-wise, pound-foolish") ★; a virtual-summit case study — 20-30K registrants, an enterprise
  speaker roster ★; the Mexico M&A anecdote — "you can't trade on potential" ★). **No genuinely new
  material this run for content-marketing, paid-ads, analytics-cro, email-marketing, or
  ai-marketing** — the "Where's Waldo" AI-content-sameness metaphor and the "Project Magi" prediction
  both recurred without new substance; a companion gray-area tool (retention.com) disclosed in the
  same segment as the LinkedIn tactic was excluded as **Eric Siu's material, not Neil's**. **New
  unreconciled variant flagged (not a hard contradiction):** a third, different self-reported
  AnswerThePublic acquisition date — "February, 2022" — surfaces alongside the registry-verified
  2022-05-31 close and the previously-flagged "Feb 2023" self-reports, now three distinct dates on
  record ([[../wiki/entities/np-digital|entities/np-digital]]); the existing 11x-vs-8x Mexico-M&A
  figure variant and the Seattle residency discrepancy (given further, still-unresolved texture via
  a follow/unfollow-bot anecdote) are both carried forward, not smoothed. Persona: **beliefs.md**
  (109→115 sources; the going-private rationale, wealth-as-investment philosophy, luxury-purchases-
  diminishing-returns, true-omnichannel-vs-multichannel + Nike/Disney/Ryan-Reynolds-MNTN, the
  refund/brand-protection value, the Mexico M&A discipline anecdote, a family-over-money values
  statement), **voice.md** (82→90 sources; "That was actually my biggest mistake in my life," "I'm
  not a CEO, I would be a terrible CEO," "You can't trade on potential," "you got to kiss a lot of
  frogs," "penny-wise, pound-foolish," "I don't believe money is everything in this world," the NYT-
  bestseller-mechanics candor quote, a rare on-mic family interruption), **biography.md** (87→94
  sources; the irrevocable-trust/inheritance disclosure, the Beverly Hills house + Patek
  Philippe/Maybach diminishing-returns disclosure, the early-Airbnb $240K cold-call contract, the
  candid Hustle/NYT-bestseller mechanics + speaking-fee trajectory, the three-part growth-strategy
  list, a family recording-interruption confirmation, the Seattle follow-bot anecdote), **appearance.md**
  unchanged (7 sources; no new appearance material this run). Recompiled **system-prompt.md v15 → v16**
  (compiled_from_sources 1,089 → 1,156): wove in the going-private/"terrible CEO" self-framing, the
  wealth-as-investment philosophy paired with the irrevocable-trust regret, the true-omnichannel-vs-
  multichannel differentiation belief, the refund-policy brand-protection value, the Mexico M&A
  anecdote + agency-acquisition diligence checklist, the NP Digital naming origin, the course-selling
  walk-away, the $50K speaking-fee update, the early-Airbnb $240K contract, the Threads 8.3x
  experiment, and the family-over-money values statement; kept the five-factor ranking framework,
  the black-hat LinkedIn disclosure, the international-expansion detail, and the client case studies
  topic-hub-only per the changelog. `index.md` updated (topic-hub summaries, entity list, persona
  summaries, header). `pipeline/synthesis-state.md` high-water mark advanced to batch #147 / 1,156
  L2 sources; no pending checkpoints remain.
- [x] 2026-07-22 — **synthesis pass 14** — @neilpatel 2022-12 → 2023-06 P2 tactical era complete
  (1,089 L2 sources total, batches #128–#137 / log cont. 106, 2022-12-15→2023-06-22 solo run; fully
  Neil-attributed, a run unusually dense with guest-interview financial/family disclosure). Drained
  the 10 accumulated `Synthesis notes:` lines. Promotions (quality-over-volume; pure repeats/
  reinforcements dropped): **agency-entrepreneurship** (the KISSmetrics $1,250,391 value-proposition
  mistake ★; the India Q&A operating philosophy — "110%" presence, a values triad, "player-coach"
  hiring ★; a GM-firing Crazy Egg origin variant + the AnswerThePublic economics + PE/IPO-decline
  independence value ★; the personal-brand naming story sharpened; the uncle's leveling-mantra
  origin attributed for the first time; a cold-calling monetization variant; the FTX consulting
  relationship confirmed in Neil's own words ★; the KISSmetrics FTC investigation + AnswerThePublic
  "overpay" confirmed ★; the MBE certification tiebreaker + $120-180K/mo personal burn-rate
  breakdown ★; the never-CEO-himself pattern + no-money-to-kids philanthropy stance, two named
  programs ★; the "forget personal brand, hire operators" tension ★; the most granular
  AnswerThePublic economics + VC-declined/bank-AR-financing history ★; the First Republic Bank
  day-trade + mentor "John" + no-private-jet minimalism ★; real-estate-as-personal-residence-mistake
  + the Crazy Egg 2008-crisis attribution sharpened; the Brazil-expansion origin story + Mike
  Gullickson's fuller career history ★; the richest biographical/family disclosure to date
  (marriage, kids, "7,8,9" declined offers) ★; the WealthCon keynote + $515M acquisition offer ★;
  the fullest teen-founder origin account ★; the "riches are in the niches" → "big massive markets"
  belief reversal ★), **seo** (the Amazon "A10" algorithm named explicitly; a "4,500 algorithm
  changes in 2020" stat + YoY Search Console refresh workflow; the content-simplicity philosophy
  sharpened — "write for a kindergartner"), **content-marketing** (the hedgehog concept named ★; a
  ranked TAM-based niche-selection doctrine; the WealthCon 10-hack content/personal-brand keynote ★;
  the content-production pipeline named; the Gary Vaynerchuk content-repurposing credit reinforced),
  **social-media** (the email-as-social-growth-lever tactic; an Instagram-over-Facebook prediction;
  LinkedIn confirmed as NP Digital's #2 revenue channel after YouTube; a celebrity-endorsement
  alignment thesis — Ryan Reynolds/Mint Mobile, LeBron/Tonal vs. generic deals; TikTok cost-
  efficiency vs. Facebook), **email-marketing** (the email-deliverability "taint" mechanism +
  QuickSprout origin anecdote; SMS-over-email revenue preference + PayPal ~18% lift), **analytics-
  cro** (the Dave Brailsford "marginal gains" analogy + an own-vs-cited-data contrast; the Walmart
  Labs hyper-personalization pushback; a PayPal-checkout ~18% revenue lift), **paid-ads** (a
  carousel-ads engagement-rate stat bank; TikTok's ~40-50%-cheaper cost-efficiency vs. Facebook),
  **ai-marketing** (E-A-T + "Where's Waldo" AI-content-commoditization metaphor + the "Project Magi"
  prediction ★; a 5-year no-AI-replacement forecast reasoned from data quality ★; a "Success with
  Soul" AI/E-E-A-T skepticism demo; two near-term AI-disruption points named). **New CONTRADICTION
  flagged, not reconciled:** a self-reported-vs-registry-verified AnswerThePublic acquisition-date
  discrepancy ("February 2023" self-reported vs. the registry-verified 2022-05-31 close, also
  refining SUBJECT.md's "acquired 2022" note) — flagged on [[../wiki/entities/np-digital|
  entities/np-digital]]. Also carried, not smoothed: a third Crazy Egg origin variant (fired from a
  GM ad-spend account) alongside the existing two tellings ([[../wiki/entities/crazy-egg|
  entities/crazy-egg]]); a further Mike Gullickson career-history variant, still not fully
  reconciled ([[../wiki/entities/mike-gullickson|entities/mike-gullickson]]); a sister-name spelling
  variant ("Amy" vs. "Amee"); and a minor self-reported age inconsistency (37 vs. "38 now," within
  the same two weeks). Persona: **beliefs.md** (98→109 sources; the "110%" presence philosophy, the
  TAM-ranked niche doctrine, the hedgehog concept, the "riches are in the niches" reversal,
  "software is a race to the bottom," the independence-over-a-sale value, the "forget personal
  brand, hire operators" tension, the never-CEO/no-money-to-kids philanthropy stance, the personal-
  residence wealth-philosophy carve-out, a 5-year no-AI-replacement forecast), **voice.md**
  (71→82 sources; "I think of life as whatever you do, put in 110%", the hedgehog "meaningfully
  reach a hundred people" line, "I don't care for the money... building a bigger business", "I'm a
  terrible leader, I really am", "software is a race to the bottom", "forget personal brand, I would
  just go hire people", the "riches are in the niches" reversal quote, the uncle's leveling-mantra
  quote), **biography.md** (76→87 sources; the uncle's mantra origin, a cold-calling monetization
  variant, the fullest teen-founder origin account, the First Republic Bank day-trade + mentor
  "John", the richest family disclosure to date), **appearance.md** unchanged (7 sources; no new
  appearance material this run). Recompiled **system-prompt.md v14 → v15** (compiled_from_sources
  1,010 → 1,089): wove in the "110%"-presence philosophy + values triad, the TAM-ranked niche
  doctrine + "riches are in big markets" reversal, the hedgehog concept, "software is a race to the
  bottom," the independence-over-a-sale value (declined $515M offer), the never-CEO/no-money-to-kids
  philanthropy stance, the "forget personal brand, hire operators" tension, the personal-residence
  wealth carve-out, the 5-year no-AI-replacement forecast, E-A-T + "Where's Waldo," and the richest
  family/teen-founder biographical material; kept the remaining tactical/framework material
  topic-hub-only per the changelog. `index.md` updated (topic-hub summaries, entity list, persona
  summaries, header). `pipeline/synthesis-state.md` high-water mark advanced to batch #137 / 1,089
  L2 sources; no pending checkpoints remain.
- [x] 2026-07-21 — **synthesis pass 13** — @neilpatel 2022-06 → 2022-12 P2 tactical era complete
  (1,010 L2 sources total, batches #118–#127 / log cont. 96–105, 2022-06-04→2022-12-12 solo run;
  fully Neil-attributed solo tactical/case-study content). Drained the 10 accumulated `Synthesis
  notes:` lines. Promotions (quality-over-volume; pure repeats/reinforcements dropped): **seo**
  ("Battlefield Bypass" black-hat retelling named + quantified ★; the "almost ranking" Search
  Console tactic + Ubersuggest AI writer ★; a CTR-lift stat block for titles/meta descriptions,
  cross-linked as one dataset; international-SEO (hreflang, Nike brand-query example) and
  Amazon-SEO as distinct sub-verticals; the buy-and-301-merge acquisition tactic + YouTube
  first-24-hours engineered spike ★; "vet the people" reinforced + a Media Post award citation),
  **agency-entrepreneurship** (the freemium-to-services business model named explicitly ★
  — Ubersuggest-as-loss-leader vs. HubSpot-vs-Dentsu/WPP/Omnicom; the immigrant-mother origin
  story elaborated with a free-preschool-attendance clause ★; a three-point, dated
  speaking-for-free belief-evolution arc (2019→2022→2026) ★; the Crunchbase-teardown playbook
  extended with an up-to-$20M ceiling + 1-in-4-5 conversion rate; LinkedIn talent-poaching
  outreach tactic; a personal philanthropy/donate-not-inherit statement ★; the quantified 2022
  content-production system ★ cross-linked from content-marketing; new webinar co-hosting
  partners (BigCommerce, WP Engine) + a five-touch reminder cadence), **content-marketing** (the
  quantified 2022 content-production system ★, the audience-to-owned-product model (Kylie
  Jenner/Gary Vaynerchuk), the 2017 YouTube-channel-launch origin story), **social-media** ("Why I
  Focus on Social Media Marketing Over SEO" channel-prioritization philosophy ★, the LinkedIn
  low-competition-content thesis, Position-Based attribution as his stated personal practice),
  **email-marketing** (email-vs-SMS engagement figures, browser push notifications as a distinct
  channel, a staged SMS discount drip sequence), **analytics-cro** (Position-Based attribution),
  **ai-marketing** (an early, explicitly human-in-the-loop AI-adoption stance dated to December
  2022 ★, predating the 2025-26 GEO/AEO material by ~2 years). **paid-ads: no genuinely new
  material this run** (the 32%-more-backlinks and email-vs-SMS figures from the same source went
  to seo/email-marketing instead). **No new hard contradictions flagged this pass** — carried, not
  reconciled: a CTR-stat overlap between two Ubersuggest-derived sources (cross-linked, not
  double-counted, per the source pages' own flag) and a Mike Gullickson name-spelling variant
  ("Gullaksen") with a new $325M iCrossing/Hearst sale-price detail not in the earlier telling
  ([[../wiki/entities/mike-gullickson]]). Persona: **beliefs.md** (93→98 sources; the
  business-is-a-sport/donate-not-inherit philanthropy stance, the freemium-to-services thesis
  named explicitly, the social-vs-SEO channel-prioritization philosophy, the speaking-for-free
  2019→2022→2026 arc, the AI-adoption-since-2022 stance), **voice.md** (66→71 sources; "it's...a
  sport, and I just have to hit a number", "what worked for Google, didn't really work for
  YouTube", "there's more money in marketing services than there is in marketing software",
  "you're not just looking for coaches, you're looking for players", "adapt it to your life", "I'm
  not an expert in any of those topics"), **biography.md** (70→76 sources; the philanthropy/
  donate-not-inherit statement, the granular 2022 daily routine — 700+ employees/900+ clients
  marker, script-writing habit, wife's "10 minutes" line, kids no-phone playtime — the immigrant-
  mother origin elaborated, the expertise-vs-hustle cautionary anecdote, the fuller "Battlefield
  Bypass" black-hat retelling), **appearance.md** (6→7 sources; a variant intermittent-fasting
  eating window — first meal at noon vs. the existing 11am-6pm window — recorded as a variant to
  reconcile, not a contradiction). Recompiled **system-prompt.md v13 → v14**
  (compiled_from_sources 932 → 1,010). System-prompt version at pass end: **v14**.
- [x] 2026-07-21 — **synthesis pass 12** — @neilpatel 2021-11 → 2022-06 P2 tactical era complete (932
  L2 sources total, batches #108–#117 / log cont. 86–95, 2021-11-22→2022-06-02 solo run; fully
  Neil-attributed solo tactical/case-study content). Drained the 10 accumulated `Synthesis notes:`
  lines. Promotions (quality-over-volume; pure repeats/reinforcements dropped): **seo** ("Google
  trusts brands" ranking rationale + 6-7-person content-refresh team; who-NOT-to-compete-with 3-tier
  framework; CTR-over-backlinks reranking claim + optimize-vs-create decision rule; the fullest
  competitor-research tool roster in the corpus ★), **paid-ads** (cross-channel competitor-research
  tool roster ★ — SpyFu/BigSpy/Not Just Analytics/Sociality.io/Facebook Ad Library named favorite;
  the $500,000 TV-ad legitimacy case study ★ — ~640 employees, Inc. 500 #21, weak ROI but
  RFP-inclusion effect), **content-marketing** (~140-pieces/mo cross-platform content cadence ★ +
  English-only/team-translation disclosure; the "boring product" 5-tip framework — narrative,
  anchor-to-needs, visual, humor, status-elevation), **social-media** (Instagram 0→290K
  partnership-growth framework ★ — ~8% cold-outreach hit-rate, staged peer→bigger-account→
  reciprocal-shoutout sequence; TikTok-delegation surprise story + 0→30K-in-6mo growth; 5am-vs-6pm
  posting-time data point + QVC/home-shopping analogy; YouTube first-24-hours virality mechanic +
  yes/no-vs-open-ended comment self-correction), **ai-marketing** (a repeated, dated "saves ~half
  the time... not perfect" AI-writing-tool self-assessment), **agency-entrepreneurship** (new entity
  [[../wiki/entities/mike-gullickson|Mike Gullickson]], NP Digital CEO; the hiring-twice heuristic
  "once could always be luck, twice means they're usually good," recurring 3x; two complete teachable
  frameworks ★ — The 6 Stages of Learning Digital Marketing, How to Start a Digital Marketing Agency
  From Scratch; NP Digital $5K/mo sales-tool ROI case; "vet the people, not the agency's brand name"
  hiring stance + a $100M-raised goal-misalignment anecdote ★; the RIYA Crunchbase-teardown
  cold-outreach case ★ + its new "doesn't work above ~$100M raised" funding ceiling). **New
  CONTRADICTION flagged, not reconciled:** a 2022-04-21 self-report of an Obama-era "top 30
  entrepreneurs under 30" nomination, differing from the "top-100" framing recorded elsewhere in the
  corpus and in SUBJECT.md — both self-reported/unaudited, kept side by side
  ([[../wiki/sources/2022-04-21-yt-pwDSUP6zGeQ]]). Also carried, not smoothed: an Ubersuggest
  customer-share discrepancy ("40%+" vs. an existing "~30%" marker) and two further self-reported
  traffic-figure variants (~2.2M/mo, ~2M/mo). Persona: **beliefs.md** (88→93 sources; the hiring-twice
  heuristic, "vet the people not the brand" + goal-alignment discipline, the storytelling-is-practiced
  method, the YouTube yes/no-vs-open-ended self-correction), **voice.md** (61→66 sources; "it's not
  about your solution, it's about how it makes your customer's lives better," the grandmother
  anecdote, "I got a TikTok?", the QVC anecdote, "I don't have a fancy car, I drive a Honda Odyssey,"
  "the loudest person in the room is the weakest," "once could always be luck, twice means they're
  usually good"), **biography.md** (60→70 sources; own-YouTube-channel growth history — failed
  paid-ads phase vs. daily-upload-phase success — TikTok-delegation surprise story, "really only"
  speaks English, John Reese early-20s-mentee detail + age-37 self-report, NP Digital 500+/640-
  employee 2022 markers, Obama contradiction + traffic-figure reconciliation flags), **appearance.md**
  (4→6 sources; the Honda Odyssey anti-flashy detail + driving-anxiety aside). Recompiled
  **system-prompt.md v12 → v13** (compiled_from_sources 853 → 932). System-prompt version at pass
  end: **v13**.
- [x] 2026-07-21 — **synthesis pass 11** — @neilpatel 2021-05 → 2021-11 P2 tactical era complete (853
  L2 sources total, batches #98–#107 / log cont. 76–85, 2021-05-15→2021-11-20 solo run; fully
  Neil-attributed — a dense stretch of biography-rich guest interviews, several with title/date
  mismatches, plus routine solo tactical content). Drained the 10 accumulated `Synthesis notes:`
  lines. Promotions (quality-over-volume; pure repeats/reinforcements dropped): **agency-
  entrepreneurship** (the key-man-syndrome-reasoned NP Digital rename origin ★ + ACS agency/2008
  crisis; the "Who is Neil Patel?" campaign retold unapologetically, quantified, + bodybuilder-pecs
  execution detail; the discontinued **Advanced Marketing Program**/info-product business ★, ~$600K/
  mo peak / $371,882/mo average, full 7-step funnel; MicroAcquire+Capchase no-money-down acquisition
  play; NP Digital declined financing offers + eat-the-cost-of-my-team's-mistake anecdote; the
  Crunchbase-teardown cold-outreach playbook extended (investor-CC, CEO-to-CMO); a third KISSmetrics-
  vs-Mixpanel dollar-figure variant), **seo** (RankBrain named explicitly; the SEO-vs-SEO-company 6x
  ROI case study; the Ubersuggest "page one ranking potential" tool feature; the ~3x-backlinks
  data-driven-content stat tied to E-A-T), **analytics-cro** (the two-step-checkout +8-11% figure;
  the Portent load-time stat; the info-product 7-step funnel with revenue figures ★; the scarcity-
  honesty ethical line + "common enemy" trigger; the logic+emotion copy-combination finding),
  **social-media** (comments-not-duration algorithm doctrine + LinkedIn>TikTok>YouTube>Google
  platform-priority ranking; the hair-extensions livestream-frequency case study; live-video-as-
  algorithmic-lever doctrine; Eric-Siu-as-benchmarked-peer + consistency-over-quality growth
  attribution), **content-marketing** (the "content blindness" thesis; neilpatel.com's explicitly
  ordered topical-expansion sequence; the Marketing School format backstory; HARO named explicitly;
  the writer-vs-marketer premium-pricing distinction), **email-marketing** (Frank Kern credited for
  "the money's in the list" — a second, conflicting attribution vs. the existing John Reese credit;
  a tighter 90-95/5-10 give/sell ratio), **paid-ads** (the toothbrush-parenting anecdote + India
  SMS-cost/Jio case; the non-Google/FB platform ROI ranking + $1.5-2M/mo avoided-ad-spend figure;
  73% mobile-commerce share), **ai-marketing** (the first AI-tool-*usage* claim — Jarvis — bridging
  the 2020 forecast and the 2023 GEO era ★; the extended AI-content-tool roster + three-stage
  Ubersuggest automation roadmap ★; the "writing is a zen moment, like ironing" personal-habit
  counterpoint to his own AI advocacy). Persona: **beliefs.md** (83→88 sources; the contentment-
  over-happiness belief-evolution flagged alongside the 2018 "success is happiness" framing, paired
  with "I just like winning" and the Bill Gates admiration; the key-man-syndrome reasoning extending
  corporate-brand-over-personal-brand; a 2021 financing-decline precedent extending capital
  discipline), **voice.md** (57→61 sources; "sales is like dating," "writing is a zen moment... like
  ironing," "I just like winning," the ketchup-stains self-presentation quote, the Frank Kern/John
  Reese conflicting-attribution note), **biography.md** (51→60 sources; mother's home-daycare
  referral network, father's savings-match reversal, AOL-hacking-at-12, the ACS agency/2008
  financial crisis, the job-board dated ~2001, a third KISSmetrics/Mixpanel dollar figure, the
  bodybuilder-pecs "Who is Neil Patel" detail, daily-routine + age-35 self-report, the Restream/Eric
  Siu livestreaming-adoption story + introvert self-disclosure, a second "lie to a client"
  confession, "I live in my wife's house"), **appearance.md** (2→4 sources; the first fitness/diet
  routine in the corpus — Body Coach HIIT, intermittent fasting, food avoidances — plus the
  gym-shorts/ketchup-stains self-presentation quote). Recompiled **system-prompt.md v11 → v12**
  (compiled_from_sources 773 → 853). **No new hard contradictions; two unreconciled variants
  carried:** a third self-reported KISSmetrics-vs-Mixpanel dollar figure ("over 50 plus million"),
  and a second, conflicting named credit for the "list is an ATM machine" line (John Reese vs. Frank
  Kern). System-prompt version at pass end: **v12**.
- [x] 2026-07-21 — **synthesis pass 10** — @neilpatel 2020-10 → 2021-05 P2 tactical era complete (773
  L2 sources total, batches #88–#97 / log cont. 66–75, 2020-10-24→2021-05-13 solo run; fully
  Neil-attributed). Drained the 10 accumulated `Synthesis notes:` lines. Five named courses launch
  and complete end-to-end within this run — **LinkedIn Unlocked**, **Facebook Unlocked**, **Local SEO
  Unlocked**, **Email Marketing Unlocked**, **CRO Unlocked** — plus **Growth Hacking Unlocked**
  launches. Promotions (quality-over-volume; pure repeats/reinforcements dropped): **social-media**
  (LinkedIn Unlocked's five-stage B2B sales-cycle framework + 80/20 Groups rule + 8-12-day webinar
  countdown framework ★; Facebook Unlocked's News-Feed-algorithm mechanism + five-rules brand-growth
  framework ★ + two-ad blog-then-retarget funnel; the Messenger-decline → push-notification pivot;
  the Gary Vaynerchuk style-contrast quote), **seo** (Local SEO Unlocked's full playbook ★ — proximity/
  relevance/prominence triad, local-reviews-matter-more thesis, Google Guarantee; the EMD
  CTR-suppression mechanism; the Wikipedia/Clutch content-gap tactic; the first-24-hours-promotion-
  drives-YouTube-ranking mechanism ★; the sitewide cornerstone-sidebar linking hack; the free-tool-
  over-content GSC figures), **content-marketing** (the quiz-funnel design ruleset ★ — 714K emails;
  the three-part blog-homepage template; the 10/40/20/30 content-time allocation; the question-
  keyword-content generalization), **email-marketing** (Email Marketing Unlocked's full course ★ —
  Exit-Intent/social-login lift figures, the 98/2 educational ratio, the four-non-opens suppression
  rule, the 760%-segmentation stat), **analytics-cro** (CRO Unlocked's full course ★ — the
  traffic×conversion formula, the Skincare-by-Alana/Atlanta case studies, the first appearance of
  Porter's Five Forces/PEST/SWOT ★, the Bezos/Zuckerberg iteration quotes), **paid-ads** (Gmail-inbox-
  ads email retargeting; the SaaS pricing-page A/B results + Spiralize competitor-agency
  recommendation), **agency-entrepreneurship** (the Bucharest origin-story interview ★ — job-board-at-
  16 reframing, "be great at one thing," SWOT sales technique, micro-commitments framework; the
  KISSmetrics $16.4M/seven-rounds fundraising history ★ + True Ventures rejected-then-invested
  anecdote ★; Growth Hacking Unlocked's "learn from other founders" doctrine ★; the 6-10x-revenue-at-
  breakeven SaaS exit claim). **New CONTRADICTION flagged, not reconciled:** two sources in this batch
  ([[../wiki/sources/2021-04-26-yt-E_CyyiRXH0U]], [[../wiki/sources/2021-05-13-yt-Ol2kGMDvX4o]]) name
  Neil's **brother-in-law** as the Crazy Egg co-founder/current full owner, in tension with the
  well-documented Hiten Shah co-founder narrative — flagged on both `wiki/entities/` pages
  ([[../wiki/entities/crazy-egg]], [[../wiki/entities/hiten-shah]]) and on `persona/biography.md`.
  Persona: **beliefs.md** (81→83 sources; "learn from other founders" doctrine, "be great at one
  thing, outsource the rest"), **voice.md** (55→57 sources; the Gary Vee style-contrast quote, "I'm
  not the smartest person out there," "a no just means not right now"), **biography.md** (49→51
  sources; the Bucharest origin-story reframing, KISSmetrics fundraising detail, the Crazy Egg
  co-founder CONTRADICTION). Recompiled **system-prompt.md v10 → v11** (compiled_from_sources 693 →
  773). System-prompt version at pass end: **v11**.
- [x] 2026-07-21 — **synthesis pass 9** — @neilpatel 2020-03 → 2020-10 P2 tactical era complete (693 L2
  sources total, batches #78–#87 / log cont. 56–65, 2020-03-14→2020-10-22 solo run; fully
  Neil-attributed; spans the SEO Unlocked link-building module completion, the full eCommerce
  Unlocked course, the full Content Marketing Unlocked course wrap-up already folded, the full
  Instagram Unlocked course, and the YouTube Unlocked course completion). Drained the 10 accumulated
  `Synthesis notes:` lines. Promotions (quality-over-volume; pure repeats/reinforcements dropped):
  **seo** (the **Link Building Score Card** — links-as-a-voting-system ★; **"YouTube SEO is the
  opposite of traditional SEO"** first-24-hours doctrine ★, a distinct counter-model to the
  accretive/authority SEO doctrine; a GSC near-miss-query keyword-gap method; a small-site
  ranking case-study bundle — Gaps.com exact-match/near-me domains, diversity update, About.com
  niche-split), **content-marketing** (**Franklin's Law of Content Success** ★; the **WHIPS**
  buyer-awareness framework ★; the **STEPS** editing checklist ★; the neilpatel.com
  positioning self-critique extending corporate-brand-over-personal-brand), **analytics-cro**
  (the landing-page UX checklist — speed/fold/clutter with named studies ★; the **"hoop theory"**
  checkout-commitment framework + Doofinder ★; hard ecommerce PDP/cart-abandonment figures —
  69.23%/35.26%/1%→2.5% ★; dark-traffic/"not provided"-keyword Analytics mechanics), **paid-ads**
  (the Amazon **ACOS** framework + review-velocity target + explicit anti-manipulation stance ★;
  marketplace-ads survey), **agency-entrepreneurship** (the **Vitamin Water/Mike Repole $4.1B**
  case study — "solve a genuinely unmet need" ★; the "let me think about it" sales-objection
  framework), **social-media** (the full **Instagram Unlocked** playbook — bio-link-as-profit-center,
  Instagram-algorithm-as-dwell-time, "Instagram SEO", influencer vetting, Kylie Cosmetics/Frank
  Body case studies, anti-account-buying stance; the **Grace & Lace** micro-influencer case study;
  the Etsy emotional-positioning exception; the first explicit, repeated self-attribution to
  **Gary Vaynerchuk's** engagement-grind tactic). Persona: **beliefs.md** (76→81 sources; the
  neilpatel.com self-critique + Vitamin Water case extending corporate-brand-over-personal-brand,
  the Branson-meeting origin story, the named Gary Vaynerchuk credit, "I don't take holidays... I
  don't count hours"), **voice.md** (53→55 sources; the Marcus Aurelius touchstone quote, "I don't
  take holidays" self-description, the 1989 Toyota Camry aside), **biography.md** (47→49 sources;
  "Real Cool Videos"/partner Ahmed small venture, the comment-reply habit dated to ~2007). Recompiled
  **system-prompt.md v9 → v10** (compiled_from_sources 613 → 693). No new contradictions beyond
  those already flagged per-source (title/date-mismatch QA notes, the 8,200-blog-posts figure left
  unreconciled against the 2019 4-posts/mo+90-updates/mo rate). System-prompt version at pass end:
  **v10**.
- [x] 2026-07-21 — **synthesis pass 8** — @neilpatel 2019-09 → 2020-03 P2 solo tactical era complete (613 L2 sources total, batches #69–#77 / log cont. 47–55, 2019-09-16→2020-03-12 solo run; fully Neil-attributed, plus the batch #68 leftover debt already folded into beliefs/voice by the prior Stage-P persona pass). Drained the 9 accumulated `Synthesis notes:` lines (batch #76 added none). Promotions (quality-over-volume; pure repeats dropped): **seo** (new "2019-10 → 2020-03" section — **infographic-backlink hack** 47 infographics/41,142 backlinks ★; **optimize-over-create** 477K-keyword formula ★; **advanced link-building playbook** 7 named plays ★; named Chrome-extension tool stack; **"keywords that never sell"** negative-keyword taxonomy ★; comparison-keywords-as-purchase-decided; **zero-click doctrine** "Google is not evil" ★; **E-A-T/Medic checklist** with self-disqualification ★; **"optimize for people not the platform"** first principle ★; **domain-authority debunk** ★; high-CPC-over-volume; YouTube channel-growth formula), **content-marketing** (**headline-writing formula** ★; content-operation quantified 4 posts/mo+90 updates/mo+12 videos/mo ★; **"tools are content marketing"** doctrine ★; three-signal content validation ★; KISSmetrics-1M-via-guest-posting ★; speak-don't-type habit + writer-hiring protocol), **agency-entrepreneurship** (**Ubersuggest bet costed** >$3M + don't-copy-me caveat ★; product-brand>personal-brand mechanism ★; "brand is the best moat" thesis ★; international-expansion origin story (Google-employee friend, Brazil-first, <25% US traffic) ★; NP Digital SMS sales motion; 5-step affiliate-selection framework; Sujan-Patel-is-cousin + brand-building mechanics), **analytics-cro** (retargeting logic↔emotion flip; popup-ceiling 2-3 max; anti-dashboard operating cadence), **social-media** (Facebook pages→groups + Messenger-bot doctrine ⚠️ dated; YouTube-SEO as alternative search engine; YouTube channel-growth formula cross-link), **email-marketing** (Frank Kern sequencing principle; repeat-vs-new segmentation), **paid-ads** (retargeting flip cross-link). New entity page: [[wiki/entities/sujan-patel]] (Neil's cousin). Persona: **beliefs.md** (68→76 sources; product-brand>personal-brand mechanism extending the corporate-brand belief, optimize-for-people-not-platform + Bezos provenance extending put-the-user-first, zero-click/"Google is not evil", domain-authority debunk, endorsing-Google-against-own-interests, Ubersuggest-bet-costed+don't-copy-me), **voice.md** (50→53 sources; "I prefer it over writing", "when it's not converting into revenue, STOP doing that", anti-dashboard "focus on execution" line), **biography.md** (44→47 sources; international-expansion origin story, KISSmetrics-1M-guest-posting extension, speaking-fee $25-50k/talk, Sujan-Patel-cousin). Recompiled **system-prompt.md v8 → v9** (compiled_from_sources 541 → 613). No new contradictions beyond those already flagged per-source (title/date-mismatch QA notes, attribution-uncertain third-party name spellings). System-prompt version at pass end: **v9**.
- [x] 2026-07-20 — **synthesis pass 7** — @neilpatel 2019-02 → 2019-09 P2 solo tactical era complete (533 L2 sources total, batches #58–#67 / log cont. 37–46, 2019-02-18→2019-09-14 solo run; fully Neil-attributed). Drained the 10 accumulated `Synthesis notes:` lines. Promotions (quality-over-volume; pure repeats dropped): **seo** (new 2019 section — **Three Unseen Laws of SEO** = brand-queries + user-metrics + adapt-to-tech ★; **user-first/search-intent** ranking with the Ahrefs free-backlink-tool case; the **no-link-building triad** land-and-expand / content-clusters / content-gaps ★; **Bing-vs-Google** first dedicated contrast — social signals a DIRECT Bing factor), **content-marketing** (**content-volume-by-Ubersuggest-domain-score** heuristic ★; **storytelling framework** core-message→story-type→CTA + Significant Objects; **rank-OLD-content** ops doctrine — 90+ updates/mo → ~4M visits; "content is king = worst advice / promotion is king" sharper articulation; repurposing micro-content playbook), **agency-entrepreneurship** (**agency cold-outreach playbook** Crunchbase→teardown→CEO cold email, "1–2 clients per 5 emails," only if raised ≥$1–2M ★; **selling-services 5-lever framework** ★ + premium/anti-discount; **disruption doctrine quantified** — free Ubersuggest self-reported ~$200k/mo loss to win brand queries, the through-line to 2026 "FREE is the lever"), **paid-ads** (**funnel-hacking doctrine** — copied funnel ≠ results; "the secret is the funnel not the ad" + LTV levers), **analytics-cro** (**quizzes +280% leads** ★; **load-time → +6% conversions/sec** Crazy Egg; **survey→A/B→re-survey** loop; **raise-price-to-raise-sales** Diamond Foundry ⚠️ vs undercut-pricing; anti-discount 29%-faster-churn datum), **social-media** (channel-ROI realism — IG indirect for B2B, big-influencer buys lose money (Kris Jenner ~$85k); rule-of-7 omnichannel + re-share cadence), **email-marketing** (ecommerce email tactics; **MobileMonkey/Messenger** 2019 boosterism ⚠️ date-stamped as later-reversed), **ai-marketing** (**2020 "automate SEO with AI/ML" JS-snippet vision** ★ — the datable origin of the 2025–26 AEO arc). Persona: **beliefs.md** (56→63 sources; 7 Rules of Money wealth philosophy, Power of No / premium-over-discounts, no-morning-routine, Three Unseen Laws of Entrepreneurship, put-the-user-first, career-sequencing ⚠️ flagged), **voice.md** (44→49 sources; "content is king is a bunch of bologna → promotion is king", "the best marketer is the one who can spend the most money on marketing", "if you want good stuff you got to pay a premium dollar", "a morning routine will not make you successful", "it's like dating — play hard-to-get"), **biography.md** (39→44 sources; fuller lost-$1M-before-21 cloud venture, KISSmetrics $17M/copycat-$100M post-mortem, "did the marketing for TechCrunch" ⚠️, pre-Ubersuggest sub-$100 CodeCanyon script, doesn't-read-many-books). Recompiled **system-prompt.md v6 → v7** (compiled_from_sources 453 → 533). **⚠️ Two flagged items carried, not smoothed**: (1) **career-sequencing** "work for others ~9 years first" (2019) vs his own teen-founder path — kept as dated retrospective advice; (2) **raise-price-to-raise-sales** (Diamond Foundry) vs **undercut-to-grow** pricing — both context-dependent, dated. System-prompt version at pass end: **v7**.
- [x] 2026-07-20 — **synthesis pass 6** — @neilpatel 2018-07 → 2019-02 P2 tactical + origin-story era complete (453 L2 sources total, batches #48–#57 / log cont. 27–36, 2018-07-28→2019-02-16 solo run; Neil-attributed, Adam Lodolce / summit-host interviewer material gated out). Drained the 10 accumulated `Synthesis notes:` lines. Promotions (quality-over-volume; pure repeats dropped): **seo** (new "2018-H2 → 2019" section — the **7 SEO experiments** canonical growth story 9k→449k / brand-query "Who is Neil Patel" +24% / entry-popup bounce 85.7→72.9% ★; **international-SEO playbook + subdomain self-reversal** ⚠️ vs 2017 subdirectory doctrine ★; own-the-whole-first-page interlinking; brand-as-top-factor reinforced; Google-vs-YouTube ranking-speed contrast; expand+prune+GIF-infographics), **agency-entrepreneurship** (new "2018-H2 → 2019" section — **free-product-as-acquisition-channel** ★ the ancestor of the 2026 "FREE is the lever" thesis; the **7-point agency-hiring vetting checklist** ★; downturn cut-yourself-first; acquire-with-leverage LBO; team>founder; never-rely-on-one-source), **analytics-cro** (**LTV 7/8/9-figure ad-spend model** ★; CRO-beats-acquisition; undercut-to-grow pricing ⚠️; **always-test-AND-retest + the Google-login tale** ★ = dated origin of the 2025 "what works now won't work forever" belief; BuiltWith→Wayback competitor A/B mining), **paid-ads** (SEO-vs-paid do-both; funnels-as-ad-costs-rise + **2008-recession ad-durability datapoint** = antecedent of 2021 recession-durable claim), **content-marketing** (**"blog less, promote more" 7×→1×/wk, 800K→1.6M/mo** ★ = dated antecedent of the 80/20 rule; advanced-content session; **content freshness/recency**; blogging-still-works-2019), **social-media** (first-hour-engagement "opposite of SEO"; Facebook-group→email qualify>size; IG-Stories volume formula; LinkedIn "see more" + comment>like; FB-native-posting; IG-weak-for-B2B), **email-marketing** (first-hour email+push blast; **Messenger-chatbot 60%+ open beats email** ⚠️ dated), **ai-marketing** (**"AI won't matter on landing pages, VR will" (2018)** ★ now-falsified belief-evolution datapoint appended to the 2018 AI-forecast section). Persona: **beliefs.md** (51→56 sources; **corporate-brand > personal-brand** contrarian belief with 2019→2024 through-line, **give-first-to-the-extreme** / refuses ads-sponsorships-affiliate, **"#1 SEO trick is building a brand"** 2018 seed, **"future is video / text overrated"** belief-evolution flagged, **judge-channel-by-connection-not-revenue**), **voice.md** (40→44 sources; "little is the new big", "page 2 = where you bury the dead bodies", "better than most", "biggest vs most-qualified group"), **biography.md** (34→39 sources; **Elpac Electronics** first-big-client named + **PokerStrategy** first-$1.2M contract + "little is the new big"; **Rockwall/fake-cancer >$1M fraud → never-burn-bridges**; **brother-in-law partner / lawyer Joey Tran / FTC-class-action** legal history; **immigrant-mother-taught-free-6-months**; **Seattle discrepancy** ⚠️ carried), **appearance.md** (1→2 sources; **six-figure dress-for-success experiment** → reverted to comfort). Recompiled **system-prompt.md v5 → v6** (compiled_from_sources 373 → 453). **⚠️ Three flagged items carried, not smoothed**: (1) the **Seattle/Vienna bio detail** ("lived a lot of my life in Seattle," a ~2014 re-upload) vs SUBJECT.md England→Orange County — recorded as an unreconciled discrepancy, NOT folded into the timeline/persona; (2) the **corporate-brand-over-personal-brand** contrarian belief, in tension with his own personal-brand-built business; (3) the **Elpac/PokerStrategy origin** promoted as concrete dated bio (reconciled against, not overwriting, the earlier "$25M first client" line). System-prompt version at pass end: **v6**.
- [x] 2026-07-19 — **synthesis pass 5** — @neilpatel 2018-01 → 2018-07 P2 tactical + mindset era complete (373 L2 sources total, batches #38–#47, 2018-01-04→2018-07-26 solo run; fully Neil-attributed, Adam Lodolce interviewer material gated out). Drained the 10 accumulated `Synthesis notes:` lines. Promotions (quality-over-volume; pure repeats dropped): **agency-entrepreneurship** (new "2018 solo-era operating principles" section — globalization/reinvest-everything $0-salary; the acquisition/M&A doctrine buy-at-2.5–3x/buy-traffic/multiple-arbitrage ★ flagged as the 2026 precursor; hire-for-hunger + culture doctrine; VC-raising playbook; intrapreneurship/apprentice-first; validate/niche/brand-byproduct; freemium-FREE "media-company/eyeballs" ★; client-concentration survival; the **"Who is Neil Patel?" campaign apology** ★), **seo** (new "2018 solo-era tactical playbook" — content clusters+long-tail buyer-intent ★, **RankBrain as UX-signals** ★, internal-linking doctrine, mobile-first index, voice search, YouTube-as-search-engine, automated-outreach stack, duplicate-content handling, three unorthodox plays, **black-hat war stories as anti-patterns** ★), **ai-marketing** (the **2018 AI-in-marketing forecast** ★ — IoT/programmatic, privacy-law-as-constraint — carried as belief-evolution vs 2025–26 AEO), **paid-ads** (product-launch funnel + opposite-pitch cart-abandonment remarketing ★; $400K FB-ads lessons ★; search-intent-first), **analytics-cro** (pricing/split-test-for-total-revenue doctrine ★; money-back-guarantee-as-UX-lever; GDPR-as-global-default), **content-marketing** (content assembly line/hire-writers-with-audience ★; underdog-platform arbitrage; one-product engine), **social-media** (FB-native-video-beats-YouTube; FB engagement-first algo; IG Stories lead-gen; master-one-platform; personal-brand-for-equity), **email-marketing** (deliverability + monthly list-scrub; content-upgrades), plus [[wiki/entities/mike-kamo]] (Mazda-dealership origin). Persona: **beliefs.md** (36→51 sources; acquisition/M&A doctrine + through-line callout, globalization, freemium-mindshare, success-is-happiness/privacy, hire-for-hunger/culture, innovate-don't-copy, validate-before-build/brand-byproduct, apprentice-first, dated 2018 crypto opinion flagged NOT-doctrine), **voice.md** (36→40 sources; "I don't care for the money, let me help you" closer, "I don't think I'm successful"/"success is subtractive"), **biography.md** (23→34 sources; black-hat era entry, fuller doctor→CS→business origin arc + theme-park-restrooms-funded-failed-agencies, KISSmetrics >$10M/$4M-burned/$17M, VC >$20M lifetime, 2018 globalization/Brazil/$0-salary, "Who is Neil Patel?" apology + "learned entrepreneurship from my mom," teenage $25K/mo client scare), and **appearance.md** (0→1 source — **first content**: the shaved-head-by-choice origin + anti-flashy self-presentation). Recompiled **system-prompt.md v4 → v5** (compiled_from_sources 295 → 373). **⚠️ Three belief-evolution items carried, not smoothed**: (1) 2018 AI forecast vs 2025–26 AEO; (2) the M&A doctrine 2018→2026 through-line; (3) the black-hat-past confession framed as his "think long-term" lesson (kept in the wiki as biography/anti-patterns, out of the persona as advice). System-prompt version at pass end: **v5**.
- [x] 2026-07-19 — **synthesis pass 4** — @neilpatel 2017-09 → 2017-12 P2 tactical + wealth-mindset era complete (295 L2 sources total, batches #28–#37, 2017-09-04→2017-12-28 solo run; fully Neil-attributed). Drained the 10 accumulated `Synthesis notes:` lines. Promotions (mostly period-tactical, into the topic hubs; quality-over-volume, pure repeats dropped): **seo** (learn-by-doing throwaway-site method; dofollow-vs-nofollow; the 404 hack; Google search operators; SERP-CTR playbook; Reddit 2017 antecedent; **local SEO for brick-and-mortar** — first sustained local cluster; the five SEO metrics / impressions-before-clicks; **owned-site growth curve 9k→89k→450k over 2yr** ★; **rank-#1 pillar-content playbook** /seo 1.5yr climb + brand tiebreaker; make-your-site-linkable), **analytics-cro** (optimize-before-volume; Crazy Egg 3-step loop; manufacture-urgency; personalization CRO; contact-page CRO; CTA placement; carousels-hurt; two-step-checkout recovery; anti-"specific-colors-convert"; **the 2017-11 measurement mini-series** — platforms over-report, validate against your own revenue ★), **paid-ads** (FB cost control; AdWords profitability levers; partner/affiliate as free traffic; profitable display; **AdWords Quality-Score "Google optimizes its own revenue" model**; high-ticket sales funnel; contests-as-lead-gen-front; mobile-app install; **2017 automated-webinar antecedent** ★ of the 2018 playbook), **content-marketing** (growth-hacking = cross-functional; make-money-blogging paths; blog-virality = emotion-first; 6-tips-great-blog-post + "dumbest person in the room"; **headline-primacy** — shares driven by headline ★; Skyscraper 10→101 outreach template), **social-media** (**posting-cadence doctrine** — volume over perfection + the **best-time-to-post mini-series** across all 4 platforms; LinkedIn native-teaser distribution; IG hashtag doctrine; Snapchat-vs-IG; social listening; social metrics = growth-rate-not-total; IG Stories; FB Live sales), **email-marketing** (double-open-rate levers; email-CTR hacks; sell-more-to-existing-customers), **agency-entrepreneurship** (differentiate by story+USP; don't-copy-competitors triad; **reputation/reviews** as a local-marketing discipline; referral-program hacks; wealth-mindset "7 secrets"; blog-to-$1k/mo; **"I'm a terrible manager"** operating self-awareness; **the candid Hustle bestseller mechanics** — service-trade bulk buys / ResultSource ★); persona **beliefs.md** (34→36 sources; money-is-hollow/business-as-sport 2017 seed, distrust-platform-numbers), **voice.md** (32→36 sources; "dumbest person in the room", "picking up trash and cleaning restrooms", "terrible manager", curiosity-gap headline), **biography.md** (18→23 sources; Hustle candid book-launch mechanics + $500k advance, Marketing School podcast origin ~500k listens/mo, management self-awareness, home-robbed-twice color); recompiled **system-prompt.md v3 → v4** (compiled_from_sources 215 → 295). **⚠️ CONTRADICTION carried, not smoothed**: "dirt poor" (2017-12-11) vs "middle class America" (2017-11-30), same week — childhood economic status inconsistent, both self-reported (flagged on biography.md). System-prompt version at pass end: **v4**.
- [x] 2026-07-19 — **synthesis pass 1** — @neilpatel P1 era complete (72 L2 sources, batches #1–#9). First synthesis pass: promoted the 9 accumulated `Synthesis notes:` lines into all 8 `wiki/topics/` hubs + `persona/beliefs.md` (19 sources), `persona/voice.md` (21 sources), `persona/biography.md` (augmented to 11 sources); compiled `persona/system-prompt.md` **v1**. System-prompt version at pass end: **v1**.
- [x] 2026-07-19 — **synthesis pass 3** — @neilpatel 2017 P2 solo tactical era complete (215 L2 sources total, batches #18–#27, 2017-05→2017-09 solo run; fully Neil-attributed). Drained the 10 accumulated `Synthesis notes:` lines. Promotions (mostly period-tactical, promoted into the topic hubs; quality-over-volume, pure repeats dropped): **seo** (2017 brand→branded-search origin + Google-Trends-as-brand-size; subdirectory-vs-subdomain site architecture; tier-two link building; hreflang/internationalization; local link building; 2017 URL-date-removal +58% datapoint; blog-URL-categories; CTR-from-paid-ads; pogo-sticking signal; get-indexed 3-step; site-speed ladder; Google News; AMP-prediction flagged superseded), **analytics-cro** (data-over-guesswork CRO sequence; A/B-test validity thresholds; opt-in cannibalization; CTA rules; copy=objection-handling; social-proof placement), **content-marketing** (adjacent-emotion ideation; About-page 5-part framework; curation automation stack; Yesware/Boomerang outreach), **paid-ads** (FB-vs-Google intent heuristic; retargeting rule-of-seven + budget anchor; don't-boost-posts; affiliate-as-CPA), **social-media** (LinkedIn native-publishing; never-buy-FB-fans; relevance-over-reach influencer rule), **email-marketing** (deliverability system; email-signature channel + "max 2 asks"), **agency-entrepreneurship** (ugly/tumbleweed niche; freemium-beats-incumbent; monetization stack; lead-quality-not-volume; outsource-on-a-budget; fake-site sandbox); persona **beliefs.md** (32→34 sources; "one-up yourself, not your competition", "optimize for lead quality, not volume"), **voice.md** (28→32 sources; "P.S. ...make my year" share-close, dyslexia disclosure, one-up-yourself refrain, "one structural change beat years of link building"), **biography.md** (16→18 sources; ~2001 SEO start, ~$400k Facebook-fans mistake); recompiled **system-prompt.md v2 → v3** (compiled_from_sources 135 → 215). System-prompt version at pass end: **v3**.
- [x] 2026-07-19 — **synthesis pass 2** — @MarketingSchoolPod P1 era complete (135 L2 sources total, batches #10–#17; co-hosted with Eric Siu, only Neil-attributed material promoted). Drained the 8 accumulated `Synthesis notes:` lines. Promotions: **ai-marketing** (new dated GEO/AEO 2023→2026 timeline + AI-augments extensions), **seo** (SEO-career adaptation, Reddit playbook, "old-school SEO is dead"), **agency-entrepreneurship** (conferences/events acquisition, agency M&A/valuation/financing, debt "turns," clean-story spinoff, AI-era business models), **content-marketing** (how-to-learn loop, write-conversationally, mine client-facing team), **social-media** (personal-brand power/fragility, keep-politics-out), **paid-ads** (creative + first-party data levers), **analytics-cro** (AI vanity-metric trap, 3,000-LP benchmarks); persona **beliefs.md** (→32 sources), **voice.md** (→28 sources; new Marketing School coinages), **biography.md** (→16 sources; ~1,000 employees, Ubersuggest LLM tracking, M&A hunting); recompiled **system-prompt.md v2**. Ephemeral 2026-Q1/Q2 model-news (Opus 4.5, token costs, Jensen Huang, etc.) deliberately NOT promoted per the do-not-promote flags. System-prompt version at pass end: **v2**.
