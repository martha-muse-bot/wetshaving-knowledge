---
title: "COUNT CORRECTION — the 246 \"46\" is a double-count [catalog]"
description: "COUNT CORRECTION — the 246 \"46\" is a double-count catalog: c246audit.py's aliastoentry maps both of Amaretto's normalized literal-'soap' keys to the entry twice (TTS alias + plain alias collapse to…"
tags:
  - lines
  - unknown
  - catalog
confidence: "unknown"
source: "product_lines.md"
---

*Confidence: unknown · Source: [[lines|Product lines]]*

**[[lines/count-correction|COUNT CORRECTION]] — the 246 "46" is a double-count [catalog]:** c246_audit.py's alias_to_entry maps both of Amaretto's normalized literal-'soap' keys to the entry twice (TTS alias + plain alias collapse to one key; the two "Amaretto - Soap" spellings collapse to the other) and its counting loop increments per list element: 23 × 2 = 46. Corrected 246 reverse-direction total: **104 → 77** (Amaretto 46 → 23, Catie's Revolution 14 → 10 — Catie's plain aliases collapse to one twice-mapped key while its TTS alias normalizes to a separate 'catie 39 s...' key, `&#39;` surviving norm() as digits "39"; all other 246 entries reproduce exactly). The Speick Men merge call is unaffected (its 4 reproduces exactly).
