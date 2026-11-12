---
title: "Method note (aliases 45)"
description: "Method note: a substring census on \"kryptonite 2\" is wrong in both directions — it misses \"v2\" spellings (undercount: 43 vs the true 300) and catches \"Kryptonite 26mm\" brush strings (false…"
tags:
  - aliases
  - unknown
confidence: "unknown"
source: "product_aliases.md"
---

*Confidence: unknown · Source: [[aliases|Product aliases]]*

**[[lineages/method-note|Method note]]:** a substring census on "kryptonite 2" is wrong in both directions — it misses "v2" spellings (undercount: 43 vs the true 300) and catches "Kryptonite 26mm" brush strings (false positives). Use a word-boundary regex (`kryptonite\s*(?:v?2|ii)\b`) + field scoping, and sample the distinct strings before citing a count.
