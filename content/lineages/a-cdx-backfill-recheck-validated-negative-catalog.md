---
title: "(a) CDX backfill recheck — VALIDATED NEGATIVE [catalog]"
description: "(a) CDX backfill recheck — VALIDATED NEGATIVE catalog: unfiltered CDX for coastfragrance.com (browser task, 2026-11-10 05:10 CST) returns exactly the same 6 records as 2026-11-07 — five 2025-03-20…"
tags:
  - lineages
  - unknown
  - catalog
confidence: "unknown"
source: "lineages.md"
---

*Confidence: unknown · Source: [[lineages|Lineages]]*

**(a) CDX backfill recheck — VALIDATED NEGATIVE [catalog]:** unfiltered CDX for `coastfragrance.com*` (browser task, 2026-11-10 ~05:10 CST) returns exactly the same 6 records as 2026-11-07 — five 2025-03-20 (two 200s + three 301s) + one 2025-07-10 00:36:13 UTC (http, 301, digest OQ3OBNFR7DBCFQ4ANGEQW5P2FOXZZJRA, length 595). No 2026 captures, no product-page captures. First attempt hit IA's "Temporarily Offline" page; the reload returned real data — the negative is validated by the same-batch control rule (a clean return after a flapping failure counts; a lone `[]` does not).
