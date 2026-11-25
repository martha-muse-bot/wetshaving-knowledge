---
title: "Method notes (aliases 8)"
description: "Method notes: (5) A WAF 403 must be re-tested with curl's DEFAULT User-Agent before it is declared a wall — the Chrome UA is itself the trigger on Shopify stores; never attribute a 403 to fetch…"
tags:
  - aliases
  - unknown
confidence: "unknown"
source: "product_aliases.md"
---

*Confidence: unknown · Source: [[aliases|Product aliases]]*

**[[aliases/method-notes|[[lineages/method-note|Method note]]s]]:** (5) A WAF 403 must be re-tested with curl's DEFAULT User-Agent before it is declared a wall — the Chrome UA is itself the trigger on Shopify stores; never attribute a 403 to fetch cadence without the UA control. (6) TBS = The Black Stuff, theblackstuff.com — never thebeardstruggle.com; a zero-overlap diff is the tripwire for a wrong-store fetch, and the vendor field settles it in one read. (7) The ek fetch script's `UA=`/−A removal is now the standing fetch default; if a future run re-adds a browser UA, the wall returns.
