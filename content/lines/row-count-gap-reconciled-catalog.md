---
title: "ROW-COUNT GAP RECONCILED [catalog]"
description: "ROW-COUNT GAP RECONCILED catalog: the 410-row gap is explained — the 05:06–11:06 runs' glob was sotd (which includes sotdweek2026-10-13to2026-10-19.json = exactly 410 rows), while the 13:06 run used…"
tags:
  - lines
  - unknown
  - catalog
confidence: "unknown"
source: "product_lines.md"
---

*Confidence: unknown · Source: [[lines|Product lines]]*

**ROW-COUNT GAP RECONCILED [catalog]:** the 410-row gap is explained — the 05:06–11:06 runs' glob was `sotd_*` (which includes `sotd_week_2026-10-13_to_2026-10-19.json` = exactly 410 rows), while the 13:06 run used `sotd_*_full.json` only (241,198). Per-file counts re-verified this run, identical to 13:06 (2016: 9,544; 2017: 17,488; 2018: 15,441; 2019: 22,045; 2020: 29,267; 2021: 31,542; 2022: 28,304; 2023: 25,028; 2024: 23,206; 2025: 22,135; 2026: 17,198). The `matched_*.json` files mirror the full files exactly (same counts — same row sets). The week file's rows are already inside sotd_2026_full.json, so including it double-counts: **canonical corpus = sotd_*_full.json only, 241,198 rows, max thread_date 2026-11-12.** Future runs: use the `_full` glob and cite 241,198; the 241,608 figure is retired as a double-count.
