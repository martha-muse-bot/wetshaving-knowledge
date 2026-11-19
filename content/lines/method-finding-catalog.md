---
title: "METHOD FINDING [catalog]"
description: "METHOD FINDING catalog — Hand & Body INCIs live in a product METAFIELD, not bodyhtml. The Lavender INCI is rendered from a metafield-richtextfield in an \"Ingredients\" accordion; products.json…"
tags:
  - lines
  - lead
  - catalog
confidence: "lead"
source: "product_lines.md"
---

*Confidence: lead · Source: [[lines|Product lines]]*

**METHOD FINDING [catalog] — Hand & Body INCIs live in a product METAFIELD, not body_html.** The Lavender INCI is rendered from a `metafield-rich_text_field` in an "Ingredients" accordion; products.json body_html for Lavender is 301 bytes (scent copy + "Net Wt. 4.75 oz", no ingredients). The 17:06 run's "live maker body carries NO INCI section for Lavender" was a products.json artifact, not a page fact. The watch snapshots can NEVER show a Hand & Body INCI — formula checks must read the live HTML page's Ingredients accordion. Also explains the 17:06 "inconsistent bodies" note: Bay Rum / Seville / Lavender lack an INCI section in body_html because theirs lives in the metafield. **[[lineages/new-narrow-lead|NEW NARROW LEAD]] (c4-narrow-216):** verify the other five scents' live metafield INCIs match their pinned brackets (Bay Rum, Cologne Russe, Lavanille, LGC, Seville) — one live-page read per scent. **Trap:** never date a metafield edit from products.json `updated_at` — it bumps ~every 2 hours store-wide in lockstep with the watch fetches (verified across all 60+ saved B&M snapshots Nov 12–18), a bulk-update artifact, not an edit signal.
