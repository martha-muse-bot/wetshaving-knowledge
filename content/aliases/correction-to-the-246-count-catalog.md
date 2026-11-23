---
title: "CORRECTION to the 246 count [catalog]"
description: "CORRECTION to the 246 count catalog: the 246 \"46\" for Amaretto is a double-count — c246audit.py's aliastoentry maps both normalized literal-'soap' keys to the entry twice (TTS alias + plain alias…"
tags:
  - aliases
  - unknown
  - catalog
confidence: "unknown"
source: "product_aliases.md"
---

*Confidence: unknown · Source: [[aliases|Product aliases]]*

**CORRECTION to the 246 count [catalog]:** the 246 "46" for Amaretto is a double-count — c246_audit.py's alias_to_entry maps both normalized literal-'soap' keys to the entry twice (TTS alias + plain alias collapse to one key; the two "Amaretto - Soap" spellings collapse to the other), and its counting loop increments once per list element: 23 × 2 = 46. Tobacco Flower's 4 is correct. The 246 reverse-direction total corrects 104 → 77 (Amaretto 46 → 23, Catie's Revolution 14 → 10 — Catie's plain aliases collapse to one key mapped twice while its TTS alias normalizes to a separate 'catie 39 s...' key, the `&#39;` surviving norm() as digits "39"; all other 246 entries reproduce exactly). The Speick Men merge call is unaffected (its 4 reproduces exactly).
