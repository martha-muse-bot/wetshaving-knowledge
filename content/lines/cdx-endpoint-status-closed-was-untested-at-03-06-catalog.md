---
title: "CDX endpoint status CLOSED (was untested at 03:06) [catalog]"
description: "CDX endpoint status CLOSED (was untested at 03:06) catalog: CDX answers fine from this sandbox this run (all queries 200). The /web/ 429 bot-flag is endpoint-specific — do not generalize it to CDX.…"
tags:
  - lines
  - unknown
  - catalog
confidence: "unknown"
source: "product_lines.md"
---

*Confidence: unknown · Source: [[lines|Product lines]]*

**CDX endpoint status CLOSED (was untested at 03:06) [catalog]:** CDX answers fine from this sandbox this run (all queries 200). The /web/ 429 bot-flag is endpoint-specific — do not generalize it to CDX. Caveat: the first two /password queries transiently returned HTTP 000 (connection failure) and succeeded on retry — retry once on 000 before declaring a CDX failure.
