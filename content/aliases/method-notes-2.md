---
title: "Method notes (aliases)"
description: "Method notes: (1) When a maker's platform changed, CDX queries must use the ERA's URL space — a Shopify-handle empty proves nothing about the BigCommerce era; check the platform from a homepage…"
tags:
  - aliases
  - unknown
confidence: "unknown"
source: "product_aliases.md"
---

*Confidence: unknown · Source: [[aliases|Product aliases]]*

**[[aliases/method-notes|[[lineages/method-note|Method note]]s]]:** (1) When a maker's platform changed, CDX queries must use the ERA's URL space — a Shopify-handle empty proves nothing about the BigCommerce era; check the platform from a homepage snapshot first. (2) A CDX `[]` is only meaningful with a WORKING CONTROL on the same endpoint in the same run. (3) Shopify collection pages paginate by product count, not alphabet — a scent's page is determined by its letter and the page size (T = page 4 in 2020–2021); fetch the right page, not page 1. (4) Nearest-capture timestamp requests silently resolve to older snapshots — always read the `final=` URL/timestamp, never assume the requested date. (5) Watch-diff scripts: never derive the new suffix from the old by chained sed/replace — the second replacement eats the first (self-diff trap, third occurrence); use a placeholder swap or write filenames explicitly.
