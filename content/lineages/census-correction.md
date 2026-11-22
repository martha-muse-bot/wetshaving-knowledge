---
title: "CENSUS CORRECTION"
description: "CENSUS CORRECTION: the Nov 19 run's \"28 superieur field hits\" is NOT reproducible — corrected counts (raw files only, 241,528 rows, accent-insensitive): 21 rows / 30 occurrences all fields / 19…"
tags:
  - lineages
  - unknown
confidence: "unknown"
source: "lineages.md"
---

*Confidence: unknown · Source: [[lineages|Lineages]]*

**CENSUS CORRECTION:** the Nov 19 run's "28 superieur field hits" is NOT reproducible — corrected counts (raw files only, 241,528 rows, accent-insensitive): 21 rows / 30 occurrences all fields / 19 soap-field occurrences. Method trap: `json.dumps()` escapes 'é' to `\u00e9`, which NFKD cannot strip — normalize raw field values, never the JSON dump.
