---
title: "Baili model-code normalization rules (2026-10-23; full analysis in hardwarelore.md)"
description: "catalog Baili model-code normalization rules (2026-10-23; full analysis in hardwarelore.md). The matcher should normalize Baili razor strings as: prefix (BR/BD/BT, in either letter order) + number;…"
tags:
  - aliases
  - unknown
  - catalog
confidence: "unknown"
source: "product_aliases.md"
---

*Confidence: unknown · Source: [[Product aliases]]*

**[catalog] Baili model-code normalization rules (2026-10-23; full
analysis in [[Hardware lore]]).** The matcher should normalize Baili
razor strings as: prefix (BR/BD/BT, in either letter order) + number;
match on the NUMBER. Observed code variants to fold: "BD179"/"BR179"/
"DB179" (transposed-prefix typo, B&B 651308 #29) → Baili 179;
"BD176"/"BR176"/"BAILi BR 176" → Baili 176; "BD191"/"BR191" → Baili
191; "BR131"/"BT131" → Baili 131; "BR171"/"BT171" → Baili 171;
"BR279"/"DB279" → Baili 279 (the butterfly/TTO — RESOLVED 2026-10-27,
[[Hardware lore]]; 279 ≠ 179, never fold into the 179 butterfly);
"BR172"/"BR72" (Chiseled Face's own product copy writes "BR72" once
for their BR172 listing — a retailer typo, not a model). "Bailin
Gongfu" (17 dataset hits, 2020–2026) is almost certainly Baili +
joke, not a product — flag, do not create an entry. "Baili - Super
Blue (BP003)" = the Super Blue DE blade SKU (BP = blade line); BP003
is a blade, never a razor. "Baili 171 head on Timeless Titanium Crown
Handle" = a BR171 head parted onto a Timeless handle (hardware mixing
— the head is Baili 171).
