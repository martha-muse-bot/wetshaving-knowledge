---
title: "Query-bug note (method)"
description: "Query-bug note (method): the run's first CDX query returned because it carried three filter=statuscode params — CDX ANDs multiple filters, so no record can be 200 AND 301 AND 302. That empty is a…"
tags:
  - lineages
  - unknown
confidence: "unknown"
source: "lineages.md"
---

*Confidence: unknown · Source: [[lineages|Lineages]]*

**Query-bug note (method):** the run's first CDX query returned `[]` because it carried three `filter=statuscode` params — CDX ANDs multiple filters, so no record can be 200 AND 301 AND 302. That empty is a query artifact, never a negative. Use ONE filter (regex alternation) or no status filter for this check.
