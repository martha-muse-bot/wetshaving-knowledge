---
title: "Method correction"
description: "Method correction: the early CDX results this run were wrong-slug artifacts, not IA outages — the first query used the cologne wildcard-prefix form and the control used the wrong LGC slug…"
tags:
  - lines
  - unknown
confidence: "unknown"
source: "product_lines.md"
---

*Confidence: unknown · Source: [[lines|Product lines]]*

**Method correction:** the early `[]` CDX results this run were wrong-slug artifacts, not IA outages — the first query used the `*cologne*` wildcard-prefix form and the control used the wrong LGC slug (`le-grand-chypre-shaving-soap`; the real handle is `le-grand-chypre-special-edition-shaving-soap`, still live in the store). IA did flap once ("Temporarily Offline" on the LGC control query) but recovered; the Cologne Russe exact-URL CDX returned 12 rows in the same session, which validates the query form. Lesson: pin the exact slug from the live store's handle list before calling a CDX empty a negative.
