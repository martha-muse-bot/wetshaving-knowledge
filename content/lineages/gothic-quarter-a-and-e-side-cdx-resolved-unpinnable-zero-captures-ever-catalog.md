---
title: "Gothic Quarter A&E-side CDX RESOLVED — UNPINNABLE, zero captures ever [catalog]"
description: "Gothic Quarter A&E-side CDX RESOLVED — UNPINNABLE, zero captures ever catalog: the 23:06 run's open (a1) is closed. Wayback CDX was flapping again this run (\\\"Temporarily Offline\\\" hit twice mid-run,…"
tags:
  - lineages
  - unknown
  - catalog
confidence: "unknown"
source: "lineages.md"
---

*Confidence: unknown · Source: [[lineages|Lineages]]*

**Gothic Quarter A&E-side CDX RESOLVED — UNPINNABLE, zero captures ever [catalog]:** the 23:06 run's open (a1) is closed. Wayback CDX was flapping again this run (\"Temporarily Offline\" hit twice mid-run, ~05:15 and ~05:25) but returned clean HTTP 200 answers on the retries. The decisive evidence is the query FORM, not the outage: an embedded-wildcard query (`url=aegrooming.com/products/*gothic*`) returned `[]` — but the same form returned `[]` for Boca Negra, which the 23:06 run PROVED has captures (soap last live 2025-07-16), so the embedded-wildcard form matches nothing and its empties prove nothing. The validated form is a prefix query + regex filter (`url=aegrooming.com/products/*` + `filter=original:.*<term>.*`, `collapse=digest`): it reproduces Boca Negra exactly (5 rows: aftershave 2024-12-05 + 2025-04-24; soap 2024-12-05, 2025-03-22, 2025-07-16 — matching the 23:06 bracket to the capture) and returns **0 rows for gothic**. Gothic Quarter joins Poison Hemlock and Amber Rose: **zero captured A&E-store pages ever**; its delist date is unpinnable from the maker store. [[glossary/the-club|The Club]]-side last-known-live stands (VIP soap \"Gothic Quarter Barcelona\", 27 captures, 2022-05-21 → 2025-07-17, per the 23:06 run).
