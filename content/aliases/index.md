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
"Lucky Tiger, OoO" (13u/1a — the ", OoO" is an author annotation = Oil of Olay Complete (lotion-as-aftershave), author-group tag (Fahrenheit915/Old_Hiker/I_Like_a_Clean_Bowl); product = Lucky Tiger. RESOLVED 2026-11-05, see glossary.md).
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
(2) **RESOLVED 2026-11-03 (learner NWSC run):** the NWSC exclusive is
an **Ogallala Bay Rum** product (maker pinned by rocketk455's own
notes) — NOT a Summer Break one-off. Backlog (d) closed; see the
Ogallala Bay Rum brand entry in lineages.md + the run section below.
(3) other
pre-launch Bufflehead prototype strings in 2015–2016 notes; (4) other
makers' prototype one-offs narrated in Lather Games notes (Heirloom
surfaced in LG 2016 Wild Card — the "one off" notes-grep is reusable).
Thread: the meet-one-off run's leftover (d) — rocketk455's "Ogallala Bay Rum 2018 Nebraska Wet Shaving Club Exclusive." Method: full-corpus string census (soap/notes fields) + rocketk455's notes before web slots.
**Findings (ESTABLISHED):**

**[catalog] Validator actions:**

The 2026-11-01 Leaf run left a lead: scan ischiapp's parentheticals across
all years to catch any of his tags sitting in the catalog as aliases. Full
corpus scan (sotd_2016–2024_full.json, 747 distinct parenthetical tags):
the tags ARE author-scoped as suspected, and several had already leaked
into the catalog — mostly harmless, two need validator action.

---
Three dataset-only/ex-MO titles pinned to lineage:

---
**Lather-Games fiction brands — NEVER create catalog entries.**
Lather Games 2026 ran in **October 2026** with themed days (Graveyard
Day Oct 29, Monster Mash Oct 24, Reckoning Day Oct 25), and the
in-character theme posts contain FULLY FICTIONAL brands with fake
origin stories, fake reviews, and fake reviewer personas:

Method note: when a string's brand has no web footprint AND the note
reads as in-character fiction (reviews-with-personas, marketing-copy
voice, theme-day posting), check the note for the real products
before creating an entry — the fiction brands borrow real products
("BobTheBob" reviewed Stirling Baker Street in the same note).
AntwonPeachFuzz's 2026-11-02 note also shows "345 Soap Co." and
"Seaforth!" as his real den — the fiction was a one-day persona.
**Barrister and Mann Cologne Russe — naming lore (maker-attested
via poster quotes, LEAD-grade until the page is read firsthand)
[catalog]:** B&M Special Edition shaving soap (Omnibus base per the
2026-10-26 dataset product fields: "Barrister and Mann - Cologne
Russe - Shaving Soap, Omnibus Base"; matching splash/EdP-family
posts exist). The product-page copy, quoted verbatim in TWO dataset
notes (AdWorried2804 + AntwonPeachFuzz, both 2026-10-26):
"is a throwback to a scent created by the House of Guerlain for the
Russian royal family and discontinued in the early twentieth
century." The page is linked with a Wayback snapshot
(web.archive.org/web/20240225024729/...) — so the product shipped by
Feb 2024 at the latest. Poster AdWorried2804 adds the pre-1918
reasoning himself ("for the Russian royal family" ⇒ before 1918).
Catalog: never fold vintage **Guerlain Eau de Cologne Russe**
strings into B&M Cologne Russe (century apart, maker vs homage).
Residual: Wayback read of the actual page (live-browser job — the
text sandbox got HTTP 403 from web.archive.org 2026-11-03) to firm
the maker-copy attribution and pin the exact release date.

**Thread:** backlog item (g) — "second mining dimension: misspellings of ARTISAN brands (this pass was dominated by mass-market names because verified entries skew that way — restrict targets to artisan entries and re-rank)." STILL OPEN since 2026-11-02; now resolved.
**Method:** wrote `knowledge/tools/misspell_mine_artisan.py` — same blocked-Levenshtein miner as 2026-11-02 but targets restricted to VERIFIED entries whose brand is NOT in a documented mass-market/heritage/consumer/fragrance/retailer exclusion list (Gillette, Wilkinson, Nivea, Proraso, Arko, Tabac, Old Spice, Dior, Chanel, etc.); wetshaving-specialist retailers (Maggard, WCS, Pasteur) KEPT as artisan-channel targets. Miner ran ~11 min: **1,063 artisan near-miss pairs** → top-400 staged at `knowledge/tools/misspelling_cands_artisan_2026-11-04.json`. Also wrote the FULL unrestricted 1,439-pair list at `knowledge/tools/misspelling_cands_all_2026-11-04.json` (advances backlog item (a) — the complete candidate inventory). Built `build_string_index.py` + `string_index.pkl` (217,315 exact dataset strings) + `review_cands.py` for fast author/note lookup. **All 400 pairs manually reviewed.**
**Method notes (standing):** (1) The miner proposes; the DATASET disposes — every genuine pair was confirmed by author-scoped note reads, never by edit distance alone. (2) Single-author abbreviations stay LEADS (not established) unless a second voice or maker source confirms. (3) The exclusion list has a gap: Giorgio Armani / Dolce & Gabbana / designer-fragrance brands slipped through (they're "artisan" only in the negative sense) — future runs should exclude the fragrance-designer tier explicitly. (4) NEVER correct model numbers/handles across the Maggard MR/V series or ATT S/H/G series by distance — the miner proposed MR1→MR6, V3→V3A, S2→SE1; these are distinct products.
### Established genuine pairs (typed → meant) [catalog]

### Annual/yearly products are distinct (never fold) [catalog]

### Stirling "<scent> oil" routing rule [catalog]
**Stirling "<scent> oil" strings = the OIL product, never fold into soap/splash/fragrance.** rocketk455's note "Beard: Stirling Executive Man oil" confirms beard-oil USE, but the product is Stirling's **pre-shave oil** (B&B: "The Stirling Executive Man pre-shave oil was an interesting experience"). Catalog: Stirling oil entries NOT FOUND — coverage lead (create per-scent or line entry; do NOT alias to soap/splash).
### False-match guard additions (miner wrongly "corrected" real products) [catalog]

### Routine-text guards (never products) [catalog]
shower / water / wash / rinse / lotion / splash / bath / beer / none / nada / nowt / nope / alum / salsa / purple / green mug / EVOO / "shaving soap I made" / "Tobac". **@-handles are social tags, never products** (the benilla photo-credit pattern: "@benilla" in aftershave field = photo credit). **"[Mammoth" = truncation artifact** (bracket from a longer string).
### Field-routing leads for validators [catalog]

### Web-verification leads (logged; live browser not available to learner)
HoM Cirrus; Duke Cannon Seneca/Fulton; Royall Bay Rhum 57; A&E The Club Black; Ethos Success/Succès; Soap Commander Gratitude; MLS Ruby's Garden; Joserra Noir Noir; Abbate Vegano; Carbon Shaving Co. scope; iKon coverage; Shavent catalog entry.
### Dataset leads (single-author or unpinned; need a second voice)

**Backlog:** item (g) checked off (resolved). New narrow leads parked in backlog. Item (a) (full candidate inventory) advanced via `misspelling_cands_all_2026-11-04.json`.

## Product aliases

- [[aliases/lab-blue|"Lab Blue"]]
- [[aliases/wizamet-super-iridium-polsilver-super-iridium|Wizamet Super Iridium ≠ Polsilver Super Iridium]]
- [[aliases/gem-platinum-diamond-glide-is-a-double-edge-blade|GEM Platinum Diamond Glide is a DOUBLE-EDGE blade]]
- [[aliases/gem-slim-v-flat-top-is-not-a-gem-model-name|"GEM Slim V Flat Top" is NOT a GEM model name]]
- [[aliases/wolfman-wr3-gem-format-head-wr4-artist-club-head|Wolfman WR3 = GEM-format head; WR4 = Artist Club head]]
- [[aliases/sticky-community-nickname-for-wilkinson-swords-1960s-de-razor-not-a-model-name|"Sticky" = community nickname for Wilkinson Sword's 1960s DE razor (not a model name, not the modern Classic)]]
- [[aliases/bare-name-conventions|Bare-name conventions]]
- [[aliases/the-recency-trap-methodological-2026-10-21-when-a-dataset-string-matches-no|The recency trap (methodological, 2026-10-21). When a dataset string matches NO known product, check for a]]
- [[aliases/bbs-0-personna-new-angle-70-community-nickname-2026-10-21|"BBS-0" = Personna "New Angle 70" (community nickname, 2026-10-21)]]
- [[aliases/the-freedberg-razorock-emperor-former-name-2026-11-06|"The Freedberg" = RazoRock Emperor (former name, 2026-11-06)]]
- [[aliases/amazlenut-b-and-m-barrister-and-mann-amazelnut-2026-11-01|"Amazlenut (B&M)" → Barrister and Mann "Amazelnut" (2026-11-01)]]
- [[aliases/watchmen-the-watchman-zingari-man-2026-11-04|"Watchmen" → The Watchman (Zingari Man) (2026-11-04)]]
- [[aliases/barritser-barrister-2026-11-03|"Barritser" → Barrister (2026-11-03)]]
- [[aliases/oggalla-ogallala-2026-11-06|"Oggalla" → Ogallala (2026-11-06)]]
- [[aliases/duxham-duplex-shavette-durham-duplex-2026-10-29|"Duxham Duplex shavette" → Durham Duplex (2026-10-29)]]
- [[aliases/personna-specimen-prep-blade|"Personna Specimen Prep (Blade)"]]
- [[aliases/baili-model-code-normalization-rules-2026-10-23-full-analysis-in-hardwarelore-md|Baili model-code normalization rules (2026-10-23; full analysis in hardwarelore.md)]]
- [[aliases/kismet-german-hair-shaper-blade-brand-2026-10-21|"Kismet" = German hair-shaper blade brand (2026-10-21)]]
- [[aliases/name-collision|NAME COLLISION]]
- [[aliases/kismet-maker-attribution-resolved-2026-10-22|Kismet MAKER ATTRIBUTION — RESOLVED (2026-10-22)]]
- [[aliases/personna-travel-is-a-descriptor-not-a-product|"Personna travel" is a descriptor, NOT a product]]
- [[aliases/gillette-airline-tech-is-a-coined-provenance-descriptor-not-a-product-resolved|"Gillette Airline Tech" is a coined provenance descriptor, NOT a product (RESOLVED 2026-10-29). wegian]]
- [[aliases/kismett-hair-shaper|kismett hair shaper]]
- [[aliases/kismet-hai-shaper|kismet hai shaper]]
- [[aliases/wholly-law-wholly-kaw-2026-11-10|"Wholly Law" → Wholly Kaw (2026-11-10)]]
- [[aliases/b-and-m-spice-naming-trap|B&M "Spice" naming trap]]
- [[aliases/tatra-tatara-naming-trap-established-2026-10-21|Tatra ≠ Tatara (naming trap, established 2026-10-21)]]
- [[aliases/the-gillette-blue-blade-family-four-distinct-products-share-one-name-space|The Gillette "Blue" blade family — FOUR distinct products share one name space]]
- [[aliases/dapper-dragon-soaps-ouroboros|Dapper Dragon Soaps "Ouroboros"]]
- [[aliases/beaver-woodwright|"Beaver Woodwright"]]
- [[aliases/bandit-collab-cluster|"Bandit" collab cluster]]
- [[aliases/chatillon-lux-observed-misspellings-mined-2026-10-21|Chatillon Lux observed misspellings (mined 2026-10-21)]]
- [[aliases/wholly-kaw-spelling-variants-mined-2026-10-22|Wholly Kaw spelling variants (mined 2026-10-22)]]
- [[aliases/wax-pass-was-u-j-mts-pre-bufflehead-sampling-phase-not-a-brand|"Wax Pass" was u/j-mt's pre-Bufflehead sampling phase, NOT a brand]]
- [[aliases/grooming-dept-maol-frankenlime|"Grooming Dept / MAOL - Frankenlime"]]
- [[aliases/primos|"primos"]]
- [[aliases/house-of-mammoth-indigo-renamed-mood-indigo-2021-early-2022|House of Mammoth "Indigo" = renamed "Mood Indigo" (2021→early 2022)]]
- [[aliases/stirling-kaboom-deton-8-rename-2019|Stirling "Kaboom" → "Deton-8" (rename, 2019)]]
- [[aliases/zingari-man-the-gypsy|Zingari Man "The Gypsy"]]
- [[aliases/caties-bubbles-blugere-renamed-jersey-blues|Catie's Bubbles "Blugere" = renamed "Jersey Blues"]]
- [[aliases/dusy-kabinett-klar-kabinett-reincarnated|Dusy Kabinett = Klar Kabinett reincarnated]]
- [[aliases/noble-otter-hamam-renamed-hamami|Noble Otter "Hamam" = renamed "Hamami"]]
- [[aliases/lord-tajam-egypt-lord-platinum-regional-rebrand-resolved-2026-10-30|Lord "Tajam" (Egypt) = Lord Platinum regional rebrand (RESOLVED 2026-10-30]]
- [[aliases/the-handlebar-supply-ethos-grooming-essentials-caution-2026-10-22-corrected|"The Handlebar Supply" ≠ Ethos Grooming Essentials (caution, 2026-10-22; CORRECTED 2026-10-26]]
- [[aliases/the-cornfed-viking|The Cornfed Viking]]
- [[aliases/makers-own-announcement-2025-01-25-old-story-names-new-note-number-names|Maker's own announcement (2025-01-25): old story names → new note+number names. Canonical = the NEW name; old name =]]
- [[aliases/six-lassco-scents-live-on-as-chiseled-face-products-lineage-in-lineages-md-in|SIX LASSCo scents live on as Chiseled Face products (lineage in lineages.md), in two waves. They are CONTINUATIONS]]
- [[aliases/matcher-guidance-bare-black-rose-soap-strings-need-brand-date-to-disambiguate|Matcher guidance: bare "Black Rose" soap strings need brand + date to disambiguate (LA pre-2021; CF 2021-04-13+; "The]]
- [[aliases/correction-2026-11-01|CORRECTION (2026-11-01)]]
- [[aliases/through-the-fire-fine-crafts-plural-ttffcrafts-com-2024-through-the-fire-fine|"Through the Fire Fine Crafts" (plural, ttffcrafts.com, 2024+) = "Through the Fire Fine Craft"]]
- [[aliases/2019-2021-a-scent|2019–2021: a SCENT]]
- [[aliases/2020-2023-the-bases-other-name|2020–2023: the base's other name]]
- [[aliases/2023-the-brand-line|2023+: the brand/line]]
- [[aliases/reverence-revenance-aion-skincare-scent|Reverence / Revenance (Aion Skincare scent)]]
- [[aliases/smdf|"SMdF"]]
- [[aliases/crystal-vs-israeli-reds-vs-israeli-personnas|"Crystal" vs "Israeli Reds" vs "Israeli Personnas"]]
- [[aliases/faux-fusion-rebranded-dorco-pace-6-lead-2026-10-24|"Faux Fusion" = rebranded Dorco Pace 6+ (lead, 2026-10-24)]]
- [[aliases/faux-fusion-resolved-2026-10-25|"Faux Fusion" RESOLVED 2026-10-25]]
- [[aliases/pinaud-clubman-and-pinaud-clubman-are-one-brand-group-the-us-clubman-line-now|"Pinaud", "Clubman", and "Pinaud Clubman" are ONE brand group (the US Clubman line, now owned by American International]]
- [[aliases/big-ben-is-two-products-split-by-field-never-by-name|"Big Ben" is TWO products, split by FIELD, never by name]]
- [[aliases/sir-sir|"SIR" = "Sir"]]
- [[aliases/m-uer-and-wirtz-missing-the-second-r-is-a-pervasive-dataset-typo|"Mäuer & Wirtz" (missing the second r) is a pervasive dataset typo]]
- [[aliases/dupe-caution|Dupe caution]]
- [[aliases/kent-sb2|Kent SB2]]
- [[aliases/false-friend-kent-of-inglewood-is-not-kent-brushes|FALSE FRIEND: "Kent of Inglewood" is NOT Kent Brushes]]
- [[aliases/kent-cream-kent-shaving-cream-strings|"Kent cream" / "Kent Shaving Cream" strings]]
- [[aliases/rejected-rebrand-bluebeards-revenge|REJECTED rebrand: Bluebeard's Revenge]]
- [[aliases/enders-dollar-razor|"Enders' Dollar Razor"]]
- [[aliases/christy-christy-se-christy-co-massage-bar-se-not-enders|"Christy" / "Christy SE" → Christy Co. Massage Bar SE, NOT Enders]]
- [[aliases/enders-by-christy-no-dataset-strings-yet-enders-speed-family|"Enders by Christy" (no dataset strings yet) → Enders Speed family]]
- [[aliases/correction-of-a-standing-backlog-guess|CORRECTION of a standing backlog guess]]
- [[aliases/hoffmans-broken-rebranded-burn-the-ships|"Hoffman's Broken" = rebranded "Burn the Ships"]]
- [[aliases/catalog-guidance-catalog|Catalog guidance [catalog] (aliases)]]
- [[aliases/new-leads|New leads]]
- [[aliases/florena-bare-strings-are-not-nivea|"Florena" bare strings are NOT Nivea]]
- [[aliases/method-note-the-refinement-pattern|Method note (the refinement pattern)]]
- [[aliases/ss-cola-sudsy-soapery-cola-author-scoped-abbreviation-lead|"SS Cola" → Sudsy Soapery Cola (author-scoped abbreviation, lead)]]
- [[aliases/razorock-blondie-rebranded-zenith-80n-established-community|RazoRock "Blondie" = rebranded Zenith 80N (established, community)]]
- [[aliases/antica-barbieria-colla-abc-boar-zenith-b03-a26-zenith-b2|Antica Barbieria Colla (ABC) boar ≈ Zenith B03-A26 ("Zenith B2") (aliases)]]
- [[aliases/gillette-astra-is-one-authors-styling-not-a-product-line|"Gillette Astra" is one author's styling, not a product line]]
- [[aliases/b-and-b-auto-censors-a-s-s-read|B&B auto-censors "A.S.S." — read "]]
- [[aliases/astra-blue-bare-blue-blue-blue-pack-the-superior-stainless|"Astra Blue" bare / "(Blue)" / "[Blue]" / "blue-pack" = the Superior Stainless]]
- [[aliases/tass-the-artisan-soap-shoppe|"TASS" = The Artisan Soap Shoppe]]
- [[aliases/hema-de-blades-private-label-personna-made-in-israel|"HEMA" DE blades = private-label Personna made in Israel]]
- [[aliases/vokshod-166u-40a-voshkohd-17u|"Vokshod" (166u/40a) + "Voshkohd" (17u)]]
- [[aliases/persona-116u-10a-cartridge-blade-fields-personna-brand-level-the-matched-target|"Persona" (116u/10a, cartridge/blade fields) → Personna (brand-level; the matched target was Twin Pivot Plus]]
- [[aliases/perssona-blue-53u|"Perssona Blue" (53u)]]
- [[aliases/merker-34c-hd-74u-mercur-34c-15u-2a-merkur-mk23c-14u-merkur-34c|"Merker 34C HD" (74u) + "Mercur 34C" (15u/2a) + "Merkur MK23C" (14u) → Merkur 34C]]
- [[aliases/mhule-r89-20u|"Mhule R89" (20u)]]
- [[aliases/gilette-minora-stainless-28u-2a-gilette-7-oclock-green-27u-gillette-minora|"Gilette Minora Stainless" (28u/2a), "Gilette 7 O'clock (Green)" (27u) → Gillette Minora Stainless]]
- [[aliases/gillette-platinium-20u-gillette-platinun-18u|"Gillette Platinium" (20u) + "Gillette Platinun" (18u)]]
- [[aliases/shick-injector-21u-4a|"Shick Injector" (21u/4a)]]
- [[aliases/bolanzo-14u|"Bolanzo" (14u)]]
- [[aliases/saponificio-vatesino-70th-anniversary-soap-31u|"Saponificio Vatesino - 70th anniversary - Soap" (31u)]]
- [[aliases/chatillion-lux-pure-lavender-25u|"Chatillion Lux Pure Lavender." (25u)]]
- [[aliases/chanel-bleau-de-chanel|"Chanel – Bleau de Chanel"]]
- [[aliases/pinuad-clubman-aftershave-lotion-33u|"Pinuad - Clubman Aftershave Lotion" (33u)]]
- [[aliases/rapira-swedish-super-steel-28u-2a|"Rapira Swedish Super Steel" (28u/2a)]]
- [[aliases/stirling-rambling-man-49u-2a|"Stirling Rambling Man" (49u/2a)]]
- [[aliases/personna-hairshaper-16u|"Personna hairshaper" (16u)]]
- [[aliases/pol-silver-48u-12a-pol-silver-si-15u-2a|"Pol Silver" (48u/12a) + "Pol-Silver SI" (15u/2a)]]
- [[aliases/acutech-pro-15u|"AcuTech Pro" (15u)]]
- [[aliases/bbysmooth-16u|"BBYSMOOTH" (16u)]]
- [[aliases/att-se1-76u-9a-above-the-tie-s1-slant|"ATT SE1" (76u/9a) → Above the Tie S1 Slant]]
- [[aliases/barrister-and-mann-lavender-interupted-37u|"Barrister & Mann - Lavender Interupted" (37u)]]
- [[aliases/southern-witchcrafts-incopreal-soap-77u|"Southern Witchcrafts Incopreal soap" (77u)]]
- [[aliases/catie-s-bubbles-berry-good-noah-36u|"Catie’s Bubbles – Berry Good Noah" (36u)]]
- [[aliases/spearhead-seaforth-3-scotts-18u|"Spearhead – Seaforth! 3 Scotts" (18u)]]
- [[aliases/the-holy-black-gunpower-spice-16u|"The Holy Black - Gunpower Spice" (16u)]]
- [[aliases/london-razors-coffee-and-contemplation-14u|"London Razors – Coffee and Contemplation" (14u)]]
- [[aliases/barrister-and-mann-passifloria-15u|"Barrister and Mann - Passifloria" (15u)]]
- [[aliases/aqua-di-gio-44u|"Aqua Di Gio" (44u)]]
- [[aliases/pacific-shave-co-caffeinated-aftershave-balm-27u|"Pacific Shave Co. - Caffeinated Aftershave Balm" (27u)]]
- [[aliases/stirling-falskally-15u|"Stirling Falskally" (15u)]]
- [[aliases/razorock-mission-15u|"RazoRock Mission" (15u)]]
- [[aliases/noble-otter-noc1-78u-noble-otter-noc1-36u-noble-otter-no1c-razor|"Noble Otter NOC1" (78u) + "Noble Otter (NOC1)" (36u) → Noble Otter NO1C razor]]
- [[aliases/likegrandpa-26u|"@likegrandpa" (26u)]]
- [[aliases/b-and-m-vanille-21u-8a|"B&M Vanille" (21u/8a)]]
- [[aliases/hom-almond-leather-bath-soap-266u-1a-author-scoped|"HoM Almond Leather Bath Soap" (266u/1a, author-scoped)]]
- [[aliases/as-suffix-aftershave-variant-convention|"AS" suffix = aftershave-variant convention]]
- [[aliases/maggard-v2oc-22u|"Maggard V2OC" (22u)]]
- [[aliases/stirling-oil-strings-bergamot-lavender-40u-ozark-mountain-35u-gentleman-33u|"Stirling … oil." strings (Bergamot Lavender 40u, Ozark Mountain 35u, Gentleman 33u, Arkadia 28u, Mountain Man 27u, Bay]]
- [[aliases/merkur-41c-89u-catalog-has-attested-unverified-entries-the-real-merkur-1904|"Merkur 41C" (89u; catalog has attested unverified entries) = the real Merkur "1904" open-comb, short hex handle (B&B]]
- [[aliases/parker-65r-15u-corroborated-unverified-entry-real-3-piece-engraved-black-oxide|"Parker 65R" (15u + corroborated unverified entry) = real 3-piece, engraved black-oxide handle (countryknives.com]]
- [[aliases/edwin-jagger-de86-66u-3a-edwin-jagger-de86rc-20u-edwin-jagger-de87-24u-5a-de86|"Edwin Jagger DE86" (66u/3a) / "Edwin Jagger DE86RC" (20u) / "Edwin Jagger DE87" (24u/5a) / "DE86" (19u) = real]]
- [[aliases/shavent-121u-2a-real-german-brand-shavent-munich-founded-2020-father-daughter|"Shavent" (121u/2a) = real German brand (Shavent, Munich; founded 2020; father-daughter Armin Lutz Seidel + Romy]]
- [[aliases/timor-30u-10a-real-solingen-blade-brand-loccitane-baux-real-loccitane-fragrance|"Timor" (30u/10a) = real Solingen blade brand; "L'Occitane Baux" = real L'Occitane fragrance; "Barrister & Mann Ferox"]]
- [[aliases/feather-super-79u-7a-in-blade-field-almost-surely-the-feather-artist-club|"Feather Super" (79u/7a) in blade field = almost surely the Feather Artist Club Professional Super (PS-20) blade, NOT]]
- [[aliases/routine-text-false-positives-never-products-never-aliases-shower-shower-cold|Routine-text false positives (never products, never aliases): "Shower"/"shower"/"Cold Water"/"Water"/"cold]]
- [[aliases/parker-111w-real-parker-model|"Parker 111W" = real Parker model]]
- [[aliases/brokenjaw622s-edwin-jagger-111w-2024-2026-3-strings-brand-misattribution|brokenjaw622's "Edwin Jagger 111W" (2024–2026, 3 strings) = brand misattribution]]
- [[aliases/blade-field-bare-feather-super-79u-7a-at-mining-201-rechecked-includes-razor|Blade-field bare "Feather Super" (79u/7a at mining; 201 rechecked = includes razor-field Alumigoose context)]]
- [[aliases/persona-super-personna-super-stainless-usa-made-accutec-verona|"Persona Super" = Personna Super Stainless (USA-made, AccuTec Verona)]]
- [[aliases/grooming-dept-otium-real-grooming-dept-scent|"Grooming Dept Otium" = REAL Grooming Dept scent]]
- [[aliases/merkur-super-blade-field-shorthand-for-the-merkur-super-platinum-de-blade|"Merkur Super" = blade-field shorthand for the Merkur Super Platinum DE blade (Solingen)]]
- [[aliases/single-author-zero-web-hit-typo|Single-author + zero-web-hit ≠ typo]]
- [[aliases/author-pin-rule-p-21-reaffirmed-in-miniature|Author-pin rule (P-21) reaffirmed in miniature]]
- [[aliases/miner-near-misses-that-must-not-be-trusted|Miner near-misses that must NOT be trusted]]
- [[aliases/hoffmans-x-aka-brushworx-the-collab-brush|"Hoffman's x AKA Brushworx" = the collab brush]]
- [[aliases/hoffman-base-a-posters-base-tagging-convention-not-a-maker-distinction|"(Hoffman Base)" = a poster's base-tagging convention, not a maker distinction]]
- [[aliases/amazons-burn-the-ships-hoffmans-burn-the-ships|Amazon's "Burn The Ships" ≠ Hoffman's "Burn the Ships"]]
- [[aliases/red-hollow-dead-hollow|"Red Hollow" ≠ "Dead Hollow"]]
- [[aliases/name-form-folds-one-brand-group|Name-form folds (one brand group)]]
- [[aliases/hoffmans-grooming-broken|"Hoffman's Grooming - Broken"]]
- [[aliases/catalog-actionable-see-lineages-md-entry-for-sourcing-1-the-two-unverified-a|Catalog-actionable (see lineages.md entry for sourcing): (1) the two unverified "A Date With Mrs. Claus" clusters]]
- [[aliases/colonel-conk-soaps-are-vdh-made-not-the-other-way-round-2026-11-06|Colonel Conk soaps are VDH-made, NOT the other way round (2026-11-06)]]
- [[aliases/prosaro-green-proraso-menthol-and-eucalyptus-green-2026-11-02|"Prosaro Green" → Proraso Menthol & Eucalyptus (Green) (2026-11-02)]]
- [[aliases/b-and-m-soa-10u-7a-soap-soapmakers-of-awesometown|"B&M SoA" (10u/7a, soap) → Soapmakers of Awesometown]]
- [[aliases/b-and-m-lpc-13u-5a-barrister-and-mann-lpc-7u-1a-lpc-etc-70-rows-2016-2021-le|"B&M LPC" (13u/5a) / "Barrister and Mann LPC" (7u/1a) / "LPC." etc. (70 rows 2016–2021) → Le Petit Chypré (Latha base)]]
- [[aliases/b-and-m-llc-9u-4a-2017-b-and-m-llc-b-and-m-llc-lime-lavender-cedarwood|"B&M LLC" (9u/4a, 2017) / "B&M LLC" / "B&M-LLC" → Lime, Lavender, Cedarwood]]
- [[aliases/barrister-and-mann-c2-6u-1a-b-and-m-c2-b-and-m-c2-edp-c2-as-citricuy|"Barrister and Mann - C2" (6u/1a) / "B&M C2" / "B&M C2 edp" / "C2 AS" → Citricuyá]]
- [[aliases/dr-jons-1803-12u-4a-dr-jons-1803-a-real-scent-never-fold-into-dr-jons-13|"Dr. Jon's 1803" (12u/4a) → Dr. Jon's 1803, a REAL scent (never fold into "Dr. Jon's 13"]]
- [[aliases/mercur-merker-34c-family-extensions-merker-34c-6u-1a|"Mercur/Merker 34C" family extensions: "Merker 34c" (6u/1a)]]
- [[aliases/caities-bubbles-berry-good-noah-13u-1a|"Caitie's Bubbles Berry Good Noah." (13u/1a)]]
- [[aliases/barrister-and-mann-dickens-revisted-aftershave-trythatsoap-13u-6a|"Barrister and Mann - Dickens Revisted - Aftershave" (13u/6a)]]
- [[aliases/chatillion-lux-sunrise-on-lasalle-13u-1a|"Chatillion Lux Sunrise on LaSalle" (13u/1a)]]
- [[aliases/summer-break-soaps-wood-shop-edp-13u-1a|"Summer Break Soaps Wood Shop EdP" (13u/1a)]]
- [[aliases/stirling-conifferous-12u-1a|"Stirling Conifferous" (12u/1a)]]
- [[aliases/karve-alum-sb-b-12u-1a-karve-brass-sb-a-8u-2a-karve-brass-sb-f-6u-1a-karve-alum|"Karve alum SB-B" (12u/1a) / "Karve Brass SB A" (8u/2a) / "Karve Brass SB F" (6u/1a) / "Karve alum SB-C" (6u/4a) →]]
- [[aliases/southern-witchcraft-fougere-nemeta-12u-4a|"Southern Witchcraft - Fougere Nemeta" (12u/4a)]]
- [[aliases/barrister-and-mann-chesire-balm-12u-1a|"Barrister and Mann - Chesire Balm" (12u/1a)]]
- [[aliases/zingariman-unscented-after-shave-balm-12u-1a|"ZingariMan – Unscented After Shave Balm" (12u/1a)]]
- [[aliases/barrister-and-mann-tuesday-aftershave-trythatsoap-12u-3a|"Barrister & Mann - Tuesday - Aftershave" (12u/3a)]]
- [[aliases/cl-rose-santal-as-13u-4a-dg-88-chestnut-st-as-11u-1a-cl-santal-auster-10u-6a-cl|"CL Rose Santal AS" (13u/4a) / "DG 88 Chestnut St AS" (11u/1a) / "CL Santal Auster" (10u/6a) / "CL Nefertiti" (11u/3a)]]
- [[aliases/sv-stella-alpina-12u-4a|"SV Stella Alpina" (12u/4a)]]
- [[aliases/personna-pdg-12u-2a|"Personna PDG" (12u/2a)]]
- [[aliases/maggard-lime-and-bergamot-11u-7a|"Maggard Lime and Bergamot" (11u/7a)]]
- [[aliases/balzano-11u-5a|"Balzano" (11u/5a)]]
- [[aliases/penhaligons-sartorial-11u-2a|"Penhaligons Sartorial" (11u/2a)]]
- [[aliases/personna-blues-11u-2a|"Personna Blues" (11u/2a)]]
- [[aliases/schick-pro-line-p-30-11u-1a-schick-pro-line-8u-2a-schick-pro-line-6u-1a-shick|"Schick Pro Line P-30" (11u/1a) / "Schick Pro Line" (8u/2a) / "Schick Pro-line" (6u/1a) / "Shick ProLine" (6u/1a)]]
- [[aliases/gillette-7o-clock-super-stainless-11u-1a|"Gillette 7o clock Super stainless" (11u/1a)]]
- [[aliases/astras-11u-2a|"Astras" (11u/2a)]]
- [[aliases/permasharps-11u-2a|"Permasharps" (11u/2a)]]
- [[aliases/wilkison-sword-11u-1a|"Wilkison Sword" (11u/1a)]]
- [[aliases/london-razos-mountain-laurel-edp-11u-1a|"London Razos - Mountain Laurel - EdP" (11u/1a)]]
- [[aliases/creed-adventus-11u-2a|"Creed - Adventus" (11u/2a)]]
- [[aliases/bic-chrome-platinium-11u-2a|"BIC Chrome Platinium" (11u/2a)]]
- [[aliases/gentlemens-nod-musashi-11u-1a|"Gentlemen's Nod – Musashi" (11u/1a)]]
- [[aliases/barrister-and-mann-vanille-11u-2a|"Barrister and Mann Vanille" (11u/2a)]]
- [[aliases/barrister-and-mann-limon-11u-1a-fragrance-latha-limon|"Barrister and Mann - Limon" (11u/1a, fragrance) → Latha Limon]]
- [[aliases/terre-du-hermes-10u-1a|"Terre du Hermes" (10u/1a)]]
- [[aliases/zingari-man-the-sea-farer-7u-1a|"Zingari Man - The Sea Farer" (7u/1a)]]
- [[aliases/soap-commander-honour-7u-1a|"Soap Commander Honour" (7u/1a)]]
- [[aliases/stirling-arcadia-7u-1a|"Stirling Arcadia" (7u/1a)]]
- [[aliases/declaration-grooming-la-petit-prairie-7u-1a|"Declaration Grooming La Petit Prairie" (7u/1a)]]
- [[aliases/stirling-unsented-balm-7u-1a|"Stirling - Unsented - Balm" (7u/1a)]]
- [[aliases/b-and-m-full-measure-of-men-7u-1a|"B&M - Full measure of men" (7u/1a)]]
- [[aliases/astra-s-p-7u-4a|"Astra s/p" (7u/4a)]]
- [[aliases/cella-bongiorno-al-sandalo-7u-4a|"Cella - Bongiorno al Sandalo" (7u/4a)]]
- [[aliases/voskhods-9u-3a|"Voskhods" (9u/3a)]]
- [[aliases/mickey-lee-soapworks-colonia-di-agrumes-7u-1a|"Mickey Lee Soapworks Colonia di Agrumes" (7u/1a)]]
- [[aliases/blacklands-vector-ac-9u-1a|"Blacklands Vector AC" (9u/1a)]]
- [[aliases/gc0-84p-9u-1a|"GC0.84P" (9u/1a)]]
- [[aliases/proraso-refrescante-aftershave-9u-1a|"Proraso - Refrescante - Aftershave" (9u/1a)]]
- [[aliases/sperahead-shaving-company-3-scots-9u-1a|"Sperahead Shaving Company – 3 Scots" (9u/1a)]]
- [[aliases/razorock-de1-9u-2a-razor-field|"Razorock de1" (9u/2a, razor field)]]
- [[aliases/chiseledface-summer-storm-aftershave-8u-1a|"Chiseledface Summer Storm Aftershave" (8u/1a)]]
- [[aliases/gillette-platnum-8u-1a|"Gillette Platnum" (8u/1a)]]
- [[aliases/astra-superior-platium-8u-1a|"Astra - Superior Platium" (8u/1a)]]
- [[aliases/apr-velours-noir-edt-8u-2a|"APR Velours Noir EdT" (8u/2a)]]
- [[aliases/summer-break-soaps-shhh-8u-1a|"Summer Break Soaps - Shhh!" (8u/1a)]]
- [[aliases/wolfman-mr2-8u-1a|"Wolfman MR2" (8u/1a)]]
- [[aliases/parker-solo-edge-8u-1a|"Parker Solo Edge" (8u/1a)]]
- [[aliases/reminiscence-patchouli-8u-1a|"Reminiscence- Patchouli" (8u/1a)]]
- [[aliases/noble-otter-nobc1-8u-1a|"Noble Otter (NOBC1)" (8u/1a)]]
- [[aliases/rouge-perfumery-mousse-illuminee-fragrantica-8u-1a|"Rouge Perfumery Mousse Illuminee" (8u/1a)]]
- [[aliases/stirling-sdm-8u-3a-aftershave-soap|"Stirling SDM" (8u/3a, aftershave/soap)]]
- [[aliases/wk-washingtons-blend-8u-2a|"WK Washington's Blend" (8u/2a)]]
- [[aliases/stirling-executive-man-oil-8u-1a|"Stirling Executive Man oil" (8u/1a)]]
- [[aliases/cf-orange-creamsicle-6u-2a|"CF Orange Creamsicle" (6u/2a)]]
- [[aliases/lasso-topanga-fougere-6u-1a|"LASSO Topanga Fougere" (6u/1a)]]
- [[aliases/merker-34c-6u-1a|"Merker 34c" (6u/1a)]]
- [[aliases/myrsol-aqua-balsamica-6u-3a|"Myrsol Aqua Balsamica" (6u/3a)]]
- [[aliases/black-ship-grooming-phillips-fougere-6u-1a|"Black Ship Grooming "Phillips Fougere"" (6u/1a)]]
- [[aliases/aqua-di-gio-6u-6a|"Aqua di Gio" (6u/6a)]]
- [[aliases/talbot-authors-ridge-6u-2a|"Talbot Author's Ridge" (6u/2a)]]
- [[aliases/ever-ready-stream-line-6u-1a|"Ever Ready Stream Line" (6u/1a)]]
- [[aliases/zingari-manthe-socialite-aftershave-6u-1a|"Zingari ManThe Socialite Aftershave" (6u/1a)]]
- [[aliases/stirling-soap-co-deep-blu-sea-eau-de-toilette-6u-1a|"Stirling Soap Co. - Deep Blu Sea - Eau de Toilette" (6u/1a)]]
- [[aliases/shannons-soap-indigo-oud-6u-2a|"Shannon's Soap - Indigo Oud" (6u/2a)]]
- [[aliases/loccitane-6u-1a-aftershave|"Loccitane" (6u/1a, aftershave)]]
- [[aliases/chatillon-lux-1904-edp-6u-4a|"Chatillon Lux - 1904 - EdP" (6u/4a)]]
- [[aliases/chatillon-lux-yuzu-rose-patchoulli-6u-1a|"Chatillon Lux - Yuzu/Rose/Patchoulli" (6u/1a)]]
- [[aliases/pinaud-clubman-aftershave-lotion-6u-1a|"Pinaud - Clubman Aftershave Lotion" (6u/1a)]]
- [[aliases/stirling-soap-co-6ix7even-6u-1a|"Stirling Soap Co. - 6ix7even" (6u/1a)]]
- [[aliases/barrister-mann-leviathannn-6u-1a|"barrister + mann LEVIATHANNN" (6u/1a)]]
- [[aliases/stirling-vanilla-sandlewood-6u-1a|"Stirling Vanilla Sandlewood." (6u/1a)]]
- [[aliases/sbsw-hook-6u-3a-storybook-soapworks-hook|"SBSW Hook" (6u/3a) → Storybook Soapworks Hook]]
- [[aliases/dg-ypr-6u-2a-soap-yuzu-rose-patchouli-ypr-author-scoped-abbreviation-cf-the|"DG YPR" (6u/2a, soap) → Yuzu/Rose/Patchouli ("YPR" author-scoped abbreviation, cf. the glossary YRP lead; 2 authors]]
- [[aliases/catiesbubbles-6u-1a-caties-bubbles-handle-as-brand-product-unpinned|"@catiesbubbles" (6u/1a) → Catie's Bubbles (handle-as-brand; product unpinned]]
- [[aliases/stirlingsoap-9u-1a|"@stirlingsoap" (9u/1a)]]
- [[aliases/likegrandpa-already-on-file-same-pattern|"@likegrandpa" already on file (same pattern)]]
- [[aliases/fatip-picollo-6u-2a|"Fatip Picollo" (6u/2a)]]
- [[aliases/edwin-jagger-89-6u-1a|"Edwin Jagger - 89" (6u/1a)]]
- [[aliases/razorock-mission-already-on-file-razo-rock-baby-smooth-9u-2a|"RazoRock Mission" already on file; "Razo Rock Baby Smooth" (9u/2a)]]
- [[aliases/shick-injector-already-on-file-shick-injector-blade-7u-1a-schick-injector|"Shick Injector" already on file; "Shick Injector blade." (7u/1a) → Schick Injector Blades; "Shick G4" (9u/1a) → Schick]]
- [[aliases/skinbracer-7u-3a|"Skinbracer" (7u/3a)]]
- [[aliases/pol-silver-7u-1a|"pol silver" (7u/1a)]]
- [[aliases/personna-lab-blues-7u-4a-personna-comfort-coated|"Personna Lab Blues" (7u/4a) → Personna Comfort Coated]]
- [[aliases/proraso-white-pre-10u-1a-proraso-white-pre-9u-1a-proraso-pre-9u-1a-preshave|"Proraso white Pre" (10u/1a) / "Proraso white pre" (9u/1a) / "Proraso Pre" (9u/1a, preshave) / "Proraso - Pre Shave]]
- [[aliases/royall-bay-rhum-57-7u-1a-royall-bay-rhum-57-variant-tag|"Royall Bay Rhum 57" (7u/1a) → Royall Bay Rhum ("57" variant tag]]
- [[aliases/highland-spring-soap-co-green-door-7u-2a-highland-springs-soap-co-green-door|"Highland Spring Soap Co. - Green Door" (7u/2a) → Highland Springs Soap Co. Green Door ("Spring" singular variant]]
- [[aliases/southern-witchcrafts-grapefruit-splash-8u-1a-sw-gravefruit-the-pun-name-is-the|"Southern Witchcrafts - Grapefruit splash" (8u/1a) → SW Gravefruit (the pun name is the product; "Grapefruit" is the]]
- [[aliases/sylva-7u-3a-fragrance-chatillon-lux-sylva-edp-retired-parfums-scent|"Sylva" (7u/3a, fragrance) → Chatillon Lux Sylva EdP (retired Parfums scent; thescentbase list corroborated by dataset]]
- [[aliases/caties-bubbles-maggard-razors-2023-meetup-10u-1a-the-2023-maggard-meetup|"Catie's Bubbles – Maggard Razors 2023 Meetup" (10u/1a) → the 2023 Maggard Meetup exclusive (2023-dated strings from 5]]
- [[aliases/hom-dg-cerberus-11u-1a|"HoM/DG - Cerberus" (11u/1a)]]
- [[aliases/chatillon-lux-88-chestnut-st-edc-7u-1a|"Chatillon Lux - 88 Chestnut St - EdC" (7u/1a)]]
- [[aliases/caties-bubbles-miracle-edp-7u-1a-fragrance|"Catie's Bubbles - Miracle EdP" (7u/1a, fragrance)]]
- [[aliases/razorock-what-the-puck-black-7u-1a|"Razorock 'what the puck' black" (7u/1a)]]
- [[aliases/merkur-42c-12u-4a-merkur-42c-7u-3a-real|"Merkur 42C" (12u/4a) / "Merkur 42c" (7u/3a) = REAL]]
- [[aliases/m-hle-r106-13u-1a-8u-1a-9u-1a-m-hle-r106-real|"Mühle R106" (13u/1a + 8u/1a + 9u/1a "Mühle R106") = REAL]]
- [[aliases/maggard-v3-maggards-v3-13u-3a|"Maggard V3" ("Maggards v3" 13u/3a)]]
- [[aliases/maggard-mr1-11u-2a-real-handle|"Maggard MR1" (11u/2a) = REAL handle]]
- [[aliases/parker-29l-8u-2a-real|"Parker 29L" (8u/2a) = REAL]]
- [[aliases/parker-91r-7u-2a-real|"Parker 91R" (7u/2a) = REAL]]
- [[aliases/weber-arc-13u-3a-real|"Weber ARC" (13u/3a) = REAL]]
- [[aliases/ej-de86-7u-1a-real|"EJ de86" (7u/1a) = REAL]]
- [[aliases/weishi-13u-8a-blade-razor-fields-real-brand|"Weishi" (13u/8a, blade/razor fields) = REAL brand]]
- [[aliases/merkur-15-c-7u-1a-real|"Merkur 15 c" (7u/1a) = REAL]]
- [[aliases/carbon-7u-4a-razor-field-carbon-shaving-co-razors|"Carbon" (7u/4a, razor field) = Carbon Shaving Co. razors]]
- [[aliases/yves-saint-laurent-y-10u-3a-real|"Yves Saint Laurent - Y" (10u/3a) = REAL]]
- [[aliases/gillette-mach3-8u-2a-real-cartridge|"Gillette Mach3" (8u/2a) = REAL cartridge]]
- [[aliases/shavent-11u-1a-razor-field|"Shavent." (11u/1a, razor field)]]
- [[aliases/ikon-11u-1a-razor-field-real-brand|"iKon" (11u/1a, razor field) = REAL brand]]
- [[aliases/zaza|"ZaZa"]]
- [[aliases/racer-racer-11u-2a-7u-1a-blade-field-real|"Racer"/"RACER" (11u/2a + 7u/1a, blade field) = REAL]]
- [[aliases/lada-7u-3a-blade-field-real|"lada" (7u/3a, blade field) = REAL]]
- [[aliases/solimo-6u-1a-blade-field-real|"Solimo" (6u/1a, blade field) = REAL]]
- [[aliases/green-mug-green-mug-13u-1a-10u-1a-bowl-field|"Green Mug"/"Green Mug -" (13u/1a + 10u/1a, bowl field)]]
- [[aliases/barrister-and-mann-ferox-10u-4a-6u-2a|"Barrister and Mann Ferox" (10u/4a + 6u/2a)]]
- [[aliases/star-13u-2a-blade-razor|"Star" (13u/2a, blade/razor)]]
- [[aliases/capri-10u-3a-aftershave|"Capri" (10u/3a, aftershave)]]
- [[aliases/hags-darkside-9u-1a-soap|"HAGS - Darkside" (9u/1a, soap)]]
- [[aliases/tallow-steel-1-up-9u-1a-soap|"Tallow + Steel – 1 Up" (9u/1a, soap)]]
- [[aliases/stirling-emp-9u-3a-fragrance|"Stirling - EMP" (9u/3a, fragrance)]]
- [[aliases/stirling-rose-10u-3a|"Stirling Rose" (10u/3a)]]
- [[aliases/stirling-soap-company-tsuka-10u-2a-fragrance|"Stirling Soap Company - Tsuka" (10u/2a, fragrance)]]
- [[aliases/bufflehead-a1a-10u-5a-soap|"Bufflehead A1A" (10u/5a, soap)]]
- [[aliases/eleven-5-8u-1a-soap|"Eleven - 5" (8u/1a, soap)]]
- [[aliases/cl-us-12u-1a-aftershave|"CL US" (12u/1a, aftershave)]]
- [[aliases/razorock-smile-8u-1a-razor|"RazoRock Smile" (8u/1a, razor)]]
- [[aliases/cb-v-7u-1a-aftershave-fragrance|"CB V" (7u/1a, aftershave/fragrance)]]
- [[aliases/att-g1-7u-1a|"ATT G1" (7u/1a)]]
- [[aliases/above-the-tie-atlas-s2-7u-2a|"Above The Tie Atlas S2" (7u/2a)]]
- [[aliases/through-the-fire-fine-craft-m-10u-1a|"Through the Fire Fine Craft - M" (10u/1a)]]
- [[aliases/shick-super-stainless-9u-1a-blade|"Shick super stainless" (9u/1a, blade)]]
- [[aliases/chicago-grooming-fomo-8u-1a-soap|"Chicago Grooming - Fomo" (8u/1a, soap)]]
- [[aliases/strike-gold-shave-tds-8u-1a|"Strike Gold Shave – TDS" (8u/1a)]]
- [[aliases/gillette-yellows-9u-1a-7-oclock-sharpedge-color-nickname-single-author|"Gillette yellows" (9u/1a) → 7 O'Clock SharpEdge (color nickname; single author]]
- [[aliases/gem-micro-magic-open-comb-1st-gen-13u-1a|"GEM Micro-Magic Open Comb (1st gen)" (13u/1a)]]
- [[aliases/stirling-rose-real-discontinued-scent|"Stirling Rose" = REAL discontinued scent]]
- [[aliases/emp-stirling-emp-its-own-scent|"EMP" / "Stirling - EMP" = its OWN scent]]
- [[aliases/stirling-tsuka-maker-attested-hanae-mori-dupe|"Stirling - Tsuka" = maker-attested Hanae Mori dupe]]
- [[aliases/zaza-10u-2a-blade-real-zaza-stainless-steel-de-blades|"ZaZa" (10u/2a, blade) = REAL — Zaza Stainless Steel DE blades]]
- [[aliases/razorock-smile-8u-1a-actually-22-rows-2-authors-2026-real|"RazoRock Smile" (8u/1a → actually 22 rows, 2 authors, 2026) = REAL]]
- [[aliases/hags-hags-artisan-shaving-products-brand-established|HAGS = HAGS Artisan Shaving Products — brand ESTABLISHED]]
- [[aliases/tallow-steel-1-up-real-1up-t-and-s-limited-edition|"Tallow + Steel – 1 Up" = REAL — "1UP", T&S Limited Edition]]
- [[aliases/cl-us-12u-2a-aftershave-chatillon-lux-unconditional-surrender-aftershave|"CL US" (12u/2a, aftershave) = Chatillon Lux "Unconditional Surrender" aftershave]]
- [[aliases/cb-v-7u-2a-aftershave-fragrance-caties-bubbles-v|"CB V" (7u/2a, aftershave/fragrance) = Catie's Bubbles "V"]]
- [[aliases/att-g1-7u-1a-razor-real|"ATT G1" (7u/1a, razor) = REAL]]
- [[aliases/att-atlas-s2-7u-2a-razor-real|"ATT Atlas S2" (7u/2a, razor) = REAL]]
- [[aliases/blackland-era-warning-2026-11-03|BLACKLAND-ERA WARNING (2026-11-03)]]
- [[aliases/eleven-5-8u-1a-soap-eleven-5-year-anniversary-edition|"Eleven - 5" (8u/1a, soap) = Eleven "5 Year Anniversary Edition"]]
- [[aliases/shick-super-stainless-9u-1a-blade-vintage-schick-super-stainless-de-blade-not|"Shick super stainless" (9u/1a, blade) = vintage SCHICK Super Stainless DE blade (NOT Shark)]]
- [[aliases/chicago-grooming-fomo-8u-1a-oleo-fomo-under-the-renamed-brand|"Chicago Grooming - Fomo" (8u/1a) = Oleo "FOMO" under the renamed brand]]
- [[aliases/capri-10u-3a-aftershave-folsom-and-co-capri|"Capri" (10u/3a, aftershave) = Folsom & Co. "Capri"]]
- [[aliases/star-de-razor-vintage-mid-century-star-de-not-the-kampfe-wedge-blade|"Star" DE razor = vintage mid-century "Star" DE (NOT the Kampfe wedge-blade)]]
- [[aliases/merkur-42c-closed-comb-scalloped-safety-bar-41c-open-comb|Merkur 42C = CLOSED COMB (scalloped safety bar); 41C = open comb (aliases)]]
- [[aliases/strike-gold-shave-tds-8u-1a-actually-40-rows-1-author|"Strike Gold Shave – TDS" (8u/1a→ actually 40 rows, 1 author)]]
- [[aliases/bufflehead-a1a-10u-5a-soap-2|"Bufflehead A1A" (10u/5a, soap) (aliases)]]
- [[aliases/through-the-fire-fine-craft-m-10u-1a-soap|"Through the Fire Fine Craft - M" (10u/1a, soap)]]
- [[aliases/grooming-dept-otium-note-pyramid|"Grooming Dept Otium" note pyramid]]
- [[aliases/m-hle-r106-r108-head-attributions|Mühle R106/R108 head attributions]]
- [[aliases/caties-bubbles-porch-drinks-soap-caties-bubbles-carnavis-and-richardson-collab|Catie's Bubbles "Porch Drinks" soap = Catie's Bubbles × Carnavis & Richardson collab; Chatillon Lux "Les]]
- [[aliases/tuscany-the-headline-audit-gap|TUSCANY = the headline audit gap]]
- [[aliases/royal-verified-entries-owed|ROYAL — verified entries owed]]
- [[aliases/red-eye-verified-entries-owed|RED EYE — verified entries owed]]
- [[aliases/agar-fragrance-entry-owed|AGAR fragrance — entry owed]]
- [[aliases/stirling-clubman-aftershave-entry-owed-missing|STIRLING CLUBMAN aftershave — entry OWED (missing)]]
- [[aliases/grapefruit-with-menthol-verified-promotion-owed|GRAPEFRUIT WITH MENTHOL — verified promotion owed]]
- [[aliases/bonaparte-verified-promotion-owed|BONAPARTE — verified promotion owed]]
- [[aliases/plumeria-verified-promotion-owed|PLUMERIA — verified promotion owed]]
- [[aliases/sunflower-fields-aftershave-note-only|SUNFLOWER FIELDS aftershave — note only]]
- [[aliases/anise-0-dataset-strings|Anise: 0 dataset strings]]
- [[aliases/banana-3-hits-3-authors-soap-field-2022-2023|Banana: 3 hits / 3 authors, soap field, 2022–2023]]
- [[aliases/ember-retired-as-a-stirling-scent|"Ember" RETIRED as a Stirling scent]]
- [[aliases/emp-loop-closed|EMP loop closed]]
- [[aliases/dunshire-is-mid-discontinuation|"Dunshire" is mid-discontinuation]]
- [[aliases/stirling-spice-maker-old-spice-homage|Stirling Spice (maker: Old Spice homage)]]
- [[aliases/the-scent-descriptions-page-is-the-makers-canonical-registry-keeps-discontinued|The scent-descriptions page is the maker's canonical registry (keeps discontinued scents listed). Recheck quarterly]]
- [[aliases/tffc-neroli-soleil|TFFC "Neroli Soleil"]]
- [[aliases/tffc-woody-wagon|TFFC "Woody Wagon"]]
- [[aliases/summer-break-soaps-hay-dirt-cedar|Summer Break Soaps "Hay/Dirt/Cedar"]]
- [[aliases/bufflehead-heirloom|Bufflehead "Heirloom"]]
- [[aliases/maker-pinned-ogallala-bay-rum-not-summer-break-soaps|Maker pinned: Ogallala Bay Rum, not Summer Break Soaps]]
- [[aliases/product|Product]]
- [[aliases/ogallala-brand-established|Ogallala brand established]]
- [[aliases/bonus-ballenclaugh-corroboration|Bonus — Ballenclaugh corroboration]]
- [[aliases/bonus-cannonball-launch-pinned|Bonus — Cannonball launch pinned]]
- [[aliases/merge-unverified-soap-ogallala-bay-rum-2018-nebraska-wet-shaving-club-exclusive|MERGE unverified/soap/ogallala-bay-rum-2018-nebraska-wet-shaving-club-exclusive +]]
- [[aliases/never-fold-nwsc-exclusive-strings-into-summer-break-soaps-rocketk455-was-the|NEVER fold NWSC-exclusive strings into Summer Break Soaps (rocketk455 was the member, not the maker) or into retail]]
- [[aliases/merge-brand-groups-ogallala-bay-rum-ogallala|Merge brand groups ogallala-bay-rum + ogallala]]
- [[aliases/fanzine-saponifications|Fanzine Saponifications]]
- [[aliases/cap-rw-a-genuine-kai-product-code-not-an-author-tag|(CAP-RW) = a GENUINE Kai product code, not an author tag]]
- [[aliases/sapphoo-red-chinese-replica-blade-never-fold-to-kai|Sapphoo Red = Chinese replica blade, never fold to Kai]]
- [[aliases/action-merge-the-lemonwald-kinghood-duplicate|ACTION — merge the Lemonwald/Kinghood duplicate]]
- [[aliases/action-strip-sample-repack-from-four-soap-entry-ids|ACTION — strip "-sample-repack" from four soap entry IDs]]
- [[aliases/rip-discontinued-tag-not-ischiapp-only|"(RIP)" = discontinued tag (NOT ischiapp-only)]]
- [[aliases/shade-schade-resolved-was-glossary-lead|SHaDE/SCHaDE RESOLVED (was glossary lead)]]
- [[aliases/baybarry-anecdotal-provenance-chain-confirmed|Baybarry anecdotal provenance chain confirmed]]
- [[aliases/benton-park-american-perfumer-never-maher-olfactive|"Benton Park" = AMERICAN PERFUMER, never Maher Olfactive]]
- [[aliases/tempo-rubato-discontinued-mo-standard|"Tempo Rubato" = discontinued MO standard]]
- [[aliases/barrel-aged-treachery-le-confirmed|"Barrel Aged Treachery" LE confirmed]]
- [[aliases/the-shave-repository-the-tales-of-the-forgotten|"The Shave Repository - The Tales of the Forgotten"]]
- [[aliases/grave-robber-soap-co-cleansing-fire|"Grave Robber Soap Co. - Cleansing Fire"]]
- [[aliases/central-texas-soaps-cowboy-spice-pasteurs-exclusive-pasteur-pharmacy|"Central Texas Soaps Cowboy Spice (Pasteur's Exclusive)" / "(Pasteur Pharmacy Collaboration)"]]
- [[aliases/lqv-chatillon-lux-la-quatri-me-ville|LQV → Chatillon Lux La Quatrième Ville]]
- [[aliases/moti-declaration-grooming-massacre-of-the-innocents|MOTI → Declaration Grooming Massacre of the Innocents]]
- [[aliases/mmbt-gem-micromatic-bullet-tip-flying-wing|MMBT → GEM Micromatic Bullet Tip (= Flying Wing)]]
- [[aliases/gls-gratiot-league-square|GLS = Gratiot League Square]]
- [[aliases/sbsw-storybook-soapworks|SBSW = Storybook Soapworks]]
- [[aliases/hc-and-c-hendrix-classics-and-co|HC&C = Hendrix Classics & Co]]
- [[aliases/mlsw-mickey-lee-soapworks|MLSW = Mickey Lee Soapworks]]
- [[aliases/bam-bm-barrister-and-mann|BaM / BM = Barrister and Mann]]
- [[aliases/br-barristers-reserve|BR = Barrister's Reserve]]
- [[aliases/gtb-chiseled-face-ghost-town-barber|GTB = Chiseled Face Ghost Town Barber]]
- [[aliases/gc0-84p-razorock-game-changer-0-84-plate|GC0.84P = RazoRock Game Changer 0.84 plate]]
- [[aliases/v2oc-maggard-v2-open-comb-head|V2OC = Maggard V2 open-comb head]]
- [[aliases/clux-chatillon-lux|CLux = Chatillon Lux]]
- [[aliases/asft-lucky-tiger-after-shave-face-tonic|ASFT = Lucky Tiger After Shave Face Tonic]]
- [[aliases/lpp-la-petite-prairie|LPP = La Petite Prairie]]
- [[aliases/cda-colonia-di-agrumi|CdA = Colonia di Agrumi]]
- [[aliases/sw-southern-witchcrafts|SW = Southern Witchcrafts]]
- [[aliases/yrp-ypr-yuzu-rose-patchouli|YRP / YPR = Yuzu Rose Patchouli]]
- [[aliases/rhino-zoologist-rhinoceros|Rhino → Zoologist Rhinoceros]]
- [[aliases/blackbeard-wsp-wet-shaving-products-blackbeard|Blackbeard → WSP (Wet Shaving Products) Blackbeard]]
- [[aliases/kool-kool-shave-cream|Kool → Kool Shave Cream]]
- [[aliases/herod-parfums-de-marly-herod|Herod → Parfums de Marly Herod]]
- [[aliases/treat-treet|Treat → Treet]]
- [[aliases/waking-dreams-waking-dream|Waking Dreams → Waking Dream]]
- [[aliases/reminisence-patchouli-reminiscence-patchouli|Reminisence Patchouli → Reminiscence Patchouli]]
- [[aliases/encre-noir-encre-noire|Encre Noir → Encre Noire]]
- [[aliases/sbs-roty-2022-2023-2024|SBS ROTY 2022 / 2023 / 2024]]
- [[aliases/caties-bubbles-maggard-meetup-2023-vs-2024|Catie's Bubbles Maggard Meetup 2023 vs 2024]]
- [[aliases/caties-bubbles-dftr-done-for-the-retirement-resolved-2026-11-05|Catie's Bubbles "DFTR" = "Done For The Retirement" (RESOLVED 2026-11-05)]]
- [[aliases/djt-vs-tds-are-companion-scents-never-fold-djt-tds|DJT vs TDS are companion scents, never fold DJT→TDS]]
- [[aliases/shavent|Shavent (aliases)]]
- [[aliases/gem-1924|GEM 1924]]
- [[aliases/att-se1|ATT SE1]]
- [[aliases/maggard-v3a-v3-mr1-mr6-mr18-mv3a|Maggard V3A / V3 / MR1 / MR6 / MR18 / Mv3a]]
- [[aliases/ikon-razors|iKon razors]]
- [[aliases/razorock-de1-baili-176|RazoRock DE1 = Baili 176]]
- [[aliases/att-h1-g1-atlas-s2|ATT H1 / G1 / Atlas S2]]
- [[aliases/b-and-m-ferox-royal-soa-lpc-c2-pp8|B&M Ferox / Royal / SoA / LPC / C2 / PP8]]
- [[aliases/tffc-m|TFFC "M"]]
- [[aliases/hags-darkside|HAGS Darkside]]
- [[aliases/t-and-s-1up|T&S 1UP]]
- [[aliases/razorock-smile|RazoRock Smile]]
- [[aliases/zaza-blades|ZaZa blades]]
- [[aliases/folsom-capri|Folsom Capri]]
- [[aliases/eleven-5|Eleven "5"]]
- [[aliases/dr-jons-1803-hex|Dr. Jon's 1803 / Hex]]
- [[aliases/cb-v-x|CB V / X]]
- [[aliases/cl-us|CL US]]
- [[aliases/pannacrema-nu-via-nera|PannaCrema Nuàvia Nera]]
- [[aliases/a-and-e-uno|A&E Uno]]
- [[aliases/bufflehead-a1a|Bufflehead A1A]]
- [[aliases/segal|Segal (aliases)]]
- [[aliases/solimo-amazon-kit-baili-db279-identification-conditional-corrected-2026-11-08|Solimo = Amazon kit, Baili DB279 identification CONDITIONAL (corrected 2026-11-08)]]
- [[aliases/carbon-razor-field-carbon-shaving-co|"Carbon" razor field = Carbon Shaving Co]]
- [[aliases/guard-catalog-caron-paris-carbon-shaving-co|GUARD [catalog]: Caron (Paris) ≠ Carbon Shaving Co]]
- [[aliases/carbon-le-variant-folding-catalog|Carbon LE/variant folding [catalog]]]
- [[aliases/canoe-dana-canoe|"Canoe" = Dana Canoe]]
- [[aliases/lv-orage-louis-vuitton-orage|"LV Orage" = Louis Vuitton Orage]]
- [[aliases/brut-faberg-brut|"Brut" = Fabergé Brut]]
- [[aliases/a-and-e-tobacco-road-soap-vs-splash-vs-edp-three-formats-route-carefully|A&E Tobacco Road soap vs splash vs EDP (three formats, route carefully)]]
- [[aliases/cb-v-edp-cb-miracle-edp|CB "V" EdP; CB "Miracle" EdP]]
- [[aliases/wk-washingtons-blend-soap|WK Washington's Blend soap]]
- [[aliases/cl-santal-auster|CL Santal Auster]]
- [[aliases/shannons-indigo-oud-soap|Shannon's Indigo Oud soap]]
- [[aliases/cf-orange-creamsicle-aftershave|CF Orange Creamsicle aftershave]]
- [[aliases/b-and-m-beaudelaire-aftershave|B&M Beaudelaire aftershave]]
- [[aliases/hom-tobacconist-and-dammusi-balms|HoM Tobacconist & Dammusi balms]]
- [[aliases/m-and-m-garda-siochana-soap|M&M Garda Siochana soap]]
- [[aliases/zingari-the-essentials-balm|Zingari "The Essentials" balm]]
- [[aliases/strop-shoppe-baker-street-vs-special-edition|Strop Shoppe Baker Street vs Special Edition]]
- [[aliases/b-and-m-limon-fragrance-environmental-gap380|B&M "Limon" fragrance (Environmental-Gap380)]]
- [[aliases/ethos-success|Ethos Success]]
- [[aliases/stirling-slant-matuhg-mpontiff|"Stirling Slant" (Matuhg, mpontiff]]
- [[aliases/magnet-razor-iamsms-5-introductionmajor655|"Magnet Razor" (iamsms ×5, IntroductionMajor655)]]
- [[aliases/tsm-salve-iamsms-tsm-the-shave-market|"TSM Salve" (iamsms; TSM = The Shave Market]]
- [[aliases/ooo-fahrenheit915-lucky-tiger-ooo|"OoO" (Fahrenheit915 "Lucky Tiger, OoO")]]
- [[aliases/rex-1955|"Rex 1955"]]
- [[aliases/wolfman-wr7|Wolfman WR7]]
- [[aliases/wcs-84|WCS 84]]
- [[aliases/pfte-115u-13a|"PFTE" (115u/13a)]]
- [[aliases/stirling-mita-133u-32a|"Stirling MITA" (133u/32a)]]
- [[aliases/tms-fougere|"TMS Fougere"]]
- [[aliases/tsm-foug-re-chatillon-lux-scent-named-for-the-shave-market-facebook-group|"TSM Fougère" = Chatillon Lux scent NAMED FOR The Shave Market (Facebook group)]]
- [[aliases/caties-bubbles-le-march-du-rasage-the-parallel-tsm-exclusive|Catie's Bubbles "Le Marché du Rasage" = the parallel TSM exclusive]]
- [[aliases/guard-tsm-the-shave-mercantile|GUARD: TSM ≠ The Shave Mercantile]]
- [[aliases/tms-fougere-2|"TMS Fougere" (aliases)]]
- [[aliases/method-note|Method note (aliases)]]
- [[aliases/ag-1889-aim-guerlain-1889-named-for-pattern-established|"AG 1889" = "Aimé Guerlain 1889" — named-for pattern, established]]
- [[aliases/typo-pairs-established|Typo pairs, established]]
- [[aliases/ag-1889-aftershave-skin-food-r-wetshaving-exclusive|"AG 1889 Aftershave Skin food (r/wetshaving exclusive)"]]
- [[aliases/method-note-2|Method note (aliases 2)]]
- [[aliases/magnet-razor-everyday-shaving-stinger|"Magnet Razor" → Everyday Shaving "Stinger"]]
- [[aliases/stinger-ambiguity-guard|"Stinger" ambiguity guard]]
- [[aliases/bare-everyday-razor-ambiguity|Bare "Everyday Razor" ambiguity]]
- [[aliases/stirling-slant|"Stirling Slant"]]
- [[aliases/ooo-oil-of-olay-complete|"OoO" → Oil of Olay Complete]]
- [[aliases/maker-side-title-browser-wayback-read-2026-11-05|Maker-side title (browser Wayback read 2026-11-05)]]
- [[aliases/correction-roller-bar-is-not-a-stinger-variant|CORRECTION — "roller bar" is NOT a Stinger variant]]
- [[aliases/price-timeline-established|Price timeline (established)]]
- [[aliases/twilley-role-refined|Twilley role, refined]]
- [[aliases/magnet-razor-guard-extended|"Magnet Razor" guard, extended]]
- [[aliases/method-note-3|Method note (aliases 3)]]
- [[aliases/glhf-workshop-scent-cluster-fragrance-format-maker-u-pridetwo|GLHF Workshop scent cluster (fragrance format; maker u/pridetwo]]
- [[aliases/aion-trap-gd-scent-vs-aion-skincare-brand|"Aion" TRAP — GD scent vs Aion Skincare brand]]
- [[aliases/b-and-m-cologne-russe|B&M "Cologne Russe"]]
- [[aliases/dr-jons-sakura-musk|Dr. Jon's "Sakura Musk"]]
- [[aliases/method-note-4|Method note (aliases 4)]]
- [[aliases/one-product-canonical-maker-name-succ-s-french-for-success-success-and-succes|ONE product: canonical maker name "Succès" (French for "success"). "Success" and "Succes" are poster spellings of the]]
- [[aliases/maker-side-confirmation-live-store-ethosgroomingessentials-com-products-json|Maker-side confirmation (live store, ethosgroomingessentials.com/products.json, complete ≤250-product read, page 2]]
- [[aliases/fold-rules|Fold rules]]
- [[aliases/f-base-is-a-real-maker-base-name-not-a-product-split|"F Base" is a real maker base name, not a product split]]
- [[aliases/maker-side-typo-noted-not-corrected|Maker-side typo, noted not corrected]]
- [[aliases/method-note-5|Method note (aliases 5)]]
- [[aliases/verdict-the-buyout-is-true-in-substance-wrong-as-framed|VERDICT: the buyout is TRUE IN SUBSTANCE, WRONG AS FRAMED]]
- [[aliases/correction-modern-minora-stainless-is-made-in-russia-ppi-not-egypt|CORRECTION: modern Minora Stainless is made in RUSSIA (PPI), NOT Egypt]]
- [[aliases/razor-fold-rules|Razor fold rules]]
- [[aliases/author-scoped-tags-never-expand-community-wide|Author-scoped tags, never expand community-wide]]
- [[aliases/method-note-6|Method note (aliases 6)]]
- [[aliases/soap-commander-gratitude|Soap Commander "Gratitude"]]
- [[aliases/mls-rubys-garden-dataset-attested-no-web-identity-not-rubys-green|MLS "Ruby's Garden" — dataset-attested, NO web identity; NOT Ruby's Green]]
- [[aliases/correction-2026-11-11-user-ruling-the-never-fold-line-above-is-retired|CORRECTION 2026-11-11 (user ruling — the "never fold" line above is RETIRED)]]
- [[aliases/joserra-noir-noir|Joserra "Noir Noir"]]
- [[aliases/abbate-y-la-mantia-vegano|Abbate y la Mantia "Vegano"]]
- [[aliases/reserve-beta-soapmakers-of-awesometown|"Reserve Beta" → Soapmakers of Awesometown]]
- [[aliases/rex-1955-2|"Rex 1955" (aliases)]]
- [[aliases/wcs-handle-codes|WCS handle codes]]
- [[aliases/method-note-item-15|Method note (item 15)]]
- [[aliases/accuforge-brand-retention-resolved-the-brand-survives-alongside-gem-pdg|AccuForge brand retention — RESOLVED: the brand SURVIVES alongside GEM PDG]]
- [[aliases/accutec-pro-premium-author-scoped-shorthand-not-a-product|"AccuTec Pro Premium" — author-scoped shorthand, NOT a product]]
- [[aliases/cc-lab-blue-dissenter-re-examined-catalog-guidance-unchanged-do-not-split|CC≠Lab Blue dissenter — re-examined; catalog guidance UNCHANGED (do not split)]]
- [[aliases/battle-brothers-watch-check-2026-11-05|Battle Brothers watch check 2026-11-05]]
- [[aliases/narrow-leads-spun-off|Narrow leads spun off]]
- [[aliases/bigfoot-shaves-kit-razor-baili-bd179-br179|Bigfoot Shaves kit razor = Baili BD179/BR179]]
- [[aliases/bigfoot-shaves-blades-maker-still-unpinned-do-not-fold-into-baili-bp007|Bigfoot Shaves blades — maker STILL UNPINNED; do NOT fold into Baili BP007]]
- [[aliases/dataset-re-verified-2026-11-05-full-corpus-field-level|Dataset re-verified 2026-11-05 (full corpus, field-level)]]
- [[aliases/new-leads-2|New leads (aliases)]]
- [[aliases/method-note-7|Method note (aliases 7)]]
- [[aliases/asylum-tallow-soaps-wsp-formula-t-established-by-maker-copy-fingerprint|Asylum tallow soaps = WSP Formula T — ESTABLISHED by maker-copy fingerprint]]
- [[aliases/tallow-line-map-5-scents-soap-125g-splash-100ml|Tallow-line map (5 scents × soap 125g + splash 100ml)]]
- [[aliases/correction-old-virginia-2017-only-was-wrong|CORRECTION: "Old Virginia (2017 only)" was wrong]]
- [[aliases/f-and-m-dataset-scope-corrected|F&M dataset scope corrected]]
- [[aliases/nicepack-s-l-corporate-identity-resolved-maker-side-primary|NicePack, S.L. — corporate identity RESOLVED (maker-side primary)]]
- [[aliases/narrow-leads|Narrow leads (aliases)]]
- [[aliases/method-note-8|Method note (aliases 8)]]
- [[aliases/dr-jons-sunday-funday-extravaganza-is-a-series-tag-strip-it-when-matching|Dr. Jon's "Sunday Funday Extravaganza" is a SERIES tag — strip it when matching]]
- [[aliases/sakura-musk-is-the-sole-attested-wcs-developed-dr-jons-scent|Sakura Musk is the SOLE attested WCS-developed Dr. Jon's scent]]
- [[aliases/west-coast-shaving-has-delisted-dr-jons-entirely-live-check-2026-11-07|West Coast Shaving has delisted Dr. Jon's entirely (live check 2026-11-07)]]
- [[aliases/razwar-dr-jons-scent-for-razwar-attested|"RazWar" — Dr. Jon's scent for razwar, attested]]
- [[aliases/typo-pair|Typo pair]]
- [[aliases/narrow-leads-2|Narrow leads (aliases 2)]]
- [[aliases/method-note-9|Method note (aliases 9)]]
- [[aliases/dg-milksteak-dirtyver-contemplation-established-carryovers-dataset-level|DG Milksteak Dirtyver + Contemplation — ESTABLISHED carryovers (dataset level)]]
- [[aliases/dg-slug-rule-never-read-a-dg-products-base-from-its-shopify-slug|DG slug rule — never read a DG product's base from its Shopify slug]]
- [[aliases/narrow-leads-3|Narrow leads (aliases 3)]]
- [[aliases/method-note-10|Method note (aliases 10)]]
- [[aliases/hom-cirrus-a-one-off-charity-commission-not-a-retail-scent-established|HoM "Cirrus" — a one-off charity commission, NOT a retail scent (established)]]
- [[aliases/hom-indigo-aftershave-exists-established-heavily-used|HoM "Indigo" aftershave EXISTS (established, heavily used)]]
- [[aliases/indigo-is-in-wind-down-at-the-maker-live-store-2026-11-07|Indigo is in wind-down at the maker (live store, 2026-11-07)]]
- [[aliases/ag-1889-delist-date-cdx-retry-one-capture-only-bracket-unchanged|AG 1889 delist-date CDX retry — one capture only, bracket unchanged]]
- [[aliases/narrow-leads-4|Narrow leads (aliases 4)]]
- [[aliases/method-note-11|Method note (aliases 11)]]
- [[aliases/duke-cannon-seneca-real-proper-cologne-launch-scent-established|Duke Cannon "Seneca" — REAL Proper Cologne launch scent (established)]]
- [[aliases/duke-cannon-fulton-the-launch-name-of-grant-rename-established|Duke Cannon "Fulton" = the launch name of Grant — RENAME, established]]
- [[aliases/duke-cannon-randolph|Duke Cannon "Randolph"]]
- [[aliases/oud-mukhallat-catalog-misbrand-corrected|"Oud Mukhallat" catalog misbrand CORRECTED]]
- [[aliases/method-note-12|Method note (aliases 12)]]
- [[aliases/classic-country-barber-classic-country-barbershop|"Classic Country Barber" → "Classic Country Barbershop"]]
- [[aliases/mochachino-is-an-intentional-misspelling-maker-attested|"Mochachino" is an INTENTIONAL misspelling (maker-attested)]]
- [[aliases/tsm-house-line-seven-soaps-one-vegan-base-music-city-suds-made|TSM house line — seven soaps, one vegan base, Music City Suds-made]]
- [[aliases/music-city-suds-has-its-own-shaving-line|Music City Suds has its OWN shaving line]]
- [[aliases/the-simple-life-tsms-house-line-name-lead-grade-membership|"The Simple Life" = TSM's house LINE name (lead-grade membership)]]
- [[aliases/no-tsm-exclusives-for-other-artisans-established-by-complete-store-read|No TSM exclusives for other artisans (established by complete-store read)]]
- [[aliases/narrow-leads-5|Narrow leads (aliases 5)]]
- [[aliases/method-note-13|Method note (aliases 13)]]
- [[aliases/coast-fragrance-and-shave-soaps-resolved-as-a-real-micro-brand-catalog|Coast Fragrance and Shave Soaps — RESOLVED as a real micro-brand [catalog]]]
- [[aliases/terra-and-tallow|Terra & Tallow]]
- [[aliases/method-note-14|Method note (aliases 14)]]
- [[aliases/correction|CORRECTION (aliases)]]
- [[aliases/sly-sloth-soaps-resolved-workshop-candidate-only-never-a-product|"Sly Sloth Soaps" — RESOLVED: workshop candidate only, never a product]]
- [[aliases/etsy-listing-names-as-evidence|Etsy listing names as evidence]]
- [[aliases/cdx-correction|CDX correction]]
- [[aliases/method-note-15|Method note (aliases 15)]]
- [[aliases/qcv-quatre-cent-vingt-resolved|"QCV" = Quatre Cent Vingt (RESOLVED)]]
- [[aliases/abbreviation-fold-rules-dataset-census-6-993-cb-rows|Abbreviation fold rules (dataset census, 6,993 CB rows)]]
- [[aliases/tonsorium-fougere-tonsorium-author-scoped-descriptor|"Tonsorium Fougere" = Tonsorium (author-scoped descriptor)]]
- [[aliases/guy-noir-cb-lead-do-not-fold-anywhere|"Guy Noir" (CB) — LEAD, do not fold anywhere]]
- [[aliases/wcs-chypre-oriental-cologne-cb-made-luxury-cream-established|WCS Chypre/Oriental/Cologne = CB-made Luxury Cream (established)]]
- [[aliases/promotion-gaps-no-verified-entry-in-any-format|Promotion gaps (no verified entry in any format)]]
- [[aliases/image-only-maker-names-cdx-batch-1-zero-dataset-strings|Image-only maker names (CDX batch 1, zero dataset strings)]]
- [[aliases/irish-cream-as-a-cb-name-poster-paraphrase-only|"Irish Cream" as a CB name = poster paraphrase only]]
- [[aliases/method-note-16|Method note (aliases 16)]]
- [[aliases/narrow-leads-6|Narrow leads (aliases 6)]]
- [[aliases/dfs-2017-l-and-l-groomings-damn-fine-shave-forum-limited-edition-established|"DFS 2017" = L&L Grooming's Damn Fine Shave forum limited edition (established)]]
- [[aliases/guard-dfs-2017-is-two-products-one-per-maker|GUARD — "DFS 2017" is TWO products, one per maker]]
- [[aliases/vegan-on-a-post-july-2016-l-and-l-dg-soap-string-pre-bison-puck-never-a|"Vegan" on a post-July-2016 L&L/DG soap string = pre-bison puck, never a parallel line]]
- [[aliases/cl-parfums-wind-down-recheck-2026-11-08-01-11-cst-no-change|CL Parfums wind-down recheck 2026-11-08 01:11 CST — NO CHANGE]]
- [[aliases/narrow-leads-7|Narrow leads (aliases 7)]]
- [[aliases/method-note-17|Method note (aliases 17)]]
- [[aliases/men-barbiere-brush-omega-made|Men-Ü Barbiere brush = Omega-made]]
- [[aliases/proraso-travel-boar-omega-50068-bambino-third-measurement|Proraso travel boar = Omega 50068 Bambino — third measurement]]
- [[aliases/imperial-barber-products-brand-pinned-see-lineages-md|Imperial Barber Products — brand pinned (see lineages.md)]]
- [[aliases/pereira-boar-semogue-rechecked-still-a-lead|Pereira boar = Semogue — rechecked, still a LEAD]]
- [[aliases/narrow-leads-8|Narrow leads (aliases 8)]]
- [[aliases/method-note-18|Method note (aliases 18)]]
- [[aliases/the-club-black-is-two-products-never-fold-across-them|"The Club Black" is TWO products — never fold across them]]
- [[aliases/brand-of-record-rule-for-the-line|Brand-of-record rule for the line]]
- [[aliases/the-club-scent-program-vip-exclusives-a-and-e-made|The Club scent program (VIP exclusives, A&E-made)]]
- [[aliases/premise-corrections|Premise corrections]]
- [[aliases/narrow-leads-9|Narrow leads (aliases 9)]]
- [[aliases/method-note-19|Method note (aliases 19)]]
- [[aliases/longer-handle-link-second-attested-still-single-author|Longer-handle link SECOND-ATTESTED, still single-author]]
- [[aliases/solimo-kit-db279-downgraded-to-conditional|Solimo-kit = DB279 DOWNGRADED to conditional]]
- [[aliases/dataset-re-census-full-corpus-240-951-rows-through-2026-11-06|Dataset re-census (full corpus, 240,951 rows through 2026-11-06)]]
- [[aliases/retail-route-exhausted-this-run|Retail route exhausted this run]]
- [[aliases/narrow-leads-10|Narrow leads (aliases 10)]]
- [[aliases/method-note-20|Method note (aliases 20)]]
- [[aliases/tek-is-canonical-maker-spelling|Tek is canonical (maker spelling)]]
- [[aliases/tech-without-b1-tek-as-a-loose-alias|"Tech" without B1 → Tek as a LOOSE alias]]
- [[aliases/b1-tech-the-b1-family-never-the-tek-entry|"B1 Tech" → the B1 family, NEVER the Tek entry]]
- [[aliases/sbs-guard|SBS guard]]
- [[aliases/el-jefe|El Jefe (aliases)]]
- [[aliases/narrow-leads-11|Narrow leads (aliases 11)]]
- [[aliases/the-coast-soap-scents-came-from-the-cologne-line-established|The Coast soap scents came from the cologne line (established)]]
- [[aliases/marrakech-oud-grasse-rose-cologne-only-zero-footprint|Marrakech (Oud) + Grasse (Rose) — cologne-only, zero footprint]]
- [[aliases/terra-soap-unscented-only-established|Terra soap = Unscented only (established)]]
- [[aliases/recipe-3|"Recipe #3"]]
- [[aliases/coast-tub-packaging|Coast tub packaging]]
- [[aliases/coast-soap-price-guard|Coast soap price guard]]
- [[aliases/method-note-21|Method note (aliases 21)]]
- [[aliases/indigo-splash-balm-delist-bracket-only-after-2025-11-05-before-2026-11-07|Indigo splash/balm delist — BRACKET only: after 2025-11-05, before 2026-11-07]]
- [[aliases/indigo-soap-the-may-2025-flicker|Indigo soap — the May-2025 flicker]]
- [[aliases/indigo-edp-discontinuation-bracket-2025-08-23-2026-08-27|Indigo EdP discontinuation — BRACKET: 2025-08-23 → 2026-08-27]]
- [[aliases/the-scents-only-live-sku-is-the-1-2oz-tusk-soap-sample|The scent's only live SKU is the 1/2oz Tusk soap sample]]
- [[aliases/method-note-22|Method note (aliases 22)]]
- [[aliases/program-list-corrected-30-scents-not-14|Program list CORRECTED — 30 scents, not 14]]
- [[aliases/fold-rules-club-a-and-e-migration-series|Fold rules — Club↔A&E migration series]]
- [[aliases/boo-one-scent-boo-is-punctuation|BOO = one scent; "BOO!!" is punctuation]]
- [[aliases/chalkys-charkys-midnight-special-one-authors-private-label|"Chalky's / Charky's Midnight Special" = one author's private label]]
- [[aliases/francisco-caties-bubbles-made-club-channel-dupe-paco-rabanne-pour-homme-1973|Francisco = Catie's Bubbles-made, Club-channel; dupe = Paco Rabanne Pour Homme (1973)]]
- [[aliases/charlatans-traipse-count-the-apostrophe-form|Charlatans Traipse — count the apostrophe form]]
- [[aliases/a-cold-day-in-hell-vs-a-cold-day-in-hell-2-two-products|A Cold Day In Hell vs A Cold Day...In Hell 2 — TWO products]]
- [[aliases/post-shave-serum-no-3-single-author-no-siblings|Post Shave Serum No 3 — single-author, no siblings]]
- [[aliases/collision-guards|Collision guards]]
- [[aliases/delisted-at-retail-set-live-nov-2026|Delisted-at-retail set (live Nov 2026)]]
- [[aliases/unverified-only-promotion-evidence-catalogmerged-json-oct-21-export|Unverified-only promotion evidence (catalogmerged.json, Oct 21 export)]]
- [[aliases/method-note-23|Method note (aliases 23)]]
- [[aliases/correction-the-recipe-is-aftershave-only-no-soap-entry-is-owed|CORRECTION — The Recipe is AFTERSHAVE-ONLY; no soap entry is owed]]
- [[aliases/pedro-fiasco-marzipan-a-scent-of-pedro-fiascos-legendary-soap|Pedro Fiasco "Marzipan" = a scent of Pedro Fiasco's Legendary soap]]
- [[aliases/method-note-24|Method note (aliases 24)]]
- [[aliases/maker-store-delist-brackets-aegrooming-com|Maker-store delist brackets (aegrooming.com)]]
- [[aliases/correction-amber-rose-began-at-the-club-2018-not-at-a-and-e-retail|CORRECTION — Amber Rose began at the Club (2018), not at A&E retail]]
- [[aliases/boca-negra-parfum-extrait-a-club-vip-fragrance-product-not-a-soap-splash-variant|Boca Negra Parfum Extrait = a Club VIP FRAGRANCE product, not a soap/splash variant]]
- [[aliases/gothic-quarter-barcelona-the-club-listing-name-a-and-e-retail-the-gothic-quarter|"Gothic Quarter Barcelona" = the Club-listing name; A&E retail = "The Gothic Quarter"]]
- [[aliases/method-note-25|Method note (aliases 25)]]
- [[aliases/hema-de-blades-rebranded-personna-resolved-established-era-split|HEMA DE blades = rebranded Personna — RESOLVED (established, era-split)]]
- [[aliases/everclear-blue-blades-a-separate-vintage-hema-house-brand-not-the-modern-blade|"Everclear Blue Blades" = a SEPARATE vintage HEMA house brand, not the modern blade]]
- [[aliases/correction-to-the-backlog|CORRECTION to the backlog]]
- [[aliases/hema-aftershave-balm|HEMA aftershave balm]]
- [[aliases/method-note-26|Method note (aliases 26)]]
- [[aliases/francisco-dupe-target-resolved-paco-rabanne-pour-homme-1973-jean-martel|Francisco dupe target RESOLVED — Paco Rabanne Pour Homme (1973, Jean Martel)]]
- [[aliases/collision-guard-francisco-is-a-three-way-namespace|Collision guard — "Francisco" is a three-way namespace]]
- [[aliases/method-note-27|Method note (aliases 27)]]
- [[aliases/gothic-quarter-a-and-e-side-wayback-verdict-zero-captured-maker-store-pages-ever|Gothic Quarter — A&E-side Wayback verdict: zero captured maker-store pages ever]]
- [[aliases/dirty-ginger-cream-slugs-both-real-parallel-listings|Dirty Ginger cream slugs — both real, parallel listings]]
- [[aliases/five-scent-late-capture-recheck-no-change|Five-scent late-capture recheck — no change]]
- [[aliases/method-note-28|Method note (aliases 28)]]
- [[aliases/singles-the-audits-zero-dataset-strings-yet-is-wrong|"Singles" — the audit's "zero dataset strings yet" is WRONG]]
- [[aliases/singles-line-maker-listing-evidence-on-file-club-store-live-2026-11-09|Singles line — maker-listing evidence on file (Club store, live 2026-11-09)]]
- [[aliases/method-note-29|Method note (aliases 29)]]
- [[aliases/imperial-travel-shave-brush-promotion-ready-two-sku-split|Imperial Travel Shave Brush — promotion-ready, two-SKU split]]
- [[aliases/pereira-metal-brush|Pereira metal brush]]
- [[aliases/method-note-30|Method note (aliases 30)]]
- [[aliases/charky-peter-charkaliss-nickname-established-daily-lather-2017|"Charky" = Peter Charkalis's nickname — ESTABLISHED (Daily Lather, 2017)]]
- [[aliases/chalky-engineeredshaves-typo-of-charky-established|"Chalky" = EngineeredShave's typo of "Charky" — ESTABLISHED]]
- [[aliases/method-note-31|Method note (aliases 31)]]
- [[aliases/the-wood-still-single-author-stays-unverified-catalog|"The Wood" — still single-author, stays unverified [catalog]]]
- [[aliases/the-wood-woods-and-spices-fold-rule-never-fold-catalog|"The Wood" ≠ "Woods & Spices" — fold rule: NEVER fold [catalog]]]
- [[aliases/wood-and-spice-singular-woods-and-spices-title-variant-catalog|"Wood & Spice" (singular) = "Woods & Spices" title variant [catalog]]]
- [[aliases/method-note-32|Method note (aliases 32)]]
- [[aliases/the-wood-listing-cdx-is-inconclusive-catalog|The Wood listing — CDX [] is INCONCLUSIVE [catalog]]]
- [[aliases/the-recipe-launch-still-unpinned-catalog|The Recipe launch — still unpinned [catalog]]]
- [[aliases/method-note-33|Method note (aliases 33)]]
- [[aliases/cherry-soda-cherry-cola-fold-catalog|"Cherry Soda" → Cherry Cola, FOLD [catalog]]]
- [[aliases/dirty-ginger-handle-rule-never-fold-on-handle-evidence-catalog|Dirty Ginger handle rule — NEVER fold on handle evidence [catalog]]]
- [[aliases/gothic-quarter-aftershave-merge-then-promote-catalog|Gothic Quarter aftershave — MERGE then PROMOTE [catalog]]]
- [[aliases/the-recipe-soap-entry-owed-aftershave-attestation-stale-catalog|The Recipe — soap entry OWED, aftershave attestation STALE [catalog]]]
- [[aliases/method-note-34|Method note (aliases 34)]]
- [[aliases/st-ha-maker-established-expansions|ST / HA — maker-established expansions]]
- [[aliases/stirling-stainless-stirling-stainless-de-stainless-handle-de-razor|"Stirling Stainless" / "Stirling Stainless DE" ≠ "Stainless Handle DE Razor"]]
- [[aliases/handle-name-trap-austin-dallas-fort-worth-are-shared-handle-names|Handle-name trap — Austin / Dallas / Fort Worth are shared handle names]]
- [[aliases/stirling-slant-fold-rules-restated|"Stirling Slant" — fold rules restated]]
- [[aliases/serial-strings-are-plate-batch-sequence|Serial strings are plate+batch+sequence]]
- [[aliases/method-note-35|Method note (aliases 35)]]
- [[aliases/hom-indigo-edp-page-removed-not-merely-discontinued|HoM Indigo EdP — page REMOVED, not merely discontinued]]
- [[aliases/indigo-soap-unavailable-on-2025-10-12-new-capture-read|Indigo soap — unavailable on 2025-10-12 (new capture read)]]
- [[aliases/splash-handle-pinned|Splash handle pinned]]
- [[aliases/method-note-36|Method note (aliases 36)]]
- [[aliases/vshod-custom-manchurian-shaving-brush-01-048|vshod "CUSTOM MANCHURIAN SHAVING BRUSH 01–048"]]
- [[aliases/guard-bare-custom-manchurian-is-not-the-vshod-line|GUARD — bare "Custom Manchurian" is NOT the vshod line]]
- [[aliases/cl-parfums-wind-down-watch-e-rechecked-2026-11-09-23-15-cst-no-change|CL Parfums wind-down watch (e) RECHECKED 2026-11-09 23:15 CST — NO CHANGE]]
- [[aliases/101-og1-certain-design-identity-chronology|"101" → OG1 (certain, design identity + chronology)]]
- [[aliases/102-stays-its-own-entry-x3-never-folds-into-102|"102" stays its own entry; X3 NEVER folds into 102]]
- [[aliases/el-jefe-ac-format-entry|"El Jefe" → AC-format entry]]
- [[aliases/sbs-design-gloss|SBS design gloss]]
- [[aliases/dual-comb-ikons-dual-function-head|"Dual Comb" = iKon's dual-function head]]
- [[aliases/b1-oss-vs-og1-guard|"B1 OSS" vs "OG1" guard]]
- [[aliases/black-birch-stout-maker-notes-on-file-entries-owed|"Black Birch Stout" — maker notes on file; entries owed]]
- [[aliases/pedro-fiascos-legendary-one-product-four-scent-variants|Pedro Fiasco's Legendary = ONE product, FOUR scent variants]]
- [[aliases/gothic-quarter-delist-date-wayback-route-closed-validated-negative|Gothic Quarter delist date — Wayback route CLOSED (validated negative)]]
- [[aliases/singles-5-products-amplifier-is-edp-only|"Singles" = 5 products, Amplifier is EdP-only]]
- [[aliases/re-verified-no-change|Re-verified, no change]]
- [[aliases/cb-metal-tags-are-attributes-never-entries-with-launch-brackets-now-pinned|CB metal tags are attributes, never entries — with launch brackets now pinned]]
- [[aliases/bison-ss-bison-stainless-bison-stainless-steel-razor-karve-bison-fold-as|"Bison SS" / "Bison Stainless" / "Bison Stainless Steel" → razor/karve-bison, FOLD as material attribute]]
- [[aliases/overlander-metal-scope-note|Overlander metal scope note]]
- [[aliases/method-note-37|Method note (aliases 37)]]
- [[aliases/re-verified-no-change-2|Re-verified, no change (aliases)]]
- [[aliases/foutere|"Foutere"]]
- [[aliases/bare-tsm-fold-rule-corrected|Bare "TSM" fold rule, corrected]]
- [[aliases/tsm-group-buy-commissioned-strings-fold-never-separate-entries|TSM group-buy / commissioned strings — fold, never separate entries]]
- [[aliases/tsm-custom-brushes-are-group-program-items-not-maker-lines|TSM custom brushes are group-program items, not maker lines]]
- [[aliases/re-verified-no-change-3|Re-verified, no change (aliases 2)]]
- [[aliases/cl-tsm-unconditional-surrender|"CL - TSM - Unconditional Surrender"]]
- [[aliases/clux-tsm-y-r-p-the-plain-chatillon-lux-yuzu-rose-patchouli-aftershave-entry|"CLux TSM Y/R/P" → the plain Chatillon Lux Yuzu/Rose/Patchouli aftershave entry]]
- [[aliases/method-the-group-other-scent-carryover-pattern|METHOD — the "GROUP - <other scent>" carryover pattern]]
- [[aliases/unconditional-surrender-date-guards|Unconditional Surrender date guards]]
- [[aliases/re-verified-no-change-4|Re-verified, no change (aliases 3)]]
- [[aliases/barrister-and-mann-tsm-2015-cologne-russe|"Barrister & Mann/TSM 2015 Cologne Russe"]]
- [[aliases/tsm-straight-by-daniel-arman-maker-level-only-no-entry-p-19|"TSM straight by Daniel Arman" → maker-level only, no entry (P-19)]]
- [[aliases/tsm-numbered-customs-series-map-corrected|TSM numbered Customs — series map corrected]]
- [[aliases/tsm-blue-with-synth-majorhawkicedagger-june-2020-3|"TSM Blue with synth" (majorhawkicedagger, June 2020 ×3)]]
- [[aliases/dg-trismegistus-tsm-group-buy|DG Trismegistus TSM group buy]]
- [[aliases/cologne-russe-launch-base-white-label-established|Cologne Russe launch base = White Label, ESTABLISHED]]
- [[aliases/cologne-russe-base-arc-scent-base-key-white-label-sep-2015|Cologne Russe base arc (scent+base key): White Label (Sep 2015)]]
- [[aliases/cologne-russe-delisted-feb-2024|Cologne Russe DELISTED Feb 2024]]
- [[aliases/method-note-38|Method note (aliases 38)]]
- [[aliases/full-measurement-of-man-the-full-measure-of-man-misspelling|"Full Measurement of Man" → "The Full Measure of Man" (misspelling)]]
- [[aliases/full-measure-of-a-man-third-name-variant-author-scoped|"Full Measure of a Man" — third name variant (author-scoped)]]
- [[aliases/bare-cool-reserve-cool|Bare "Cool" = Reserve Cool]]
- [[aliases/lavender-black-label-black-label-era-tag-not-a-variant|"Lavender (Black Label)" = Black Label era tag, not a variant]]
- [[aliases/lime-lavender-and-cedarwood-lavender|"Lime, Lavender, and Cedarwood" ≠ Lavender]]
- [[aliases/russe-cologne-russe-short-form-verified|"Russe" = Cologne Russe (short form, verified)]]
- [[aliases/re-verified-no-change-5|Re-verified, no change (aliases 4)]]
- [[aliases/behind-the-whatsis|"behind the whatsis"]]
- [[aliases/b-and-m-whatsis-excelsior-verified-soap-entry-excelsior-era-tag|"B&M Whatsis Excelsior" → verified soap entry (Excelsior-era tag)]]
- [[aliases/behold-the-whatsis-reborn-the-whatsis-family-lockharts-channel|"Behold the Whatsis! Reborn" → the Whatsis family (Lockhart's channel)]]
- [[aliases/whatsis-whatsis-capitalization-is-noise|"WhatsIs" / "whatsis" capitalization is noise]]
- [[aliases/fragrance-entry-flag-validators-not-a-fold|Fragrance-entry FLAG (validators, not a fold)]]
- [[aliases/dedup-flags-validators|Dedup flags (validators)]]
- [[aliases/method-note-39|Method note (aliases 39)]]
- [[aliases/re-verified-no-change-6|Re-verified, no change (aliases 5)]]
- [[aliases/correction-full-measure-of-a-man-is-not-author-scoped-not-2-rows|CORRECTION — "Full Measure of a Man" is NOT author-scoped, NOT 2 rows]]
- [[aliases/b-and-m-hand-and-body-soap-shaving-soap-never-fold-across-the-line|B&M Hand & Body Soap ≠ shaving soap (never fold across the line)]]
- [[aliases/b-and-m-samhain-verified-soap-barrister-and-mann-samhain-aftershave-entry-owed|B&M Samhain → verified soap/barrister-and-mann-samhain; aftershave entry OWED]]
- [[aliases/whatsis-7b-confirmed-madflava81s-2022-excelsior-is-template-carryover|Whatsis (7b) CONFIRMED — Madflava81's 2022 "(Excelsior)" is template carryover]]
- [[aliases/whatsis-7d-confirmed-whats-it-alias-is-on-the-verified-soap-entry|Whatsis (7d) CONFIRMED — "Whats It" alias IS on the verified soap entry]]
- [[aliases/method-note-40|Method note (aliases 40)]]
- [[aliases/re-verified-no-change-7|Re-verified, no change (aliases 6)]]
- [[aliases/sunny-lane-verified-soap-barrister-and-mann-sunny-lane|Sunny Lane → verified soap/barrister-and-mann-sunny-lane]]
- [[aliases/figarose-verified-soap-barrister-and-mann-figarose|Figarose → verified soap/barrister-and-mann-figarose]]
- [[aliases/correction-2|CORRECTION (aliases 2)]]
- [[aliases/method-note-41|Method note (aliases 41)]]
- [[aliases/re-verified-no-change-8|Re-verified, no change (aliases 7)]]
- [[aliases/sessions-series-canonical-series-title-maker|"Sessions Series" = canonical series title (maker)]]
- [[aliases/kanno-new-entry-owed-soap-aftershave-owed|Kanno → NEW entry owed (soap) + aftershave owed]]
- [[aliases/king-two-walters-waits-verified-sessions-soaps-aftershaves-owed|King / Two Walters / Waits → verified Sessions soaps; aftershaves owed]]
- [[aliases/little-walker-misspelling-of-little-walter-harmonica-player|"Little Walker" = misspelling of Little Walter (harmonica player)]]
- [[aliases/bare-king-is-ambiguous-never-auto-fold|Bare "King" is AMBIGUOUS — never auto-fold]]
- [[aliases/re-verified-no-change-9|Re-verified, no change (aliases 8)]]
- [[aliases/snippid-is-two-products-sharing-a-scent-name-format-disambiguates|"Snippid" is TWO products sharing a scent name — format disambiguates]]
- [[aliases/hom-mull-no-alias-work-needed|HoM "Mull" — no alias work needed]]
- [[aliases/re-verified-no-change-10|Re-verified, no change (aliases 9)]]
- [[aliases/correction-3|CORRECTION (aliases 3)]]
- [[aliases/hom-mull-community-first-impression-consensus-sweet-mulled-wine|HoM "Mull" — community first-impression consensus: SWEET mulled wine]]
- [[aliases/mull-false-positive-guards-for-the-matcher|"Mull" false-positive guards (for the matcher)]]
- [[aliases/method-note-42|Method note (aliases 42)]]
- [[aliases/re-verified-no-change-11|Re-verified, no change (aliases 10)]]
- [[aliases/sawdust-creations-name-forms-fold-rules|Sawdust Creations name forms — fold rules]]
- [[aliases/sawdust-false-positive-guard|"Sawdust" false-positive guard]]
- [[aliases/method-note-43|Method note (aliases 43)]]
- [[aliases/hom-mull-etymology-resolved-maker-attested|HoM "Mull" — etymology RESOLVED, maker-attested]]
- [[aliases/b-and-m-sessions-series|B&M Sessions Series]]
- [[aliases/bare-waits-soap-strings-fold-to-sessions-waits|Bare "Waits" soap strings fold to Sessions Waits]]
- [[aliases/hom-smash-dual-attribution-strings-perfumer-credit|HoM "Smash" — dual-attribution strings + perfumer credit]]
- [[aliases/hom-beloved-dating-correction|HoM "Beloved" — dating CORRECTION]]
- [[aliases/hom-dinosmores-spelling-variants|HoM "DinoS'mores" spelling variants]]
- [[aliases/hom-kryptonite-2-vs-kryptonite-validator-check-not-a-fold-rule|HoM "Kryptonite 2" vs "Kryptonite" — validator check, not a fold rule]]
- [[aliases/method-note-44|Method note (aliases 44)]]
- [[aliases/hom-kryptonite-2-is-a-distinct-product|HoM "Kryptonite 2" is a DISTINCT product]]
- [[aliases/the-verified-fragrance-house-of-mammoth-kryptonite-entry-is-the-v2-edp-under|The verified fragrance/house-of-mammoth-kryptonite entry is the v2 EdP under the v1 name]]
- [[aliases/kryptonite-v2-green-the-v2-soap-green-is-a-v2-marker|"Kryptonite V2 (green)" = the v2 soap; "green" is a v2 marker]]
- [[aliases/kryptonite-26mm-brush-strings-are-not-kryptonite-2|"Kryptonite 26mm" brush strings are NOT Kryptonite 2]]
- [[aliases/corrections-to-the-13-06-runs-kryptonite-2-entry-same-file-superseded|CORRECTIONS to the 13:06 run's Kryptonite 2 entry (same file, superseded)]]
- [[aliases/method-note-45|Method note (aliases 45)]]
- [[aliases/v2-splash-retail-listing-the-maker-page-archived|v2 splash retail listing = the maker page, archived]]
- [[aliases/v2-soap-retail-listing-the-same-slug-retitled|v2 soap retail listing = the SAME slug, retitled]]
- [[aliases/maggard-never-stocked-v2-weak-negative|Maggard never stocked v2 (weak negative)]]
- [[aliases/method-note-46|Method note (aliases 46)]]
- [[aliases/smash-merge-list-p-16-7-verified-entries-are-3-products|Smash — MERGE LIST (P-16): 7 verified entries are 3 products]]
- [[aliases/you-and-i-will-die-launched-october-4-2024|You & I (Will Die) launched October 4, 2024]]
- [[aliases/shire-2-launched-april-2023|Shire 2 launched April 2023]]
- [[aliases/beloved-launched-april-2022|Beloved launched April 2022]]
- [[aliases/kryptonite-v2-soap-delisted-from-the-live-store-bracket-oct-12-2025-nov-11-2026|Kryptonite v2 soap DELISTED from the live store (bracket Oct 12, 2025 – Nov 11, 2026)]]
- [[aliases/c-and-h-hom-you-and-i-will-die-brushes-entry-owed|C&H × HoM "You & I (Will Die)" brushes — entry owed]]
- [[aliases/method-note-47|Method note (aliases 47)]]
- [[aliases/fragrantica-house-of-mammoth-audit-full-table-9-pages|Fragrantica House of Mammoth audit — full table (9 pages)]]
- [[aliases/santa-noir-launch-nov-dec-2021|Santa Noir launch = Nov/Dec 2021]]
- [[aliases/f-d-o-launch-january-2022-full-line|Fú Dào launch = January 2022, full line]]
- [[aliases/tobacconist-launch-april-2021|Tobacconist launch = April 2021]]
- [[aliases/indigo-launch-december-2018-as-mood-indigo|Indigo launch = December 2018 as "Mood Indigo."]]
- [[aliases/embrace-launch-2021-everett-launch-spring-2024|Embrace launch = 2021; Everett launch = spring 2024]]
- [[aliases/dinosmores-entries-exist-no-gap|DinoS'mores entries exist — no gap]]
- [[aliases/method-notes|Method notes]]
- [[aliases/abbraccio-is-a-real-brush-distinct-from-embrace|"Abbraccio" is a REAL brush, distinct from Embrace]]
- [[aliases/embraced-putneycjs-pet-name-for-his-embrace-brush|"Embraced" = putneycj's pet name for his Embrace brush]]
- [[aliases/femur-lead-do-not-create-an-entry|"Femur" — LEAD, do NOT create an entry]]
- [[aliases/fu-dao-flare-the-fu-dao-brush-in-the-flare-handle-shape|"Fu Dao Flare" = the Fu Dao brush in the Flare handle shape]]
- [[aliases/c-and-h-house-handles-named-after-hom-scents-date-coin-disambiguate|C&H house handles named after HoM scents — date + coin disambiguate]]
- [[aliases/mango-wood-handle-material-never-a-scent-or-line|"Mango Wood" = handle material, never a scent or line]]
- [[aliases/grizzly-bay-shire-shire-2-second-brush-maker|Grizzly Bay Shire = Shire 2 (second brush maker)]]
- [[aliases/druidia-mammoth-tobacconist-is-not-a-c-and-h-hom-brush|Druidia × Mammoth Tobacconist is NOT a C&H × HoM brush]]
- [[aliases/mammoth-coin-numbers-xxxxmc-date-collab-brushes|Mammoth coin numbers (xxxxMC) date collab brushes]]
- [[aliases/fanchurian-version-brush-identity|Fanchurian version ≠ brush identity]]
- [[aliases/mammoth-tusk-lead-single-row|"Mammoth Tusk" — LEAD, single row]]
- [[aliases/watches-rechecked-this-run|Watches rechecked this run]]
