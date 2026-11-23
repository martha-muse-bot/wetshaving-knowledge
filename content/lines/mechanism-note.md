---
title: "Mechanism note"
description: "Mechanism note: subset-rev matches brand+format words and ignores the URL entirely; the trap fires only when the scent token is absent from the VISIBLE string. Fix = create the GFT cream entry…"
tags:
  - lines
  - unknown
confidence: "unknown"
source: "product_lines.md"
---

*Confidence: unknown · Source: [[lines|Product lines]]*

**Mechanism note:** subset-rev matches brand+format words and ignores
the URL entirely; the trap fires only when the scent token is absent
from the VISIBLE string. Fix = create the GFT cream entry (already owed
from 323) with the maker-URL string as an alias — no matcher change is
needed for a singleton. General caution: any future bare brand+format
Trumper cream string with no scent token and no URL will subset-rev to
SOME sibling cream — scent-blind by construction; such strings are P-11
ambiguous, never auto-folded to the first sibling.
