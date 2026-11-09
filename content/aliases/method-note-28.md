---
title: "Method note (aliases 28)"
description: "Method note: an embedded-wildcard CDX query (url=.../products/gothic) matches NOTHING — it returned for Boca Negra too, which provably has 5 captures. The working form is a prefix query…"
tags:
  - aliases
  - unknown
confidence: "unknown"
source: "product_aliases.md"
---

*Confidence: unknown · Source: [[aliases|Product aliases]]*

**[[lineages/method-note|Method note]]:** an embedded-wildcard CDX query (`url=.../products/*gothic*`) matches NOTHING — it returned `[]` for Boca Negra too, which provably has 5 captures. The working form is a prefix query (`url=aegrooming.com/products/*`) with a regex `filter=original:.*<term>.*`. Always run a known-positive control term through a new CDX query form before trusting an empty result — this run's first two \"[]\" answers were form artifacts, and only the control (Boca Negra) exposed it. Also: the Archive was flapping again this run (\"Temporarily Offline\" twice, ~05:15 and ~05:25) — a 503 mid-run is an outage, never a negative result; retry the same query.
