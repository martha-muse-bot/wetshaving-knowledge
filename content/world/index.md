---
title: "World notes"
tags:
  - index
---

**Thread pulled:** (c4-narrow-203) — Blizzard Battles 2026 champion, the oldest unchecked item — plus the standing watch cycle (suffix "ep"), the (389)/(374)/(379)/(220) rechecks, and notes-mining.
**Sources used:** live-browser read of the YouTube final video (uqCPSnitwNQ, browser task e2c737d4, ran 11:11–11:13 CST — transcript panel + top comments); web searches ×2 (champion/winner phrasings — noise only); Shave Dad journal live read (329 articles; latest Nov 24, 2026; no winner post; Oct 6 final is the latest Blizzard Battles entry); dataset full-corpus census (sotd_* only, 242,124 rows, max thread_date 2026-11-24 — 461 new rows since 241,663) + blizzard+win notes scan (8 hits, all false positives); watch snapshots ep (27 files, all HTTP 200 first attempt except HoM — see method note — ZERO 429s) + programmatic diff eo→ep (knowledge/work/watch_diff_eo_ep.py + .txt) + rechecks (knowledge/work/c301_watch_rechecks_ep.py + .txt); TTS cert probe; Relic homepage + sitemap curls; Wayback CDX exact-handle queries (389).

**Facts added:** world_notes.md (this run section [catalog] — (203) resolution + (389) recheck + watches + rechecks); backlog.md (run line; (203) resolved, (389) still open, 0 new leads); learning_log.md (this entry); evidence note knowledge/work/c203_blizzard_champion_2026-11-25.txt; watch snapshots saved to goal hidden_files/watch-snapshots/ — suffix "ep"; diff saved to knowledge/work/watch_diff_eo_ep.py + watch_diff_eo_ep.txt; rechecks saved to knowledge/work/c301_watch_rechecks_ep.py + .txt; fetch script knowledge/work/fetch_watches_ep.sh (+ fetch_ep.log).
**Backlog changes:** 1 resolved ((c4-narrow-203)); 0 new leads. Backlog shorter by one item net ((389)/(374)/(379) still open, plus the older open items listed in prior run lines).
**Reporting:** Routine learning per the charter — no report. The (203) resolution closes a named dataset mystery but changes no catalog work (both finalists are real products either way); the Maggard delistings are sold-out cleanup; no catalog event this run.
**Method notes:** (1) A bare-substring sed on suffixes corrupts store names: `s/eo/ep/g` rewrote "houseofmammoth" → "housepfmammoth" ("houseof" contains "eo"), so HoM 000-failed all 3 attempts this run — the site was fine (direct curl 200, 349,464B); the HoM snapshot was re-fetched by hand and validated 27/27. Never bare-sed suffixes across URLs; use quoted-token replacement (as in the diff/recheck scripts this run). (2) YouTube's timedtext endpoint returning 0 bytes does NOT mean no transcript — the "Show transcript" panel is a separate route and carries the auto-transcript; check the panel before declaring a video verdict text-unreachable. (3) Empty terminator pages (NA p7 / Maggard p14, 15B `{"products":[]}`) are normal — the script fetches one page past the end; do not read delists into them (both were empty in eo too). (4) B&M's bulk updated_at wall clock equals the fetch second in UTC terms (file mtime 17:10:13 UTC = updated_at 12:10:13-05:00) — the per-fetch bulk-touch pattern holds; a shared updated_at is not an edit.

## World notes

- [[world/event-months-on-r-wetshaving|Event months on r/Wetshaving]]
- [[world/weck-sextoblade|Weck Sextoblade]]
- [[world/a77|A77]]
- [[world/razorbladesclub-com|razorbladesclub.com]]
- [[world/cuchiller-a-moreno|Cuchillería Moreno]]
- [[world/declaration-groomings-own-site-can-return-402|Declaration Grooming's own site can return 402]]
- [[world/kismet-hair-shaper-blades|Kismet hair-shaper blades]]
- [[world/independent-mit-licensed-pipeline-over-the-same-r-wetshaving-sotd-data-github|Independent MIT-licensed pipeline over the same r/Wetshaving SOTD data (github.com/nmrs/sotd-pipeline), cloned at]]
- [[world/role-semi-validation-their-correctmatches-yaml-human-confirmed-raw-string-brand|Role: SEMI-VALIDATION. Their correctmatches/.yaml (human-confirmed raw string -> brand+product) and data/.yaml catalogs]]
- [[world/measured-2026-10-20|Measured 2026-10-20]]
- [[world/sync-plan-post-sqlite-weekly-job|Sync plan (post-SQLite): weekly job]]
- [[world/corroboration-rule-user-2026-10-20-refined|CORROBORATION RULE (user, 2026-10-20, refined)]]
- [[world/taxonomy-update-user-2026-10-20-3-distinct-authors-attested-existence|TAXONOMY UPDATE (user, 2026-10-20): 3+ distinct authors = ATTESTED (existence established, name unconfirmed), a fourth]]
- [[world/brand-of-record-user-intent-primacy-user-ruling-2026-10-21|Brand-of-record / user-intent primacy (user ruling, 2026-10-21)]]
- [[world/maggard-razors-is-a-first-check-attribution-source-user-2026-10-21|Maggard Razors is a first-check attribution source (user, 2026-10-21)]]
- [[world/trythatsoap-coms-brand-status-field-is-stale|trythatsoap.com's brand-status field is stale]]
- [[world/storybooksoapworks-com-liveness-unconfirmed-lead-2026-10-22|storybooksoapworks.com liveness UNCONFIRMED (lead, 2026-10-22)]]
- [[world/van-der-hagen-de-blades-made-by-giesen-and-forsthoff-timor-solingen|Van Der Hagen DE blades = made by Giesen & Forsthoff (Timor), Solingen]]
- [[world/astra-superior-platinum-green|Astra Superior Platinum (green)]]
- [[world/astra-superior-stainless-blue|Astra Superior Stainless (blue)]]
- [[world/gillette-minora|Gillette Minora]]
- [[world/hema-dutch-variety-store-house-brand-de-blades-rebranded-personna|HEMA (Dutch variety-store house brand) DE blades = rebranded Personna]]
- [[world/shoebox-shave-shop-shoeboxshaveshop-com|ShoeBox Shave Shop (shoeboxshaveshop.com)]]
- [[world/the-shave-supply-formerly-the-handlebar-supply|The Shave Supply, formerly The HandleBar Supply]]
- [[world/hoffritz-for-cutlery-retailer-identity-established-2026-10-29-catalog|Hoffritz for Cutlery — retailer identity ESTABLISHED 2026-10-29 [catalog]]]
- [[world/airline-amenity-kits-genuinely-included-safety-razors-in-the-golden-age|Airline amenity kits genuinely included safety razors in the golden age]]
- [[world/lather-games-2026-ran-in-october-2026|Lather Games 2026 ran in OCTOBER 2026]]
- [[world/scsurffishing-com-is-dead|scsurffishing.com is dead (world)]]
- [[world/vshod-com|vshod.com]]
- [[world/lathered-expo-brooklyn-2026-catalog|LATHERED Expo, Brooklyn (2026) [catalog]]]
- [[world/schick-edgewell-us-blade-plant-closure-lead-single-podcast-source|Schick/Edgewell US blade-plant closure — LEAD (single podcast source)]]
- [[world/the-holy-black-new-york-texas-lead-single-podcast-source|The Holy Black, New York → Texas — LEAD (single podcast source)]]
- [[world/mitchells-wool-fat-closure-rumor-persists-in-trade-press-verdict-stands|Mitchell's Wool Fat closure rumor — PERSISTS in trade press; verdict STANDS]]
- [[world/schick-edgewell-us-blade-plant-closure|Schick/Edgewell US blade-plant closure]]
- [[world/the-holy-black-new-york-texas|The Holy Black, New York → Texas]]
- [[world/schick-milford-sku-map-established-c4-narrow-144-catalog|Schick Milford SKU map — ESTABLISHED (c4-narrow-144) [catalog]]]
- [[world/blizzard-battles-2026|Blizzard Battles 2026]]
- [[world/champion-still-video-only-c4-narrow-203-catalog|Champion STILL video-only (c4-narrow-203) [catalog]]]
- [[world/triple-dog-dare-origin-established|Triple Dog Dare origin — ESTABLISHED]]
- [[world/method-notes-from-the-final-post|Method notes from the final post]]
- [[world/c4-narrow-203-resolved|(c4-narrow-203) RESOLVED]]
- [[world/c4-narrow-389-rechecked-still-open|(c4-narrow-389) RECHECKED — STILL OPEN (world)]]
- [[world/watches-maggard-sold-out-cleanup-only-eo-ep|Watches — Maggard sold-out cleanup only (eo→ep)]]
- [[world/rechecks|Rechecks (world)]]
- [[world/dataset|DATASET (world)]]
- [[world/notes-mining-slice-2026-11-23|Notes-mining slice ≥ 2026-11-23 (world)]]
- [[world/new-narrow-leads|NEW NARROW LEADS (world)]]
