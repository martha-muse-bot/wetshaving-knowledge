---
title: "P-25 — Composite split: a field string joining two or more products splits so each half matches its own entry"
description: "Statement: When one field string joins two or more products — semicolon-joined (\"Alum block; B&M Paganini's Violin\"), plus-joined (\"Wolfman WR1-OC + WRH7\"), or equivalent — the string is split at…"
tags:
  - precedent
  - standing
source: "precedents.md"
status: "standing"
---

*Status: standing · Source: [[precedents|Precedents]]*

**Statement:** When one field string joins two or more products — semicolon-joined ("Alum block; B&M Paganini's Violin"), plus-joined ("Wolfman WR1-OC + WRH7"), or equivalent — the string is split at ingest/matcher level and each half matches its own entry. Composite clusters are not entries, not folds, and not deletions: they exist only until the split routes their rows, then retire. A half that matches nothing does not split off; the string stays whole and keeps matching its own cluster.
**Established by:** User ruling 2026-11-16 (Q006543, tap "Split at ingest/matcher level"), scope extended same day by the user: all fields, including multi-razor posts ("Rockwell 6S - R3 plate ; Fine Slant touchup", "ZY 6/8; Wüsthof Trident Barber's King 6/8").
**Scope measured 2026-11-16:** 13,183 semicolon-join rows across fields (aftershave 4,560; brush 3,152; soap 2,906; razor 1,432; fragrance 1,003; blade 130); alum-led semicolon aftershave class 48 clusters / 422 uses. Plus-join rows measured same day: 7,503 total (aftershave 3,781; brush 1,354; soap 1,293; razor 959; blade 46; fragrance 70) — noisier than ';' ("barrister + mann" is a brand-name spelling, not a join), so the match-guard carries more weight for '+'.
**Design (as specified to the user 2026-11-16):** split at match time in match_all.py, dataset rows untouched; separators ';' and '+' only — never 'and'/'&', which occur inside brand names (Barrister & Mann, Wade and Butcher, "B&M" itself); guard that a part splits off only if it matches a real entry, so prose halves ("...it lathers well; it's slick...") never split; counting: each matched half counts as one use of its product.
**Applied:** 2026-11-16 — Q006543 resolved with this ruling; cluster `unverified/aftershave/alum-block-b-m-paganini-s-violin` stays unverified and matchable until the split lands.

---
