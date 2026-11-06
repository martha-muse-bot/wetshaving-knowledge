---
title: "Glossary mining: extract short ALL-CAPS tokens and nickname patterns from raw dataset strings; expand or flag"
description: "Glossary mining: extract short ALL-CAPS tokens and nickname patterns from raw dataset strings; expand or flag ambiguous. PASS COMPLETED 2026-10-30 08:15 CDT (glossary.md): full ALL-CAPS token census…"
tags:
  - question
  - open
source: "backlog.md"
---

*Status: open · Source: [[Open questions]]*

Glossary mining: extract short ALL-CAPS tokens and nickname patterns
from raw dataset strings; expand or flag ambiguous.
**PASS COMPLETED 2026-10-30 ~08:15 CDT ([[Glossary]]):** full ALL-CAPS
token census over sotd_2016–2026_full.json (6,624 distinct tokens).
~45 expansions recorded, incl. 5 new AMBIGUOUS warnings: SS
(blade/hardware: Super Stainless vs Stainless Steel vs Super Speed vs
Feather AC SS; soap: Strop Shoppe vs Sudsy Soapery — resolve per-scent),
SC (Gillette Short Comb vs Soap Commander), AA ([[glossary/austere-august|Austere August]] vs Karve
AA plate vs possible SW Autumn Ash), SHD (Maggard Super High Density
knot vs Pearl SHD-42 razor), plus DdT solved (= Delor de Treget, the
[[lineages/chatillon-lux|Chatillon Lux]] × Sudsy Soapery collab scent; CL's own aftershave exists
too — P-16 joint-credit applies), TTS solved (= TryThatSoap; "TTS 2.0"
is the DG×TTS data-driven scent, a real product), FOF solved (= Feats
of Fragrance), MOAR solved (= Zenith r/Wetshaving MOAR BOAR 31mm),
Austere August/Sample September/TabOktoberfest/GRUME challenge terms,
BBS/DFS/CCS ratings, WTG/XTG/ATG passes, and ~20 brand abbreviations
(CB, PAA, WCS, SOC, APR, TOBS, SV, RR, EJ, WSP, TSM, ATT, MLS, SW, AP,
DS, GC, CG, MR, SI, SP, SB, GSB, STF, HMW, YRP). CORRECTION folded in:
"Delor de Treget" is NOT Strop Shoppe (see DdT entry). [[aliases/method-note|Method note]]:
author-scoped abbreviations (Eighchops's DdT) resolve via the author's
other posts, not the dictionary. Re-run the census periodically —
new tokens arrive with new makers/challenges.
NEW NARROW LEADS: (a) XSE expansion (Zenith unbleached-boar code —
yourshaving product copy or Zenith factory sheet may spell it out);
**RESOLVED 2026-10-31 — functionally (see [[Glossary]] XSE entry)
[catalog]:** XSE = Zenith's unbleached-boar variant suffix (factory
code, NOT an acronym — no source spells out the letters). Every XSE
model is unbleached (80B XSE per Sharpologist "natural (light brown)
boar"; 506U XSE / 507U XSE per B&B 615177; YourShaving's 2021 "new
Zenith Unbleached boars" = the XSE line). Code decode: U = olive-wood
handle (Gentle Shave cross-ref M5/M11), B = boar-family code, ALL =
aluminum (bleached contrast model = 506ALL SE — SE marks the bleached
variant). Do NOT read XSE as "eXtra Soft" (unbleached Zenith = "the
stiffest scrubbiest boars around," B&B 577997; XS/"E.S." = extra soft
lives in the horse line). NEW LEADS: (a1) the 80N vs 80B split —
RazoRock Blondie is a rebranded Zenith 80N (B&B 648179), salononline
sells the 80B cream handle — what does N vs B denote?; (a2) "SE" scope:
does SE appear on non-aluminum bleached Zeniths, or is SE always the
bleached counterpart to an XSE model?
(a3) the Zenith N/B handle-color split — 80N XSE vs 80B XSE are BOTH
unbleached; N = black resin is established (cross-ref "507/N/L" =
Black Resin), and B ≈ white/cream handle (B&B 615177's "white plastic
handled" 80B XSE; salononline "80b Cream Handle"). LEAD: B = bianco /
N = nero (Italian color codes)? One maker-side or Italian-retailer
confirmation would firm it; do NOT cite it until then.
**RESOLVED 2026-10-31 ~12:10 CDT ([[Glossary]] XSE addendum) [catalog]:**
(a1) 80B vs 80N = HANDLE split, not knot split — the 80-series is the
big Zenith boar (~27mm x 64mm); 80B = cream/white handle, 80N = black
handle; both take XSE (unbleached) and SE (bleached) knot suffixes.
RazoRock Blondie = rebranded 80N (folded as rebrand alias; recorded in
[[Product aliases]]). (a2) SE is LINE-WIDE, not aluminum-only — 625
dataset SE strings across 20+ models, poster-explicit "bleached" twice
(505BC SE x32, 506C SE x2), across olivewood/cobalt/kintsugi/black-
resin/aluminum/cream handles. (a3) full anatomy ESTABLISHED by
correlation: two orthogonal axes — HANDLE letter (B = bianco
cream/white plastic, U = ulivo olive wood, N = nero black resin,
ALL = aluminum; via salononline "80b Cream Handle", B&B 615177,
B&B 621043 507N XSE black-resin line, Sharpologist) + KNOT suffix
(SE = bleached, XSE = unbleached; the X in XSE still unexpanded).
**Catalog rule:** bare "Zenith 80B" carries the handle letter (certain)
but no knot suffix — never read bleached/unbleached from the bare code;
P-17: one 80-series entry, handle + knot as attributes. NEW LEADS:
(a4) does a bleached-knot 80B retail SKU exist (or is the 80 family
unbleached-only now)? — resolves the bare-"80B"-era (2021-2023)
question;
**RESOLVED 2026-11-01 — NEGATIVE: no bleached-80B SKU exists (see
[[Hardware lore]] Zenith run + [[Glossary]] XSE addendum) [catalog]:**
zero "80B SE" strings in the full 2016–2026 corpus; The Gentle Shave's
Zenith code cross-reference (read live 2026-11-01) carries no 80B SE
row; Sharpologist's own bleached counterpart to the 80B XSE is the
**B08-A26** (aluminum handle) — the bleached 80-style brush lives in
the B-series. The 80-series is unbleached-only at retail: bare "80B"
(2021–2023) = the unbleached product's early/unsuffixed naming.
CORRECTION to the (a1)/(a2) resolution above: the "both take XSE and
SE" phrasing was overstated — both take XSE; neither has an SE SKU.
(a5) 505CB (Kintsugi) vs 505BC (Cobalt Blue) — pin the C/B
distinction;
**RESOLVED 2026-11-01 as DISTINCT, letter-decode of CB unpinned
([[Hardware lore]] Zenith run) [catalog]:** 505CB ↔ Kintsugi
(poster-attested "Zenith Kintsugi 505CB SE" ×2; all 49 CB hits SE,
2021–2022 + 2 in 2025); 505BC ↔ Cobalt Blue (poster-explicit "28mm
Bleached Boar" ×32; 261 hits 2021–2026, some as loose re-knotting
knots). Two codes, two handle names, non-overlapping profiles —
established distinct; do NOT expand the CB letters (no source).
NARROW LEAD: a Kintsugi-505CB retailer listing would pin the CB
decode. (a6) horse-line codes — 205WEN, XS/E.S. expansion attempts.
**RESOLVED 2026-11-01 ([[Hardware lore]] Zenith run) [catalog]:** XS =
"Extra Soft" horse — poster-explicit ("506 N XS (extra soft horse)"
×36) + decoder E1–E3 "Horse E.S." rows; horse families = E1–E3
(extra-soft), H1–H8 (standard), M (Manchurian), N (NSint synthetic),
P (silvertip "Extra"), S (TS synthetic), T (best badger "TP").
**205WEN = NEW-205 wenge-wood-handle boar, 24×47, SE = bleached**
(decoder B17/B24 + Gerry7070's own "bleached 205WEN" ×9, 2026) — it
is a BOAR, correcting this item's horse-line misfiling. All 35 corpus
hits are Gerry7070's brush. **WARNING: XS (horse) ≠ XSE (boar) —
one letter apart, opposite axes; never conflate.**
CORRECTION to the (a3) anatomy above: N = nero (black, holds) and
A = white ("barber white" 506A, decoder-verified) — but B is the
80-series' cream/white PLASTIC handle letter, NOT "bianco" (the
decoder never glosses B as a word); drop the bianco claim until a
maker source says it. Master decoder = The Gentle Shave's Zenith code
cross-reference (read live 2026-11-01): model numbers are size
families (205=24mm, 502=24.5mm, 506/507=27–27.5mm, 505=28mm,
508=31mm). Method note: retailer code-cross-reference pages are a
first-class hardware-lore source.
(b) "Wolf Whiskers ST" — assistantpigkeeper's other posts may name
the shape;
**RESOLVED 2026-10-31 as UNEXPANDED (see [[Glossary]] ST entry):** his
other 345 brush strings name no shape; the maker's live 60-shape
catalog (wolfwhiskers.com/handle-shapes, read 2026-10-31) has no "ST"
(closest = "TSE"); scope = 67 hits, ALL assistantpigkeeper 2016 —
single-author pet label, never auto-apply. Caveat: the lineup has
churned since 2016, so absence today doesn't prove ST never existed;
no source attests it as a maker shape. NEW LEAD: Wayback the
2016-era wolfwhiskers.com shape gallery — was "ST" ever a listed
shape (or an early TSE spelling)?
(c) "SS Cola" (Eric--M 2017) — Strop Shoppe LE? Sudsy
Soapery? or Wickham Club Cola in the "SS" (Super Smooth) formula?
**RESOLVED 2026-10-31 as Sudsy Soapery Cola, author-scoped lead
([[Glossary]] SS entry + [[Product aliases]]) [catalog]:** author's
other 2017 strings are full-form "Sudsy Soapery"; Sudsy Soapery Cola
is real (TTS collection 884; full-form attestation from 2018); zero
Strop Shoppe Cola products exist (brand closed ~2016). Wickham's
Super Smooth base postdates 2017. Fold into the Sudsy Soapery Cola
entry as Eric--M's abbreviation; never generalize to other "SS"
strings. NEW LEAD: Sudsy Soapery Cola launch date — was Eric--M's
Aug 2017 string the first dataset use?
(d) SW "AA" = Autumn Ash — needs a second author before it leaves
"possible".
**STILL POSSIBLE 2026-10-31 ([[Glossary]] AA entry):** full-corpus scan
found NO second author for "Southern Witchcrafts - AA" (JohnB413,
2018; his other 2016–2020 posts never spell out the scent). AND the
AA namespace is now three-way-plus: AA Shaving (brand, 2022–2026,
many authors — Oak Ash Thorn, The Hunt, Gale, Moonlight, Wapiti),
Austere August (challenge), Karve AA plate, AA Men (grooming brand).
Bare "AA" post-2022 is dominated by the AA Shaving brand and the
challenge, NOT Autumn Ash — the ambiguity warning is now structural,
not just a caution.
