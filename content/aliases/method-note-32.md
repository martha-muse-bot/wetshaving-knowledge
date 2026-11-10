---
title: "Method note (aliases 32)"
description: "Method note: a CDX outage mid-run (\"Temporarily Offline\" on the targeted queries while a different query returned clean JSON minutes earlier) is an outage, never a negative — the listing route stays…"
tags:
  - aliases
  - unknown
confidence: "unknown"
source: "product_aliases.md"
---

*Confidence: unknown · Source: [[aliases|Product aliases]]*

**[[lineages/method-note|Method note]]:** a CDX outage mid-run ("Temporarily Offline" on the targeted queries while a different query returned clean JSON minutes earlier) is an outage, never a negative — the listing route stays open and the re-run uses the validated prefix+filter form, not the embedded-wildcard form (which matches nothing).
