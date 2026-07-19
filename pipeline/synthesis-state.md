# Synthesis state

_Tracks the synthesis **high-water mark** so the synthesis loop never misses material and never
re-does work. Companion to the ingest ledger (`ledger.csv`). The detailed debt lives in `log.md`
as `Synthesis notes:` lines (every ingest batch appends one). See `tools/SYNTHESIS.md` for the loop
and `tools/synthesis_batch.py` for the driver._

## High-water mark
Synthesized through: **@MarketingSchoolPod P1 era complete — all 135 L2 sources, ingest batches #1–#17 (2016-11 → 2026-07)**, via synthesis pass 2 (2026-07-19). Pass 2 folded the @MarketingSchoolPod P1 co-hosted era (batches #10–#17, 8 `Synthesis notes:` lines of debt) into topics + persona. The next pass starts from the debt accumulated after batch #17 (i.e. the @MarketingSchoolPod P2 / @neilpatel P2 ingest that follows).

## Pending checkpoints
_(oldest first; the synthesis loop drains these top-down)_
_(none — caught up through batch #17; @MarketingSchoolPod P1 era fully synthesized)_

## Done checkpoints
- [x] 2026-07-19 — **synthesis pass 1** — @neilpatel P1 era complete (72 L2 sources, batches #1–#9). First synthesis pass: promoted the 9 accumulated `Synthesis notes:` lines into all 8 `wiki/topics/` hubs + `persona/beliefs.md` (19 sources), `persona/voice.md` (21 sources), `persona/biography.md` (augmented to 11 sources); compiled `persona/system-prompt.md` **v1**. System-prompt version at pass end: **v1**.
- [x] 2026-07-19 — **synthesis pass 2** — @MarketingSchoolPod P1 era complete (135 L2 sources total, batches #10–#17; co-hosted with Eric Siu, only Neil-attributed material promoted). Drained the 8 accumulated `Synthesis notes:` lines. Promotions: **ai-marketing** (new dated GEO/AEO 2023→2026 timeline + AI-augments extensions), **seo** (SEO-career adaptation, Reddit playbook, "old-school SEO is dead"), **agency-entrepreneurship** (conferences/events acquisition, agency M&A/valuation/financing, debt "turns," clean-story spinoff, AI-era business models), **content-marketing** (how-to-learn loop, write-conversationally, mine client-facing team), **social-media** (personal-brand power/fragility, keep-politics-out), **paid-ads** (creative + first-party data levers), **analytics-cro** (AI vanity-metric trap, 3,000-LP benchmarks); persona **beliefs.md** (→32 sources), **voice.md** (→28 sources; new Marketing School coinages), **biography.md** (→16 sources; ~1,000 employees, Ubersuggest LLM tracking, M&A hunting); recompiled **system-prompt.md v2**. Ephemeral 2026-Q1/Q2 model-news (Opus 4.5, token costs, Jensen Huang, etc.) deliberately NOT promoted per the do-not-promote flags. System-prompt version at pass end: **v2**.
