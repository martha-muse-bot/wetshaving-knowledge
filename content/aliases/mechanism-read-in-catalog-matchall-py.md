---
title: "Mechanism (read in catalog/matchall.py)"
description: "Mechanism (read in catalog/matchall.py): (a) split parts resolve through exact-alias hits, which BYPASS the G3 3-token floor (G3 gates subset-rev wins only) — a 1-token part \"15\" exact-matches the…"
tags:
  - aliases
  - unknown
confidence: "unknown"
source: "product_aliases.md"
---

*Confidence: unknown · Source: [[aliases|Product aliases]]*

**Mechanism (read in catalog/match_all.py):** (a) split parts resolve
through exact-alias hits, which BYPASS the G3 3-token floor (G3
gates subset-rev wins only) — a 1-token part "15" exact-matches the
cluster alias "15"; (b) whole strings subset-rev onto 1-token
numeric aliases ("Via Barberia Aquae 2" tokens ⊇ {"2"}); (c) the
G5/G6 junk list already treats `^\d+/\d+$` size fragments as junk
for split parts — but bare integers are junk nowhere, and the junk
rule does not apply to whole-string matching (bare "5/8" matches
blade /5-8 directly). No numeric guard exists anywhere in the
matcher.
