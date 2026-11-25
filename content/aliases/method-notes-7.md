---
title: "Method notes (aliases 6)"
description: "Method notes: (1) Substring \"oil\" matches \"Toilette\" — any Stirling-oil field scan must require \"beard oil\"/\"pre-shave oil\"/\"preshave oil\"/\"shave oil\", never bare \"oil\", or EdT strings flood the…"
tags:
  - aliases
  - unknown
confidence: "unknown"
source: "product_aliases.md"
---

*Confidence: unknown · Source: [[aliases|Product aliases]]*

**[[aliases/method-notes|[[lineages/method-note|Method note]]s]]:** (1) Substring "oil" matches "Toilette" — any Stirling-oil field scan must require "beard oil"/"pre-shave oil"/"preshave oil"/"shave oil", never bare "oil", or EdT strings flood the results. (2) The chained-sed trap struck again in this run's diff-script build (eg→eh then eh→ei in one sed chain self-diffed both sides to ei) — the placeholder-swap rewrite fixed it; the diff script's own assert would have caught it, but write old/new filenames explicitly from the start. (3) A CDX [] for a handle with known pre-window captures is meaningful (empty window, not a dead query) — but only after verifying the handle against the live catalog; the first (389) attempt used wrong handles and would have reported the same [] for the wrong reason.
