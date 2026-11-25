---
title: "(c4-narrow-392) WAF wall"
description: "(c4-narrow-392) WAF wall — RESOLVED: it was the Chrome User-Agent, not cadence or IP catalog: the ek fetch script (Chrome UA ...Chrome/120.0) got 403 on B&M, CL, BlackShip — the wall had SPREAD to…"
tags:
  - aliases
  - unknown
  - catalog
confidence: "unknown"
source: "product_aliases.md"
---

*Confidence: unknown · Source: [[aliases|Product aliases]]*

**(c4-narrow-392) WAF wall — RESOLVED: it was the Chrome User-Agent, not cadence or IP [catalog]:** the ek fetch script (Chrome UA `...Chrome/120.0`) got 403 on B&M, CL, BlackShip — the wall had SPREAD to the previously-clean stores. Same minute, curl with DEFAULT UA (no -A) returned HTTP 200 on B&M (306,385B), CL (29,443B), NA p6 (243,598B), Maggard p1 (1,292,031B), CGC (236,222B). The same Chrome UA on CGC got 403 (10,499B challenge page) one minute after a default-UA probe got 200 — UA is the discriminating variable. Fix applied: fetch_watches_ek.sh now uses curl's default UA (flag removed; header comment records the finding). The ek re-fetch: all 26 files HTTP 200 first attempt, ZERO 429s. Caveat: the ej-run wall may have had a second component (NA/Maggard walled while the other five fetched clean under the SAME Chrome UA that night) — per-store/per-hour bot scoring varies; the UA fix is the actionable finding. [[lineages/method-note|Method note]]: if 403s return, re-test with default UA before declaring a wall; never attribute a 403 to cadence without the UA control.
