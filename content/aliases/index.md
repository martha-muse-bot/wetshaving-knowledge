---
title: "Product aliases"
tags:
  - index
---

**Observed misspellings** (mined from the datasets; extend as found):
posters' misspellings of known products belong here as
typed-string → meant-product pairs, so the matcher can learn them.
(Section seeded 2026-10-20; population is the learner's job.)

**"Aion" has been a scent, a base name, and then a brand — in that
order.** Fold nothing blindly; the DATE disambiguates.

---
**Method (reusable):** normalized (ASCII-folded, lowercased, punctuation-stripped)
unmatched dataset strings (match = null or `unverified/`-prefixed, 2016–2026
matched files, 73,273 distinct) with ≥2 uses, compared by blocked Levenshtein
(same first letter, length ±3, distance ≤2/3) against 31,088 verified
catalog name strings (product + "brand product" + brand + aliases +
loose_aliases). 1,480 near-miss pairs; top 170 manually reviewed this run.
Script: knowledge/tools/misspell_mine.py, candidates: knowledge/tools/misspelling_cands_2026-11-02.json.
Counts below = post-level uses across 2016–2026 (all fields).
**ESTABLISHED typed→meant pairs** (add as aliases/typo-aliases; none recorded before):

**FALSE-MATCH GUARD (the near-miss-model-number trap) [catalog]:** edit distance
will happily "correct" real model numbers into wrong products. Confirmed this
run — these are REAL products, never typo-aliases of the near neighbor:

**LEADS (recorded, not established — resolutions 2026-11-02 ~05:40 CDT run appended below):** ~~"Parker 111W" (23u, 1 author, zero web presence) = probable typo of Parker 111B~~ — **RESOLVED: REAL PRODUCT** (white-handle butterfly; full entry hardware_lore.md). "House of Mammoth - Cirrus" (32u, 1 author) = possible "Cerberus" misspelling; "Missoni" (20u, 1 author) = possible RazoRock Mission shorthand; ~~"Persona Super" (21u/5a) = likely Personna Super Stainless but the exact variant is unpinned~~ — **RESOLVED: Personna Super Stainless (USA)** (putneycj "USA made" pin; the miner's Comfort-Coated/Lab-Blue guess was wrong); ~~"Grooming Dept Otium" (29u) = miner falsely matched Aion Unum — the real referent unpinned~~ — **RESOLVED: REAL GD scent** (multi-author + trythatsoap links + B&B attestation); ~~"Merkur Super" (49u/7a, razor field) = unpinned (Futur?)~~ — **RESOLVED: BLADE-field shorthand for Merkur Super Platinum** (the prior run's field attribution was wrong — all 49 strings are blade field); "Kai SS" (27u) = SS ambiguity (Super Stainless vs Stainless Steel — never auto-apply); "Black Beauty" (28u/8a) = ambiguous (Gillette Black Beauty adjustable vs scent strings; miner's RazoRock Black Bay match unconfirmed); "Via Barberia Aquae 2/4" (23u/22u) = numbered variant unpinned; "Herod" (16u/6a) / "Rhino" (14u/6a) = unconfirmed shorthand; "Chatillon Lux YRP/GLS" = author-scoped abbreviations, unresolved.
**Method:** dataset greps over matched_2016–2026.json (240,688 posts) for each leftover string + author-scoped checks + catalog.db cluster reads + 2 web searches. All five items resolved; item (a) (next-200 review) stays open.
**ESTABLISHED (all [catalog] unless noted):**

**Methodological notes:**

Companion to the lineages.md Hoffman's deep-dive (this run);
closes backlog lead (c) and records naming-traps.

## Product aliases

- [["Lab Blue"]]
- [[Wizamet Super Iridium ≠ Polsilver Super Iridium]]
- [[GEM Platinum Diamond Glide is a DOUBLE-EDGE blade]]
- [[Wolfman WR3 = GEM-format head; WR4 = Artist Club head]]
- [["Sticky" = community nickname for Wilkinson Sword's 1960s DE razor (not a model name, not the modern Classic)]]
- [[Bare-name conventions]]
- [[The recency trap (methodological, 2026-10-21). When a dataset string matches NO known product, check for a]]
- [["BBS-0" = Personna "New Angle 70" (community nickname, 2026-10-21)]]
- [["Amazlenut (B&M)" → Barrister and Mann "Amazelnut" (2026-11-01)]]
- [["Duxham Duplex shavette" → Durham Duplex (2026-10-29)]]
- [["Personna Specimen Prep (Blade)"]]
- [[Baili model-code normalization rules (2026-10-23; full analysis in hardwarelore.md)]]
- [["Kismet" = German hair-shaper blade brand (2026-10-21)]]
- [[NAME COLLISION]]
- [[Kismet MAKER ATTRIBUTION — RESOLVED (2026-10-22)]]
- [["Personna travel" is a descriptor, NOT a product]]
- [["Gillette Airline Tech" is a coined provenance descriptor, NOT a product (RESOLVED 2026-10-29). wegian]]
- [[kismett hair shaper]]
- [[kismet hai shaper]]
- [[B&M "Spice" naming trap]]
- [[Tatra ≠ Tatara (naming trap, established 2026-10-21)]]
- [[The Gillette "Blue" blade family — FOUR distinct products share one name space]]
- [[Dapper Dragon Soaps "Ouroboros"]]
- [["Beaver Woodwright"]]
- [["Bandit" collab cluster]]
- [[Chatillon Lux observed misspellings (mined 2026-10-21)]]
- [[Wholly Kaw spelling variants (mined 2026-10-22)]]
- [["Wax Pass" was u/j-mt's pre-Bufflehead sampling phase, NOT a brand]]
- [["Grooming Dept / MAOL - Frankenlime"]]
- [["primos"]]
- [[House of Mammoth "Indigo" = renamed "Mood Indigo" (2021→early 2022)]]
- [[Stirling "Kaboom" → "Deton-8" (rename, 2019)]]
- [[Zingari Man "The Gypsy"]]
- [[Catie's Bubbles "Blugere" = renamed "Jersey Blues"]]
- [[Dusy Kabinett = Klar Kabinett reincarnated]]
- [[Noble Otter "Hamam" = renamed "Hamami"]]
- [[Lord "Tajam" (Egypt) = Lord Platinum regional rebrand (RESOLVED 2026-10-30]]
- [["The Handlebar Supply" ≠ Ethos Grooming Essentials (caution, 2026-10-22; CORRECTED 2026-10-26]]
- [[The Cornfed Viking]]
- [[Maker's own announcement (2025-01-25): old story names → new note+number names. Canonical = the NEW name; old name =]]
- [[SIX LASSCo scents live on as Chiseled Face products (lineage in lineages.md), in two waves. They are CONTINUATIONS]]
- [[Matcher guidance: bare "Black Rose" soap strings need brand + date to disambiguate (LA pre-2021; CF 2021-04-13+; "The]]
- [[CORRECTION (2026-11-01)]]
- [["Through the Fire Fine Crafts" (plural, ttffcrafts.com, 2024+) = "Through the Fire Fine Craft"]]
- [[2019–2021: a SCENT]]
- [[2020–2023: the base's other name]]
- [[2023+: the brand/line]]
- [[Reverence / Revenance (Aion Skincare scent)]]
- [["SMdF"]]
- [["Crystal" vs "Israeli Reds" vs "Israeli Personnas"]]
- [["Faux Fusion" = rebranded Dorco Pace 6+ (lead, 2026-10-24)]]
- [["Faux Fusion" RESOLVED 2026-10-25]]
- [["Pinaud", "Clubman", and "Pinaud Clubman" are ONE brand group (the US Clubman line, now owned by American International]]
- [["Big Ben" is TWO products, split by FIELD, never by name]]
- [["SIR" = "Sir"]]
- [["Mäuer & Wirtz" (missing the second r) is a pervasive dataset typo]]
- [[Dupe caution]]
- [[Kent SB2]]
- [[FALSE FRIEND: "Kent of Inglewood" is NOT Kent Brushes]]
- [["Kent cream" / "Kent Shaving Cream" strings]]
- [[REJECTED rebrand: Bluebeard's Revenge]]
- [["Enders' Dollar Razor"]]
- [["Christy" / "Christy SE" → Christy Co. Massage Bar SE, NOT Enders]]
- [["Enders by Christy" (no dataset strings yet) → Enders Speed family]]
- [[CORRECTION of a standing backlog guess]]
- [["Hoffman's Broken" = rebranded "Burn the Ships"]]
- [[Catalog guidance [catalog] (aliases)]]
- [[New leads]]
- [["Florena" bare strings are NOT Nivea]]
- [[Method note (the refinement pattern)]]
- [["SS Cola" → Sudsy Soapery Cola (author-scoped abbreviation, lead)]]
- [[RazoRock "Blondie" = rebranded Zenith 80N (established, community)]]
- [[Antica Barbieria Colla (ABC) boar ≈ Zenith B03-A26 ("Zenith B2") (aliases)]]
- [["Gillette Astra" is one author's styling, not a product line]]
- [[B&B auto-censors "A.S.S." — read "]]
- [["Astra Blue" bare / "(Blue)" / "[Blue]" / "blue-pack" = the Superior Stainless]]
- [["TASS" = The Artisan Soap Shoppe]]
- [["HEMA" DE blades = private-label Personna made in Israel]]
- [["Vokshod" (166u/40a) + "Voshkohd" (17u)]]
- [["Persona" (116u/10a, cartridge/blade fields) → Personna (brand-level; the matched target was Twin Pivot Plus]]
- [["Perssona Blue" (53u)]]
- [["Merker 34C HD" (74u) + "Mercur 34C" (15u/2a) + "Merkur MK23C" (14u) → Merkur 34C]]
- [["Mhule R89" (20u)]]
- [["Gilette Minora Stainless" (28u/2a), "Gilette 7 O'clock (Green)" (27u) → Gillette Minora Stainless]]
- [["Gillette Platinium" (20u) + "Gillette Platinun" (18u)]]
- [["Shick Injector" (21u/4a)]]
- [["Bolanzo" (14u)]]
- [["Saponificio Vatesino - 70th anniversary - Soap" (31u)]]
- [["Chatillion Lux Pure Lavender." (25u)]]
- [["Chanel – Bleau de Chanel"]]
- [["Pinuad - Clubman Aftershave Lotion" (33u)]]
- [["Rapira Swedish Super Steel" (28u/2a)]]
- [["Stirling Rambling Man" (49u/2a)]]
- [["Personna hairshaper" (16u)]]
- [["Pol Silver" (48u/12a) + "Pol-Silver SI" (15u/2a)]]
- [["AcuTech Pro" (15u)]]
- [["BBYSMOOTH" (16u)]]
- [["ATT SE1" (76u/9a) → Above the Tie S1 Slant]]
- [["Barrister & Mann - Lavender Interupted" (37u)]]
- [["Southern Witchcrafts Incopreal soap" (77u)]]
- [["Catie’s Bubbles – Berry Good Noah" (36u)]]
- [["Spearhead – Seaforth! 3 Scotts" (18u)]]
- [["The Holy Black - Gunpower Spice" (16u)]]
- [["London Razors – Coffee and Contemplation" (14u)]]
- [["Barrister and Mann - Passifloria" (15u)]]
- [["Aqua Di Gio" (44u)]]
- [["Pacific Shave Co. - Caffeinated Aftershave Balm" (27u)]]
- [["Stirling Falskally" (15u)]]
- [["RazoRock Mission" (15u)]]
- [["Noble Otter NOC1" (78u) + "Noble Otter (NOC1)" (36u) → Noble Otter NO1C razor]]
- [["@likegrandpa" (26u)]]
- [["B&M Vanille" (21u/8a)]]
- [["HoM Almond Leather Bath Soap" (266u/1a, author-scoped)]]
- [["AS" suffix = aftershave-variant convention]]
- [["Maggard V2OC" (22u)]]
- [["Stirling … oil." strings (Bergamot Lavender 40u, Ozark Mountain 35u, Gentleman 33u, Arkadia 28u, Mountain Man 27u, Bay]]
- [["Merkur 41C" (89u; catalog has attested unverified entries) = the real Merkur "1904" open-comb, short hex handle (B&B]]
- [["Parker 65R" (15u + corroborated unverified entry) = real 3-piece, engraved black-oxide handle (countryknives.com]]
- [["Edwin Jagger DE86" (66u/3a) / "Edwin Jagger DE86RC" (20u) / "Edwin Jagger DE87" (24u/5a) / "DE86" (19u) = real]]
- [["Shavent" (121u/2a) = real German brand (Shavent, Munich; founded 2020; father-daughter Armin Lutz Seidel + Romy]]
- [["Timor" (30u/10a) = real Solingen blade brand; "L'Occitane Baux" = real L'Occitane fragrance; "Barrister & Mann Ferox"]]
- [["Feather Super" (79u/7a) in blade field = almost surely the Feather Artist Club Professional Super (PS-20) blade, NOT]]
- [[Routine-text false positives (never products, never aliases): "Shower"/"shower"/"Cold Water"/"Water"/"cold]]
- [["Parker 111W" = real Parker model]]
- [[brokenjaw622's "Edwin Jagger 111W" (2024–2026, 3 strings) = brand misattribution]]
- [[Blade-field bare "Feather Super" (79u/7a at mining; 201 rechecked = includes razor-field Alumigoose context)]]
- [["Persona Super" = Personna Super Stainless (USA-made, AccuTec Verona)]]
- [["Grooming Dept Otium" = REAL Grooming Dept scent]]
- [["Merkur Super" = blade-field shorthand for the Merkur Super Platinum DE blade (Solingen)]]
- [[Single-author + zero-web-hit ≠ typo]]
- [[Author-pin rule (P-21) reaffirmed in miniature]]
- [[Miner near-misses that must NOT be trusted]]
- [["Hoffman's x AKA Brushworx" = the collab brush]]
- [["(Hoffman Base)" = a poster's base-tagging convention, not a maker distinction]]
- [[Amazon's "Burn The Ships" ≠ Hoffman's "Burn the Ships"]]
- [["Red Hollow" ≠ "Dead Hollow"]]
- [[Name-form folds (one brand group)]]
- [["Hoffman's Grooming - Broken"]]
- [[Catalog-actionable (see lineages.md entry for sourcing): (1) the two unverified "A Date With Mrs. Claus" clusters]]
