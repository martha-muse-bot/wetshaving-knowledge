---
title: "(388) RESOLVED as NEGATIVE"
description: "(388) RESOLVED as NEGATIVE — the dataset cannot corroborate the Jul 8, 2026 oil reformulation, because there is nothing to narrate from catalog: - Post-Jul-2026 slice: 7,812 rows (threaddate >=…"
tags:
  - aliases
  - established
  - catalog
confidence: "established"
source: "product_aliases.md"
---

*Confidence: established · Source: [[aliases|Product aliases]]*

**(388) RESOLVED as NEGATIVE — the dataset cannot corroborate the Jul 8, 2026 oil reformulation, because there is nothing to narrate from [catalog]:**
- Post-Jul-2026 slice: 7,812 rows (thread_date >= 2026-07-08). Field-level scan (preshave/aftershave/fragrance/other) for "stirling"+"oil": 87 hits, ALL false positives — 56 are "Eau de Toilette" strings ("Toilette" contains the substring "oil"); 31 are dict-typed 'other' fields naming "Natures Oil Witch Hazel" toner. ZERO genuine Stirling beard/pre-shave oil product strings post-Jul-2026.
- Notes scan (stirling + oil in the same note): 24 hits, all false positives (Toilette in duplicated post text, "pine oil", "essential oils", honing oil, "oil" in other-product contexts). ZERO narrate a formula change. Notes scan (stirling + reformulat/new formula/argan/pumpkin/old-vs-new language): 7 hits, all unrelated (pumpkin SCENT notes for Stirling Pumpkin Spice soap, Ingram's reformulation, etc.).
- All-years census of genuine Stirling beard/pre-shave oil product strings ("beard oil"|"pre-shave oil"|"preshave oil"|"shave oil" + "stirling"): 526 total. By year: 2016: 1, 2017: 27, 2018: 168, 2019: 23, 2020: 88, 2021: 60, 2022: 50, 2023: 13, 2024: 3, 2025: 90, 2026: 3. The 3 2026 uses are ALL pre-changeover: 2026-04-10 geneaut "Stirling Campania Shave Oil" (preshave); 2026-05-17 JoelB "Stirling - Island Man" (other/Beard Oil, ×2 rows, same post duplicated).
- Preshave-field population control rules out a parsing artifact: 2025 rows with preshave = 5,255 (295 with "oil"); 2026 rows with preshave = 6,357 (517 with "oil") — oil use in general is UP in 2026 while [[lineages/stirling-oil|Stirling oil]] use collapsed to zero post-changeover. The Jul 8 oil reformulation rests on the maker-side Wayback pair alone (established, (386) run); the dataset cannot corroborate it. Route exhausted for the current dataset — re-open only if a post-Jul-2026 Stirling oil use ever appears.
