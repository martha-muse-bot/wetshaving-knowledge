---
title: "(c4-narrow-347) RESOLVED"
description: "(c4-narrow-347) RESOLVED — yes, other numeric clusters exist: 44 brand-less numeric-label entries, and they attract 591 matched rows. Census key: entries whose data-JSON label is a bare number or…"
tags:
  - aliases
  - unknown
confidence: "unknown"
source: "product_aliases.md"
---

*Confidence: unknown · Source: [[aliases|Product aliases]]*

**(c4-narrow-347) RESOLVED — yes, other numeric clusters exist: 44
brand-less numeric-label entries, and they attract 591 matched rows.**
Census key: entries whose data-JSON `label` is a bare number or
number-fraction AND `brand` is null (the `product` column is null for
all of them — label/alias is the only name). The queue already knew:
56 queue refs end in a bare number; soap /1, /3, /4, /5, /6 were
already retired as not_a_product (entries deleted); the rest parked.
