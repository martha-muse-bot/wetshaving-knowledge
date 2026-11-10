---
title: "CDX flapping log this run (hardware)"
description: "CDX flapping log this run: the sss prefix query hit \"Temporarily Offline\" once; the razor-filtered products query failed once the same way, then returned full data (48 rows) on retry. Outages, never…"
tags:
  - hardware
  - unknown
confidence: "unknown"
source: "hardware_lore.md"
---

*Confidence: unknown · Source: [[hardware|Hardware lore]]*

**[[lineages/cdx-flapping-log-this-run|CDX flapping log this run]]:** the `*sss*` prefix query hit "Temporarily Offline" once; the razor-filtered products query failed once the same way, then returned full data (48 rows) on retry. Outages, never negatives. The full products/* census hit its 2,000-row cap — the 0-slant/0-sss counts there are lower bounds on the crawl, but the targeted filter queries (clean `[]` while other queries returned data) carry the negative.
