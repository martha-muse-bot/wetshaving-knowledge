---
title: "Method notes (aliases 2)"
description: "Method notes: (1) A CDX is only meaningful with a WORKING CONTROL in the same run — this run had controls healthy before AND after a mid-run flap (503/000), which is what makes the (369)/(370)…"
tags:
  - aliases
  - unknown
confidence: "unknown"
source: "product_aliases.md"
---

*Confidence: unknown · Source: [[aliases|Product aliases]]*

**[[aliases/method-notes|[[lineages/method-note|Method note]]s]]:** (1) A CDX `[]` is only meaningful with a WORKING CONTROL in the same run — this run had controls healthy before AND after a mid-run flap (503/000), which is what makes the (369)/(370) empties citable; a flap window in between does not void them when the controls bracket it. (2) A failed curl connection writes a 0-byte file, not `[]` — a 3-byte `[]` file is a genuine empty CDX response; check file sizes before trusting a batch. (3) Accent + hyphen traps in watch rechecks: B&M titles carry "Fougère" (NFKD-normalize before matching) and handles use hyphens, so a spaced substring like "fougere gothique" matches neither — normalize and match on single tokens or handles.
