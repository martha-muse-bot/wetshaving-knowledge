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

**Method:** manual review of all 230 remaining staged pairs (uses-desc), same
verdict taxonomy as the 03:10 run: genuine typed→meant pairs, false-match
guard additions (real products the miner "corrected" into wrong products),
routine-text guard additions, and leads. Dataset greps over matched_2016–
2026.json for the abbreviation clusters; 7 web-search batches for the
multi-author unknowns. The top-400 is now FULLY reviewed; the remaining
~1,080 pairs below the top-400 were never staged (re-run the miner to
continue).
**ESTABLISHED typed→meant pairs [catalog] (add as aliases/typo-aliases):**

**FALSE-MATCH GUARD additions (real products the miner "corrected" into
wrong products — never fold) [catalog]:**

**ROUTINE-TEXT GUARD additions (never products, never aliases):**
"Coldwater" (11u/2a), "bath" (9u/2a), "Bath" (7u/6a), "shower;"
(6u/1a), "Nope" (7u/5a), "None." (7u/2a), "None!" (6u/4a), "nowt"
(8u/1a, Northern English "nothing"), "splash" (6u/1a), "Wash"
(6u/2a), "Rinse" (6u/1a), "Shaving soap I made" (7u/1a — homemade-soap
marker, not a product), "EVOO" (10u/1a, aftershave field — almost
certainly olive-oil-as-aftershave joke/routine, never a product),
"Lucky Tiger, OoO" (13u/1a — the ", OoO" is an author annotation of
unpinned meaning; product = Lucky Tiger).
**LEADS (unresolved unknowns — do not fold, do not alias):**

**Method notes:** (1) the miner's field-blindness keeps producing
cross-field garbage (razor-field "iKon"→aftershave, fragrance-field
"Carbon"→fragrance, blade-field "lada"→soap) — the review must check
fields, not just strings; (2) dist-1/2 on model numbers is the
highest-risk zone (42C→23C, 29L→24C, 91R→96R, R106→R41, 15C→34C,
MR1→MR14, V3→V2, DE86→DE89) — every one of these was a REAL product
this run, zero were typos; (3) the B&M abbreviation cluster (SoA/LPC/
LLC/C2) shows abbreviations are maker- or community-canonical and
must be resolved per-abbreviation, never by edit distance; (4) web
search remains mandatory before writing off a multi-author unknown
as a typo (the 05:40 run's 111W lesson, re-confirmed by 42C/29L/91R).
**Thread:** the misspellings run's Stirling leftovers — "Stirling Rose"
(10u/3a), "Stirling - EMP" (9u/3a, fragrance), "Stirling Soap Company -
Tsuka" (10u/2a, fragrance). Method: dataset field greps + the maker's own
scent-descriptions page (stirlingsoap.com/pages/scent-descriptions, fetched
live 2026-11-02, page footer "Last Updated: 11/14/2025" — the maker keeps
discontinued scents on the list with a "Discontinued" flag).
All three are MAKER-ATTESTED, real, and discontinued:

General note for validators: the maker's scent page is now on
stirlingsoap.com (migrated from stirlingsoapco.com) and it KEEPS
discontinued scents listed with a "Discontinued" flag — so a
stirlingsoap.com scent-descriptions read is a maker-grade source for
resolving "never heard of it" Stirling strings, even long-dead ones.
The page also confirms ~20 other discontinued scents (Royal, Plumeria,
Red Delicious, Red Eye, Sunflower Fields, Stirling One, Strawberry
Bubbly, Tuscany, Vanilla Bean Espresso, Stirling Clubman, Dunshire,
Ember...); the catalog's coverage against that list is un-audited.
Backlog leads (i), (v), (vi) RESOLVED by this run.
Thread: the 2026-11-02 ~09:30 CDT misspellings run left 16 narrow identity
leads unidentified. This run resolved 11 via dataset author-scope checks +
web research, corrected one prior note, and left 5 as narrowed open leads.
Method: for each typed string, pulled the author's full post context from
sotd_2016–2026_full.json first (author pin / paired strings often settle it),
then web-searched only the residue.
**RESOLVED (all ESTABLISHED unless noted):**

**STILL OPEN (narrowed):**

**Method notes:** (1) author-scope checks beat web search for half of these
— the author's other posts expand the mystery (UbaldJr's "Catie's Bubbles
V"→"CB V"; reddeckwinning's "5 Year Anniversary Edition"; LathaLife's
"Gillette Super Stainless"→"Shick"); (2) the miner's dist-2/3 targets were
wrong on ALL short-string mysteries this run (Zara, Cairo, CBL, 150, Teddy,
S1) — short strings must go through author context, never edit distance;
(3) "CB" is now the second field-dependent abbreviation after "CL"
(Chatillon Lux, aftershave-only) — razor-field CB ≠ soap-field CB.
**Thread:** the 2026-11-02 Stirling trio run left item (a) open — audit
catalog Stirling coverage against the maker's full scent list
(stirlingsoap.com/pages/scent-descriptions). Method: re-fetched the page
live 2026-11-03 (1,619 lines, footer "Last Updated: 11/14/2025" — unchanged
since 11-02); extracted every scent + its own status tag; grep'd
catalog_merged.json (1,137 stirling ids) for coverage; counted dataset uses
(soap/aftershave/fragrance fields, sotd_2016–2026) for each discontinued
scent.
Structural note on the page: the **"Discontinued/Being Discontinued"**
section mixes truly discontinued scents with seasonal and even
standard-line scents — the status flag on each scent's own tag is what
matters, not the section. Also: "Stirling Clubman" carries a **Discontinued**
tag while sitting in the **Standard Line** section.
**Discontinued/Being-Discontinued set (23, per own tags):** Agar, Amyris,
Anise, Banana, Bonaparte, City Slicker, Cypress, Dunshire ("Being
Discontinued"), EMP (Executive Man Pineapple), Glacial Lemony Orange,
Grapefruit with Menthol, Plumeria, Red Delicious, Red Eye, Rose, Royal,
Stirling Clubman, Stirling One, Strawberry Bubbly, Sunflower Fields, Tsuka,
Tuscany, Vanilla Bean Espresso.
### [catalog] Promotions / entries OWED (maker-attested + dataset-attested)

### Negative findings (no entries owed — do NOT create on maker listing alone)

### Corrections to prior notes

### Standing watch item

**Thread:** the 2026-11-03 TFFC-"M" run left two open items — (a) Old_Hiker's
other TFFC odd scents ("Neroli Soleil" ×2, "Woody Wagon" ×1), both off the
harvested TFFC scent lists; (b) generalize the meet-one-off class with a
notes-grep ("one off", "Maggard Meet", "from the artisan") for other makers
with meet-only products. Method: dataset notes reads (sotd_2016–2026_full.json),
author-scoped (the "M" run's lesson: read the author's notes before spending
web slots on single-author mysteries).
**Findings (all ESTABLISHED, from the posters' own notes):**

**Catalog rule for validators [catalog]:** the meet-only one-off class is
now confirmed across THREE makers (TFFC, Summer Break Soaps, Bufflehead
prototypes). A scent string with no web identity — especially a
single-author one — is consistent with a meet one-off or maker prototype,
NOT a mystery by default. Catalog such strings as loose author-scoped
one-off entries; never community-expand them; never mark them
"unidentified" pending a web identity that cannot exist.
**Method note:** the "M" run's lesson held twice over this run — the
dataset narrated both answers. For single-author mysteries, read the
author's notes BEFORE spending web slots; for multi-author mysteries,
check whether any author's notes narrate distribution (meet sample, PIF,
lot find) before assuming a retail product.
**New narrow leads (curiosity compounds):** (1) any other rocketk455 /
Summer Break meet one-offs (standing "one off" notes-grep route);
(2) other **Nebraska Wet Shaving Club exclusives** — rocketk455's own
2020–2021 notes narrate an "Ogallala Bay Rum 2018 Nebraska Wet Shaving
Club Exclusive" (bay rum + tobacco + bourbon; club now defunct): a
club-exclusive retail product (different class from a one-off) whose
channel may explain other odd Nebraska-linked strings; (3) other
pre-launch Bufflehead prototype strings in 2015–2016 notes; (4) other
makers' prototype one-offs narrated in Lather Games notes (Heirloom
surfaced in LG 2016 Wild Card — the "one off" notes-grep is reusable).

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
- [["Prosaro Green" → Proraso Menthol & Eucalyptus (Green) (2026-11-02)]]
- [["B&M SoA" (10u/7a, soap) → Soapmakers of Awesometown]]
- [["B&M LPC" (13u/5a) / "Barrister and Mann LPC" (7u/1a) / "LPC." etc. (70 rows 2016–2021) → Le Petit Chypré (Latha base)]]
- [["B&M LLC" (9u/4a, 2017) / "B&M LLC" / "B&M-LLC" → Lime, Lavender, Cedarwood]]
- [["Barrister and Mann - C2" (6u/1a) / "B&M C2" / "B&M C2 edp" / "C2 AS" → Citricuyá]]
- [["Dr. Jon's 1803" (12u/4a) → Dr. Jon's 1803, a REAL scent (never fold into "Dr. Jon's 13"]]
- [["Mercur/Merker 34C" family extensions: "Merker 34c" (6u/1a)]]
- [["Caitie's Bubbles Berry Good Noah." (13u/1a)]]
- [["[Barrister and Mann - Dickens Revisted - Aftershave](trythatsoap…)" (13u/6a)]]
- [["Chatillion Lux Sunrise on LaSalle" (13u/1a)]]
- [["Summer Break Soaps Wood Shop EdP" (13u/1a)]]
- [["Stirling Conifferous" (12u/1a)]]
- [["Karve alum SB-B" (12u/1a) / "Karve Brass SB A" (8u/2a) / "Karve Brass SB F" (6u/1a) / "Karve alum SB-C" (6u/4a) →]]
- [["Southern Witchcraft - Fougere Nemeta" (12u/4a)]]
- [["Barrister and Mann - Chesire Balm" (12u/1a)]]
- [["ZingariMan – Unscented After Shave Balm" (12u/1a)]]
- [["[Barrister & Mann - Tuesday - Aftershave](trythatsoap…)" (12u/3a)]]
- [["CL Rose Santal AS" (13u/4a) / "DG 88 Chestnut St AS" (11u/1a) / "CL Santal Auster" (10u/6a) / "CL Nefertiti" (11u/3a)]]
- [["SV Stella Alpina" (12u/4a)]]
- [["Personna PDG" (12u/2a)]]
- [["Maggard Lime and Bergamot" (11u/7a)]]
- [["Balzano" (11u/5a)]]
- [["Penhaligons Sartorial" (11u/2a)]]
- [["Personna Blues" (11u/2a)]]
- [["Schick Pro Line P-30" (11u/1a) / "Schick Pro Line" (8u/2a) / "Schick Pro-line" (6u/1a) / "Shick ProLine" (6u/1a)]]
- [["Gillette 7o clock Super stainless" (11u/1a)]]
- [["Astras" (11u/2a)]]
- [["Permasharps" (11u/2a)]]
- [["Wilkison Sword" (11u/1a)]]
- [["London Razos - Mountain Laurel - EdP" (11u/1a)]]
- [["Creed - Adventus" (11u/2a)]]
- [["BIC Chrome Platinium" (11u/2a)]]
- [["Gentlemen's Nod – Musashi" (11u/1a)]]
- [["Barrister and Mann Vanille" (11u/2a)]]
- [["Barrister and Mann - Limon" (11u/1a, fragrance) → Latha Limon]]
- [["Terre du Hermes" (10u/1a)]]
- [["Zingari Man - The Sea Farer" (7u/1a)]]
- [["Soap Commander Honour" (7u/1a)]]
- [["Stirling Arcadia" (7u/1a)]]
- [["Declaration Grooming La Petit Prairie" (7u/1a)]]
- [["Stirling - Unsented - Balm" (7u/1a)]]
- [["B&M - Full measure of men" (7u/1a)]]
- [["Astra s/p" (7u/4a)]]
- [["Cella - Bongiorno al Sandalo" (7u/4a)]]
- [["Voskhods" (9u/3a)]]
- [["Mickey Lee Soapworks Colonia di Agrumes" (7u/1a)]]
- [["Blacklands Vector AC" (9u/1a)]]
- [["GC0.84P" (9u/1a)]]
- [["Proraso - Refrescante - Aftershave" (9u/1a)]]
- [["Sperahead Shaving Company – 3 Scots" (9u/1a)]]
- [["Razorock de1" (9u/2a, razor field)]]
- [["Chiseledface Summer Storm Aftershave" (8u/1a)]]
- [["Gillette Platnum" (8u/1a)]]
- [["Astra - Superior Platium" (8u/1a)]]
- [["APR Velours Noir EdT" (8u/2a)]]
- [["Summer Break Soaps - Shhh!" (8u/1a)]]
- [["Wolfman MR2" (8u/1a)]]
- [["Parker Solo Edge" (8u/1a)]]
- [["Reminiscence- Patchouli" (8u/1a)]]
- [["Noble Otter (NOBC1)" (8u/1a)]]
- [["[Rouge Perfumery Mousse Illuminee](fragrantica…)" (8u/1a)]]
- [["Stirling SDM" (8u/3a, aftershave/soap)]]
- [["WK Washington's Blend" (8u/2a)]]
- [["Stirling Executive Man oil" (8u/1a)]]
- [["CF Orange Creamsicle" (6u/2a)]]
- [["LASSO Topanga Fougere" (6u/1a)]]
- [["Merker 34c" (6u/1a)]]
- [["Myrsol Aqua Balsamica" (6u/3a)]]
- [["Black Ship Grooming "Phillips Fougere"" (6u/1a)]]
- [["Aqua di Gio" (6u/6a)]]
- [["Talbot Author's Ridge" (6u/2a)]]
- [["Ever Ready Stream Line" (6u/1a)]]
- [["Zingari ManThe Socialite Aftershave" (6u/1a)]]
- [["Stirling Soap Co. - Deep Blu Sea - Eau de Toilette" (6u/1a)]]
- [["Shannon's Soap - Indigo Oud" (6u/2a)]]
- [["Loccitane" (6u/1a, aftershave)]]
- [["Chatillon Lux - 1904 - EdP" (6u/4a)]]
- [["Chatillon Lux - Yuzu/Rose/Patchoulli" (6u/1a)]]
- [["Pinaud - Clubman Aftershave Lotion" (6u/1a)]]
- [["Stirling Soap Co. - 6ix7even" (6u/1a)]]
- [["barrister + mann LEVIATHANNN" (6u/1a)]]
- [["Stirling Vanilla Sandlewood." (6u/1a)]]
- [["SBSW Hook" (6u/3a) → Storybook Soapworks Hook]]
- [["DG YPR" (6u/2a, soap) → Yuzu/Rose/Patchouli ("YPR" author-scoped abbreviation, cf. the glossary YRP lead; 2 authors]]
- [["@catiesbubbles" (6u/1a) → Catie's Bubbles (handle-as-brand; product unpinned]]
- [["@stirlingsoap" (9u/1a)]]
- [["@likegrandpa" already on file (same pattern)]]
- [["Fatip Picollo" (6u/2a)]]
- [["Edwin Jagger - 89" (6u/1a)]]
- [["RazoRock Mission" already on file; "Razo Rock Baby Smooth" (9u/2a)]]
- [["Shick Injector" already on file; "Shick Injector blade." (7u/1a) → Schick Injector Blades; "Shick G4" (9u/1a) → Schick]]
- [["Skinbracer" (7u/3a)]]
- [["pol silver" (7u/1a)]]
- [["Personna Lab Blues" (7u/4a) → Personna Comfort Coated]]
- [["Proraso white Pre" (10u/1a) / "Proraso white pre" (9u/1a) / "Proraso Pre" (9u/1a, preshave) / "Proraso - Pre Shave]]
- [["Royall Bay Rhum 57" (7u/1a) → Royall Bay Rhum ("57" variant tag]]
- [["Highland Spring Soap Co. - Green Door" (7u/2a) → Highland Springs Soap Co. Green Door ("Spring" singular variant]]
- [["Southern Witchcrafts - Grapefruit splash" (8u/1a) → SW Gravefruit (the pun name is the product; "Grapefruit" is the]]
- [["Sylva" (7u/3a, fragrance) → Chatillon Lux Sylva EdP (retired Parfums scent; thescentbase list corroborated by dataset]]
- [["Catie's Bubbles – Maggard Razors 2023 Meetup" (10u/1a) → the 2023 Maggard Meetup exclusive (2023-dated strings from 5]]
- [["HoM/DG - Cerberus" (11u/1a)]]
- [["Chatillon Lux - 88 Chestnut St - EdC" (7u/1a)]]
- [["Catie's Bubbles - Miracle EdP" (7u/1a, fragrance)]]
- [["Razorock 'what the puck' black" (7u/1a)]]
- [["Merkur 42C" (12u/4a) / "Merkur 42c" (7u/3a) = REAL]]
- [["Mühle R106" (13u/1a + 8u/1a + 9u/1a "Mühle R106") = REAL]]
- [["Maggard V3" ("Maggards v3" 13u/3a)]]
- [["Maggard MR1" (11u/2a) = REAL handle]]
- [["Parker 29L" (8u/2a) = REAL]]
- [["Parker 91R" (7u/2a) = REAL]]
- [["Weber ARC" (13u/3a) = REAL]]
- [["EJ de86" (7u/1a) = REAL]]
- [["Weishi" (13u/8a, blade/razor fields) = REAL brand]]
- [["Merkur 15 c" (7u/1a) = REAL]]
- [["Carbon" (7u/4a, razor field) = Carbon Shaving Co. razors]]
- [["Yves Saint Laurent - Y" (10u/3a) = REAL]]
- [["Gillette Mach3" (8u/2a) = REAL cartridge]]
- [["Shavent." (11u/1a, razor field)]]
- [["iKon" (11u/1a, razor field) = REAL brand]]
- [["ZaZa"]]
- [["Racer"/"RACER" (11u/2a + 7u/1a, blade field) = REAL]]
- [["lada" (7u/3a, blade field) = REAL]]
- [["Solimo" (6u/1a, blade field) = REAL]]
- [["Green Mug"/"Green Mug -" (13u/1a + 10u/1a, bowl field)]]
- [["Barrister and Mann Ferox" (10u/4a + 6u/2a)]]
- [["Star" (13u/2a, blade/razor)]]
- [["Capri" (10u/3a, aftershave)]]
- [["HAGS - Darkside" (9u/1a, soap)]]
- [["Tallow + Steel – 1 Up" (9u/1a, soap)]]
- [["Stirling - EMP" (9u/3a, fragrance)]]
- [["Stirling Rose" (10u/3a)]]
- [["Stirling Soap Company - Tsuka" (10u/2a, fragrance)]]
- [["Bufflehead A1A" (10u/5a, soap)]]
- [["Eleven - 5" (8u/1a, soap)]]
- [["CL US" (12u/1a, aftershave)]]
- [["RazoRock Smile" (8u/1a, razor)]]
- [["CB V" (7u/1a, aftershave/fragrance)]]
- [["ATT G1" (7u/1a)]]
- [["Above The Tie Atlas S2" (7u/2a)]]
- [["Through the Fire Fine Craft - M" (10u/1a)]]
- [["Shick super stainless" (9u/1a, blade)]]
- [["Chicago Grooming - Fomo" (8u/1a, soap)]]
- [["Strike Gold Shave – TDS" (8u/1a)]]
- [["Gillette yellows" (9u/1a) → 7 O'Clock SharpEdge (color nickname; single author]]
- [["GEM Micro-Magic Open Comb (1st gen)" (13u/1a)]]
- [["Stirling Rose" = REAL discontinued scent]]
- [["EMP" / "Stirling - EMP" = its OWN scent]]
- [["Stirling - Tsuka" = maker-attested Hanae Mori dupe]]
- [["ZaZa" (10u/2a, blade) = REAL — Zaza Stainless Steel DE blades]]
- [["RazoRock Smile" (8u/1a → actually 22 rows, 2 authors, 2026) = REAL]]
- [[HAGS = HAGS Artisan Shaving Products — brand ESTABLISHED]]
- [["Tallow + Steel – 1 Up" = REAL — "1UP", T&S Limited Edition]]
- [["CL US" (12u/2a, aftershave) = Chatillon Lux "Unconditional Surrender" aftershave]]
- [["CB V" (7u/2a, aftershave/fragrance) = Catie's Bubbles "V"]]
- [["ATT G1" (7u/1a, razor) = REAL]]
- [["ATT Atlas S2" (7u/2a, razor) = REAL]]
- [[BLACKLAND-ERA WARNING (2026-11-03)]]
- [["Eleven - 5" (8u/1a, soap) = Eleven "5 Year Anniversary Edition"]]
- [["Shick super stainless" (9u/1a, blade) = vintage SCHICK Super Stainless DE blade (NOT Shark)]]
- [["Chicago Grooming - Fomo" (8u/1a) = Oleo "FOMO" under the renamed brand]]
- [["Capri" (10u/3a, aftershave) = Folsom & Co. "Capri"]]
- [["Star" DE razor = vintage mid-century "Star" DE (NOT the Kampfe wedge-blade)]]
- [[Merkur 42C = CLOSED COMB (scalloped safety bar); 41C = open comb (aliases)]]
- [["Strike Gold Shave – TDS" (8u/1a→ actually 40 rows, 1 author)]]
- [["Bufflehead A1A" (10u/5a, soap) (aliases)]]
- [["Through the Fire Fine Craft - M" (10u/1a, soap)]]
- [["Grooming Dept Otium" note pyramid]]
- [[Mühle R106/R108 head attributions]]
- [[Catie's Bubbles "Porch Drinks" soap = Catie's Bubbles × Carnavis & Richardson collab; Chatillon Lux "Les]]
- [[TUSCANY = the headline audit gap]]
- [[ROYAL — verified entries owed]]
- [[RED EYE — verified entries owed]]
- [[AGAR fragrance — entry owed]]
- [[STIRLING CLUBMAN aftershave — entry OWED (missing)]]
- [[GRAPEFRUIT WITH MENTHOL — verified promotion owed]]
- [[BONAPARTE — verified promotion owed]]
- [[PLUMERIA — verified promotion owed]]
- [[SUNFLOWER FIELDS aftershave — note only]]
- [[Anise: 0 dataset strings]]
- [[Banana: 3 hits / 3 authors, soap field, 2022–2023]]
- [["Ember" RETIRED as a Stirling scent]]
- [[EMP loop closed]]
- [["Dunshire" is mid-discontinuation]]
- [[Stirling Spice (maker: Old Spice homage)]]
- [[The scent-descriptions page is the maker's canonical registry (keeps discontinued scents listed). Recheck quarterly]]
- [[TFFC "Neroli Soleil"]]
- [[TFFC "Woody Wagon"]]
- [[Summer Break Soaps "Hay/Dirt/Cedar"]]
- [[Bufflehead "Heirloom"]]
