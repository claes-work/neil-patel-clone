# BACKLOG — everything still open in this project

**How to use this in a NEW session:** just say _"Read BACKLOG.md and summarize what's
still open."_ This is the single human-readable checklist of all planned work. Tick
`[x]` when done; keep it current after each work block. (Machine state of truth for
sources stays in `pipeline/ledger.csv`; this file is the plain-language overview.)

**Snapshot (2026-07-14):** Bootstrap complete for **Neil Patel** (NP Digital / SEO).
Ledger: 4,675 items, all L0 — 124 P1 / 1,832 P2 / 2,719 P3; 2,005 long-form + 2,670
shorts across @neilpatel (2,461) and @MarketingSchoolPod (2,214, co-hosted with Eric Siu
→ attribution-gated). Book identified: *Hustle* (2016, co-authored) — text needed from
user. Next: `/loop /ingest-loop`.

---

## A. Bootstrap — DONE 2026-07-14
- [x] Run `/clone-setup Neil Patel` (identity check → SUBJECT.md → biography research
      → source map → taxonomy → channel enumeration → first commit)

## B. Video ingest — OPEN
- [ ] Drain P1 (landmark), then P2 long-form per channel (ingest loop)
- [ ] P3 guest content with attribution pass
- [ ] Shorts dedup (dupes → skipped with `dup-of:`, new → L2)
- [ ] Retry rows flagged `429` / `no-captions` / `unavailable`
- [ ] Checkpoint synthesis every ~10 batches / channel boundary (see E)

## C. Books / courses / landmark documents — OPEN
- [x] Identify what exists: *Hustle* (2016, ISBN 9781623367169, co-authored with
      Vlaskovits & Koffler — partial attribution); plus the neilpatel.com guides and
      Ubersuggest workflows (see media inventory dossier)
- [ ] Obtain *Hustle* text from the user → `raw/books/` → L3 ingest (attribute Neil's chapters)

## D. Other sources — blocked on A
- [ ] Websites/blog · press · X · Instagram · LinkedIn · podcast feeds · newsletters

## E. Synthesis / persona — ongoing once B starts
- [ ] Keep synthesis debt drained (`python tools/synthesis_batch.py status`)
- [ ] Recompile `persona/system-prompt.md` after every persona-touching pass (bump version)
- [ ] Persona-QA sessions → feed `wiki/gaps.md`
- [ ] Final lint when the corpus drains

## F. Multi-clone future — see VISION.md
- [ ] More people, each in its own repo built from this template
- [ ] Clones as cooperating agents (shared data contract, knowledge never mixed)
