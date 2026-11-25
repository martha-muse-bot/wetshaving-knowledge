---
title: "Method notes (aliases 4)"
description: "Method notes: (1) A Wayback wildcard on stirlingsoap.com/<prefix> matches only the flat BigCommerce URL space — Shopify product URLs carry /products/ between host and handle, so the same wildcard…"
tags:
  - aliases
  - unknown
confidence: "unknown"
source: "product_aliases.md"
---

*Confidence: unknown · Source: [[aliases|Product aliases]]*

**[[aliases/method-notes|[[lineages/method-note|Method note]]s]]:** (1) A Wayback wildcard on `stirlingsoap.com/<prefix>*` matches only the flat BigCommerce URL space — Shopify product URLs carry `/products/` between host and handle, so the same wildcard does NOT cover Shopify handles; query each platform's URL space separately. (2) A 0-byte CDX file (curl http=000) is a failed connection, never an empty result — the first (376) wildcard attempt failed this way; the retry with a healthy control is what makes the single-row result citable. (3) The CL price check in the diff script now matches on handle/token (fixed per the (373) method note) — Confluence/La Petite Prairie $75 print correctly. (4) Watch-snapshot scans across all 1,569 Maggard files are slow and noisy — when checking one product's history, glob by date-suffix and sample, don't dump every file.
