---
title: "(c4-narrow-93) RESOLVED"
description: "(c4-narrow-93) RESOLVED — the discrepancy is a URL-form artifact, not a data conflict catalog: the Nov 23, 2015 08:05 first captures are the COLLECTION-variant URLs, and they are real 200s:…"
tags:
  - lines
  - unknown
  - catalog
confidence: "unknown"
source: "product_lines.md"
---

*Confidence: unknown · Source: [[lines|Product lines]]*

**(c4-narrow-93) RESOLVED — the discrepancy is a URL-form artifact, not a data conflict [catalog]:** the Nov 23, 2015 08:05 first captures are the COLLECTION-variant URLs, and they are real 200s: `/collections/holiday-collection/products/le-grand-chypre-special-edition-shaving-soap` captured **2015-11-23 08:05:25** (200, digest MOAYRX22L4NVNQ7KJRSQANVDF5KNFWKA, 14,360 bytes) and `/collections/new-stuff/products/le-grand-chypre-special-edition-shaving-soap` captured **2015-11-23 08:05:38** (200, digest ZBNRFNQT255WMTZUS222SYXUKDDOV5LS, 14,334 bytes). The two digests differ — collection-chrome difference, same product content. The PLAIN `/products/le-grand-chypre-special-edition-shaving-soap` URL was NEVER captured as a 200: uncollapsed exact-URL query (www and non-www return identically — CDX normalizes the host) shows exactly three Nov–Dec 2015 captures, all 404s (Nov 26 02:33; Dec 3 03:37; Dec 3 06:27 with trailing `?`). The domain-wide catch-all confirms the complete soap-slug inventory for Nov–Dec 2015: the two Nov 23 collection 200s, the Nov 26 + Dec 3 plain-URL 404s, one Dec 3 cyber-monday-2015 404, Dec 24 collection-variant 404s, and the Nov 26 .oembed 404 — nothing else. Session validated: the Nov 23 08:06:10 splash-page 200 (`le-grand-chypre-limited-edition-alcohol-aftershave-splash?`) returned in the same queries, so the session was not flapping. **The 07:06 run's collapsed query was correct for the URL it asked — it asked the wrong URL form.** The backlog's "first captures Nov 23, 2015 08:05 (collection variants, 200)" was correct all along; the "sold out within ~3 days" reading stands (plain URL 404 by Nov 26). **Method rule:** a collapsed exact-URL CDX query answers only for that exact URL — Shopify collection-variant URLs (`/collections/<name>/products/<slug>`) are SEPARATE urlkeys with their own capture histories; always run the collections filter + domain-wide catch-all before concluding a Shopify product page was never captured live.
