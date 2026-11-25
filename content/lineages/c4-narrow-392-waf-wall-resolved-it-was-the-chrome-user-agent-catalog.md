---
title: "(c4-narrow-392) WAF wall — RESOLVED: it was the Chrome User-Agent [catalog]"
description: "(c4-narrow-392) WAF wall — RESOLVED: it was the Chrome User-Agent catalog: the ek fetch script (Chrome UA) got 403 on B&M, CL, BlackShip; same minute, curl with DEFAULT UA returned HTTP 200 on B&M,…"
tags:
  - lineages
  - unknown
  - catalog
confidence: "unknown"
source: "lineages.md"
---

*Confidence: unknown · Source: [[lineages|Lineages]]*

**[[aliases/c4-narrow-392-waf-wall|(c4-narrow-392) WAF wall]] — RESOLVED: it was the Chrome User-Agent [catalog]:** the ek fetch script (Chrome UA) got 403 on B&M, CL, BlackShip; same minute, curl with DEFAULT UA returned HTTP 200 on B&M, CL, NA p6, Maggard p1, CGC. Fix applied: fetch_watches_ek.sh now uses curl's default UA. All 26 ek files HTTP 200 first attempt, ZERO 429s. Caveat: the ej-run wall may have had a second component (NA/Maggard walled while the other five fetched clean under the SAME Chrome UA) — per-store/per-hour bot scoring varies.
