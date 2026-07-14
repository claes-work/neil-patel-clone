---
type: web-research
source_date: 2026-07-14
ingested: 2026-07-14
tags: [media-inventory, pipeline, enumeration, channels, podcast, socials, courses, guest-appearances]
---

# Media inventory dossier — Neil Patel (as of 2026-07-14)

Phase-2 consolidation of the full media surface of the SUBJECT (**Neil Patel** —
digital-marketing / SEO entrepreneur, co-founder of NP Digital, creator of Ubersuggest,
co-host of the *Marketing School* podcast). YouTube channel IDs and video/short counts
come from direct **yt-dlp** enumeration run on 2026-07-14; subscriber counts are
yt-dlp's `channel_follower_count` at the same time. Everything else was verified or
extended via web research on 2026-07-14. Every number carries its as-of date and source.
Follower counts are platform-self-reported unless noted; nothing here is
registry-verified.

**Identity guard (critical):** there are several public people named "Neil Patel." This
dossier covers ONLY the marketer (handle `@neilpatel` everywhere, co-founder NP Digital,
book *Hustle*). Explicitly NOT: Neil Patel MD (physician/YouTuber), any "Neil Patel"
actor/academic, or same-name fan accounts. See Excluded channels below.

## YouTube channels (yt-dlp enumeration, 2026-07-14 — authoritative for IDs/counts)

| Channel | Channel ID | Subs (2026-07-14) | Content (2026-07-14) | Role | Verdict |
|---|---|---|---|---|---|
| [@neilpatel](https://www.youtube.com/@neilpatel) | `UCl-Zrl0QhF66lu1aGXaTbfw` | 1,590,000 | **1,178 long-form + 1,284 shorts** (≈2,462 uploads) | Main corpus — Neil on camera, "learn digital marketing in 5 minutes a day" | **TARGET** |
| [@MarketingSchoolPod](https://www.youtube.com/@marketingschoolpod) | `UCTJmkA2-u7Kyblm5_P6tKdA` | 15,100 | "Marketing School - Daily Marketing Tips" — video/clip mirror of the daily podcast (thousands of short episodes) | Podcast channel, **co-hosted with Eric Siu** | **TARGET (attribution-gated)** |

Legacy vanity URLs `youtube.com/c/NeilPatel` and `youtube.com/user/neilvkpatel` both
resolve to the same main channel `UCl-Zrl0QhF66lu1aGXaTbfw` (verified via yt-dlp,
2026-07-14).

Cross-check on the main channel: Social Blade / vidIQ report ≈2,362 total uploads and
1.58M subs (socialblade.com/youtube/handle/neilpatel; vidiq.com, 2026-07-14) — consistent
with the yt-dlp 2,462-item / 1.59M figures (the delta is normal tab-vs-total counting and
recent uploads). Total lifetime views ≈82.7M (vidIQ, 2026-07-14).

**Host-attribution notes (binding for fidelity):**
- `@neilpatel` is Neil-fronted and is the **primary persona corpus**. Even here, some
  shorts and older uploads may feature NP Digital staff or be voiced-over agency content —
  attribute the speaker before anything flows into persona files.
- `@MarketingSchoolPod` is a **two-host** show (Neil Patel **and** Eric Siu, founder of
  Single Grain / Leveling Up). Roughly half of every episode is Eric, not Neil. **Every
  ingest from this channel MUST tag the speaker**; only Neil's turns are persona-training
  data. Treat Eric's turns as context, never as Neil's voice. This is the single biggest
  attribution risk in the whole inventory.

## Podcast — "Marketing School - Digital Marketing and Online Marketing Tips"

- **Hosts**: Neil Patel + **Eric Siu** (co-host, co-owner). Daily cadence, short episodes
  (typically 5–10 min). Active 2016–present.
- **Apple Podcasts**: id `1138869817`
  ([podcasts.apple.com/us/podcast/.../id1138869817](https://podcasts.apple.com/us/podcast/marketing-school-digital-marketing-and-online/id1138869817)).
  Apple shows "Updated Daily," years active 2016–2026, rating **4.6/5 from 1,249 ratings**;
  latest episode fetched 2026-07-14 ("Your Brand Is Invisible in AI Search (Here's the Fix)").
- **Spotify**: show `1NulSGKhstJuty8iYPBMo5`
  ([open.spotify.com/show/1NulSGKhstJuty8iYPBMo5](https://open.spotify.com/show/1NulSGKhstJuty8iYPBMo5)).
- **Website**: [marketingschool.io](https://marketingschool.io/) (full episode archive at
  `/all-episodes/`, paginated).
- **Episode count**: **2,500+** per Apple's own blurb (2026-07-14); a third-party
  aggregator (player.fm) lists ~3,559 feed items — treat 2,500–3,500 as the working range
  and pin an exact number from `marketingschool.io/all-episodes` at ingest time if needed.
- **Downloads**: "nearly 100 million" (Apple description / marketingschool.io, 2026-07-14 —
  self-reported).
- **RSS/host**: not directly captured (Apple id resolves the enclosure feed; hosting
  provider likely Libsyn — to confirm at ingest). Use Apple `1138869817` / Spotify
  `1NulSGKhstJuty8iYPBMo5` as the canonical directory IDs.
- **Dedup rule (binding for the ledger)**: the daily podcast is **mirrored** to
  `@MarketingSchoolPod` on YouTube. When both exist for the same episode, **YouTube is the
  primary ingestion source** (it carries video + captions); audio feed items enter the
  ledger only when no matching YouTube upload exists (match on title + publish date),
  and matched items stay L1 with `dup-of:<youtube-id>`. **Speaker-tagging (Neil vs Eric)
  is required regardless of which surface the item comes from.**

No evidence of a separate solo Neil Patel podcast as of 2026-07-14 — *Marketing School*
is his one recurring show. (Eric Siu's *Leveling Up* is Eric's, not Neil's — exclude.)

## Books

| Title | Year | Details | Source |
|---|---|---|---|
| *Hustle: The Power to Charge Your Life with Money, Meaning, and Momentum* | 2016 | **Co-authored** with Patrick Vlaskovits and Jonas Koffler. Rodale/Macmillan. ISBN-13 **9781623367169**, ISBN-10 **1623367166**. NYT / USA Today / LA Times bestseller. | amazon.com, penguinrandomhouse.com, goodreads.com, 2026-07-14 |

Attribution note: *Hustle* is a **three-author** book — the "money/meaning/momentum"
framework and much prose are not solely Neil's. Persona-relevant, but do not attribute the
whole book's voice to Neil.

Beyond the trade book, Neil publishes long-form **guides/e-books** on neilpatel.com (e.g.
"The Advanced Guide to SEO," "The Advanced Guide to Content Marketing," Quick Sprout
guides). These are website assets, not ISBN books — treat as blog corpus (below), not as
the book list. NOT his book: any title by "Neil Patel MD" or other same-name authors.

## Socials

Neil's own **self-reported** breakdown (X/LinkedIn/TikTok/Threads post, 2024-01-26):
"3.8M total — YouTube 1.2M · Facebook 1M · LinkedIn 571,821 · Instagram 495,000 ·
X 465,500 · TikTok 138,000." Use as a dated anchor; several are stale.

| Platform | Handle | Count | As of | Source | Confidence |
|---|---|---|---|---|---|
| YouTube | [@neilpatel](https://www.youtube.com/@neilpatel) | 1,590,000 | 2026-07-14 | yt-dlp direct | High |
| LinkedIn | [in/neilkpatel](https://www.linkedin.com/in/neilkpatel/) | 571,821 (self-report); likely higher now | 2024-01-26 (STALE) | Neil's own post | Medium. Very active platform; posts daily. |
| Instagram | [@neilpatel](https://www.instagram.com/neilpatel/) | 652,000 (2026 tracker) vs 495,000 (self-report) | 2026-07-14 / 2024-01-26 | search snippet; Neil's post | Medium. Growth curve 495K→652K plausible. |
| X / Twitter | [@neilpatel](https://x.com/neilpatel) | 465,500 | 2024-01-26 (STALE) | Neil's own post | Low. X blocks scraping; no fresh count fetchable 2026-07-14. |
| TikTok | [@neilpatel](https://www.tiktok.com/@neilpatel) | 295,900 (current) vs 138,000 (self-report) | 2026-07-14 / 2024-01-26 | search snippet; Neil's post | Medium. |
| Facebook | Neil Patel page | ~1,000,000 | 2024-01-26 (STALE) | Neil's own post | Low. |
| Threads | [@neilpatel](https://www.threads.com/@neilpatel) | count not established | 2026-07-14 | cross-posted the 3.8M breakdown | Low — existence confirmed, count unknown. |

Handle is uniformly **`@neilpatel`** across YouTube, Instagram, X, TikTok, Threads;
LinkedIn is the outlier **`in/neilkpatel`** (K = Kishorbhai). NP Digital company handles
use `@npdigital` / `@npdigitalglobal`.

## Websites / properties / tools

Neil's surface is a **web-property empire**, not a single hub. Key sites (2026-07-14):

- **[neilpatel.com](https://neilpatel.com/)** — flagship personal blog + tool hub;
  ~1.7M visitors/month (self-reported); tagline "Helping You Succeed Through Digital
  Marketing." Home of the **blog** (thousands of SEO/content/ads/analytics articles — many
  team-written; **attribution required** before persona use), the **[newsletter](https://neilpatel.com/newsletter/)**
  (~1.58M subscribers, self-reported; mostly text emails, "Proven Marketing Tips"), and the
  Ubersuggest tool landing (`/ubersuggest/`).
- **[npdigital.com](https://npdigital.com/)** — NP Digital, his global marketing agency
  (he is co-founder/CMO). Corporate/agency voice — not Neil's personal voice.
  `advanced.npdigital.com` hosts webinars/lead magnets.
- **[quicksprout.com](https://www.quicksprout.com/)** — his older SEO/blogging property;
  still publishes reviews/guides.
- **Ubersuggest** — free SEO/keyword tool he acquired and relaunched (delivered under
  neilpatel.com/ubersuggest and app.neilpatel.com). Flagship product; heavily referenced
  in his content.
- **[marketingschool.io](https://marketingschool.io/)** — the podcast's site.
- Other tools associated with Neil / his history: **AnswerThePublic** (acquired), **Hello
  Bar**, **Subscribers.com**, and (earlier co-founds) **Crazy Egg** and **KISSmetrics**.
  These are product/brand context, not persona-voice surfaces.

No Teachable/Kajabi-style paid course catalog is central to his brand (unlike some peers);
his "product" funnel is Ubersuggest + agency services + free content. If a courses page
surfaces at ingest, attribute and ledger case-by-case.

## Enumeration universe — what feeds pipeline/ledger.csv

Ledger population order and dedup precedence (all counts as of 2026-07-14):

1. **@neilpatel YouTube** — 1,178 long-form + 1,284 shorts = **≈2,462 items** (yt-dlp,
   authoritative). Primary corpus; shorts dedup against long-form (`dup-of:<id>`) where a
   short is a cut of a long video.
2. **@MarketingSchoolPod YouTube** — thousands of short daily episodes; **co-hosted**.
   Ingest with mandatory Neil-vs-Eric speaker tags; only Neil turns are persona data. Start
   with a bounded recent window (e.g. last 200) rather than the full back-catalog.
3. **Marketing School podcast feed** (Apple `1138869817` / Spotify `1NulSGKhstJuty8iYPBMo5`)
   — 2,500–3,500 items; only episodes **without** a YouTube match get their own ledger rows;
   the rest L1 `dup-of:<youtube-id>`. Same speaker-tagging rule.
4. **Book** — *Hustle* (2016) — **1 item**, landmark, priority 1, L3 (co-authored — partial
   attribution).
5. **neilpatel.com blog** — thousands of articles, priority-3 long tail; enter the ledger
   only in a dedicated later phase (attribution burden is high — much is staff-written).
6. **External guest appearances** — not yet enumerated here (biography dossier / a later
   phase owns these); each pinned appearance is a high-yield ledger row.

Rough total primary universe: ~2,460 (main YouTube) + a bounded Marketing School slice +
1 book; plus a large conditional blog/podcast long tail.

## Excluded channels (with reason)

- **NP Digital Brasil** — [@neilpatelbrasil](https://www.youtube.com/@neilpatelbrasil) /
  `UCva4ibMVTYRD1ORrdKJloTA`, 22,800 subs (yt-dlp 2026-07-14). **EXCLUDED**: Portuguese-
  language **company** channel (NP Digital's Brazil office), agency-produced, Neil rarely if
  ever on camera. Language-variant company channel, negligible persona value.
- **@marketingschool** — `UCaUOsj3-pX-3GQF9Fl9C-Lg`, **7 subs** (yt-dlp 2026-07-14).
  **EXCLUDED**: parked/dormant handle-squat; NOT the real podcast channel (that is
  `@MarketingSchoolPod`). Zero content value.
- **"Neil Patel - Topic"** (YouTube auto-generated Art Track channel, if present).
  **EXCLUDED**: algorithmic, no original content.
- **@npdigitalglobal / @npdigital** — agency handles; no Neil-fronted long-form corpus
  found under these (2026-07-14). **EXCLUDED** as persona corpus (corporate voice); may be
  cited as company context only.
- **"Neil Patel MD"** and other same-name creators/accounts — **EXCLUDED**: different
  person (physician). Identity-guard rule above.
- Fan/clip/re-upload channels of Neil's content — **EXCLUDED**: not owned, unverified,
  dedup risk.

## Source list

- yt-dlp direct enumeration (channel IDs, video/short counts, subscriber counts),
  2026-07-14.
- [socialblade.com/youtube/handle/neilpatel](https://socialblade.com/youtube/handle/neilpatel);
  [vidiq.com/youtube-stats/channel/UCl-Zrl0QhF66lu1aGXaTbfw](https://vidiq.com/youtube-stats/channel/UCl-Zrl0QhF66lu1aGXaTbfw), 2026-07-14.
- [podcasts.apple.com/.../id1138869817](https://podcasts.apple.com/us/podcast/marketing-school-digital-marketing-and-online/id1138869817);
  [open.spotify.com/show/1NulSGKhstJuty8iYPBMo5](https://open.spotify.com/show/1NulSGKhstJuty8iYPBMo5);
  [marketingschool.io](https://marketingschool.io/), 2026-07-14.
- [amazon.com Hustle](https://www.amazon.com/Hustle-Power-Charge-Meaning-Momentum/dp/1623367166);
  [penguinrandomhouse.com](https://www.penguinrandomhouse.com/books/593084/hustle-by-neil-patel-patrick-vlaskovits-and-jonas-koffler/), 2026-07-14.
- Neil Patel self-reported follower breakdown, [x.com/neilpatel/status/1750956719537332483](https://x.com/neilpatel/status/1750956719537332483), 2024-01-26.
- [neilpatel.com](https://neilpatel.com/) + [/newsletter](https://neilpatel.com/newsletter/) + [/ubersuggest](https://neilpatel.com/ubersuggest/);
  [npdigital.com](https://npdigital.com/); [quicksprout.com](https://www.quicksprout.com/), 2026-07-14.
