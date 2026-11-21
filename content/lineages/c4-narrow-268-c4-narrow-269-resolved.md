---
title: "(c4-narrow-268)/(c4-narrow-269) RESOLVED"
description: "(c4-narrow-268)/(c4-narrow-269) RESOLVED — fetch fixes proven in the wild catalog: the new fetchwatchescl.sh (retry ×3, 30s/60s backoff, temp-file-only writes, 26-file JSON validation) ran clean:…"
tags:
  - lineages
  - unknown
  - catalog
confidence: "unknown"
source: "lineages.md"
---

*Confidence: unknown · Source: [[lineages|Lineages]]*

**(c4-narrow-268)/(c4-narrow-269) RESOLVED — fetch fixes proven in the wild [catalog]:** the new fetch_watches_cl.sh (retry ×3, 30s/60s backoff, temp-file-only writes, 26-file JSON validation) ran clean: EXIT 0, 26/26 valid. SIX first-attempt HTTP 429s — B&M, CL, BlackShip, HoM, NA p1, Maggard p1 — EVERY store's first fetch 429'd, all recovered on attempt 2 (20 first-attempt 200s + 6 second-attempt 200s). No HTTP 000 this run. The 429s cluster on first-per-store fetches (Cloudflare burst gating); the backoff is load-bearing, not precautionary.
