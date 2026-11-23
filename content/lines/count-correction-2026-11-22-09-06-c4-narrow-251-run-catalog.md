---
title: "COUNT CORRECTION 2026-11-22 09:06 (c4-narrow-251 run) [catalog]"
description: "COUNT CORRECTION 2026-11-22 09:06 (c4-narrow-251 run) catalog: the census-v2 headline numbers are double-count artifacts — c244census2.py's aliastoentry maps 38 normalized keys to a repeated entry id…"
tags:
  - lines
  - unknown
  - catalog
confidence: "unknown"
source: "product_lines.md"
---

*Confidence: unknown · Source: [[lines|Product lines]]*

**[[lines/count-correction|COUNT CORRECTION]] 2026-11-22 ~09:06 (c4-narrow-251 run) [catalog]:** the census-v2 headline numbers are double-count artifacts — c244_census2.py's alias_to_entry maps 38 normalized keys to a repeated entry id (TTS link + plain form collapsing to one key, etc.) and its counting loop increments per list element. Corrected: total literal-'cream' strings **3,223 → 1,828**; genuine mis-attribution (Class B) **~549 → ~286** (Palmolive stick 245 → 105; DRH 107 → 45; Tabac 39 → 32; Sir Irisch Moos 32 → 16; Nivea balm 59 → 32; Barbasol 1919 balm 9 → 6; AoS Lavender balm 12 → 6; Musgo Real 5 → 3; Olympus 27, Proraso Sensitive bowl 3, Crabtree 3, Lider 8 unchanged). Entries with matches stays 140; the "ZERO cream-form sibling" finding is structural and unaffected. The 244 VERDICT stands — all Class B validator calls stand, same entries, smaller row counts. Full per-entry table: knowledge/work/c244_corrected_counts_2026-11-22.txt; run section below.
