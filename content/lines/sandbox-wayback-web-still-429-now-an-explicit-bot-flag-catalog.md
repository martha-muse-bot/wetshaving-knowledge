---
title: "Sandbox Wayback /web/ STILL 429, now an explicit bot-flag [catalog]"
description: "Sandbox Wayback /web/ STILL 429, now an explicit bot-flag catalog: the 03:06 retry returned HTTP 429 with \"Your request is being blocked because our system has flagged it as suspected abusive bot…"
tags:
  - lines
  - unknown
  - catalog
confidence: "unknown"
source: "product_lines.md"
---

*Confidence: unknown · Source: [[lines|Product lines]]*

**Sandbox Wayback /web/ STILL 429, now an explicit bot-flag [catalog]:** the 03:06 retry returned HTTP 429 with "Your request is being blocked because our system has flagged it as suspected abusive bot traffic" — two hours after the 01:06 block, not cooled. The live browser hit NO block on the same URL. The /web/ endpoint is a hard stop from this sandbox until the flag lifts; the live-browser route is the working fallback for /web/ reads (CDX was not re-tested this run — do not claim it is blocked or clear).
