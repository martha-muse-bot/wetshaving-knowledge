---
title: "Product lines"
tags:
  - index
---

Posters often type the LINE name alone. Lines and soap bases behave
like knot generations: identity, not decoration.

**[catalog]** TSF = Talent Soap Factory (Etsy artisan, maker Aaron; see
lineages.md). The vegan line iterates roughly once a year (RedMosquitoMM
2025-03-11 firsthand: "TSF iterates on their soap base regularly — about
once a year as far as I can tell"), so base = an era attribute (P-03/P-17),
never a product split:

**Scope:** full-corpus census over sotd_2016–2026_full.json (240,951 rows): 6,993 CB rows / 1,781 distinct strings, normalized to 119 clean scent clusters ≥5 rows; plus TryThatSoap collection mining (62 CB collections, TTS 112–2636) and two Wayback CDX slices of catiesbubbles.com. Catalog state 2026-11-07: 493 CB entries (219 verified, 119 verified soap). Full census + TTS list + CDX inventory saved in the goal's hidden_files (`cb_scent_audit_2026-11-07.txt`).
**Brand facts (ShaveSplash interview with Chris Cullen, 2026-03-19, primary-ish):** founded **2013** by **Chris Cullen**, named after his daughter Catie; one-person handmade operation ("every soap/aftershave/perfume is made by hand by one person, me"); NJ / Jersey influence — Blugere and Pine Barrens are the most Jersey-shaped scents; Barnegat Bay = fairly traditional bay rum. **Le Piment de la Vie launched 2014**, still bestseller in 2023. **322 "started as a joke**, yet it became a real fragrance." **Top of the World made with Matt at Teton Shaves.** Newer scent worlds named: Top of the World, Daydream. **No new scents imminent as of March 2026** ("creative deserts… nothing close to completion"). Bases over the years: Italian, French, French+ (jojoba oil, pricier), Luxury (cream), Premium (kokum + mango seed butter), Luxury Hard Soap 2oz — base is an era/format attribute, never the scent identity; the 2oz Luxury Hard Soap line is maker-attested via CDX popup images (LTV, LPV, UJG, Spanish Holiday, RDM, BB, AMD, Irish Coffee, PGF, TP, 95LL, Waterlyptus).
**The "CB <X>" abbreviation pattern (for the matcher):** posters abbreviate the brand AND the scent freely — LPV = Le Piment de la Vie (15 rows/10a), LTV = La Terre Verte, LMR = Le Marché du Rasage (14 rows/8a), CT Shade = Connecticut Shade (45 rows/3a), QCV = Quatre Cent Vingt (see below), CB V / CB X / CB 322 / CB Blugere / CB Porch Drinks / CB Two to Mango. **All abbreviations are scent-scoped, never auto-expanded outside CB strings** — "CB" itself is field-dependent (razor field "CB razor" = Karve Christopher Bradley, glossary.md). French names are routinely misspelled (Le Marche Du Rassage, Le Piement, Menage a Lavende, "Quatre Cent Vignt") — fold on the canonical spelling, never create entries on misspellings.
**QCV = Quatre Cent Vingt — RESOLVED [catalog]:** QCV is the initialism (Quatre-Cent-Vingt = 420). B&B 411774: "Quatre Cent Vignt translates to '4:20' and smells like… flowering cannabis"; Fragrantica: Quatre Cent Vingt launched 2017, cannabis top note, "a soft floral, but unisex fougere accented with the smell of a young cannabis flower" (maker's own note). Dataset QCV: 9 rows / 5 authors, 2016–2018 (vacaloca: "Very cannabis up front but then evolves into a fougere"; eaterofworld's 4/20 posts). **Fold all QCV clusters into the Quatre Cent Vingt entries** (soap/aftershave/fragrance); never a separate QCV entry. Note the launch-date tension: QCV soap strings predate Fragrantica's 2017 EdP launch — the soap may predate the fragrance launch; do not cite 2017 as the soap's launch.
**Promotion-ready gaps (no verified entry in any format; evidence on file):**

**WCS (West Coast Shaving) exclusives — CB-made [catalog]:** three Luxury Cream scents, TTS 1086/1087/1089: **Chypre** (many rows, jpq3366/shredsofmetal/chefkoolaid/bloodcrab/AntwonPeachFuzz, 2019–2023, soap + splash; jpq3366's note "Excited to finally try Catie's Bubbles soap" on a "WCS Chypre jojoba shaving cream" row pins the maker), **Oriental** (many rows, reguyw_nothingtolose/Mochee38/cowzilla3, 2019–2021; a matching EdT existed per reguyw_nothingtolose), **Cologne** (1 row, 2019). Catalog has verified `west-coast-shaving-chypre` entries (soap/aftershave/fragrance) — validators add CB as the manufacture attribute on the cream-era entries. **The 2023 "WCS Chypre (Duck Fat)" row is a different base era** — do not fold the duck-fat variant into the CB-made Luxury Cream entry without a base-era split. No dedicated WCS Oriental/Cologne CB entries exist — owed on TTS + dataset evidence.
**Leads (do NOT promote on current evidence):**

**Maker-site evidence route [catalog]:** catiesbubbles.com is Zen Cart + WAF — homepage fetches, category pages 403 for text fetch (backlog item (f) 2026-11-02 note still stands). **Wayback CDX is the working route:** two slices pulled 2026-11-07 (batch 1: `catiesbubbles.com*` limit 400 — admin + /images/ only, no product pages; batch 2: `catiesbubbles.com/index.php*` limit 200 JSON — the limit=1000 text query 504'd). Categories (cPath): 65, 65_77, 65_80, 65_83, 66, 67, 68, 69 (+69_66/68/72/74/75), 72, 101 (+101_91/97/99/100/102–114). Product IDs seen: 182–219, 280–285, 297–307, 325–332, 340, 352, 359, 374–376, 381–383, 391–394, 404–437, 441, 448, 478, 489, 499–500, 521–523, 586–587, 596–598, 600, 603–604, 641–646 (DFTR = 615, beyond this slice). Validators: Wayback-read the product_info pages by products_id for primary evidence; retry the limit=1000 CDX pull when IA is stable for the full inventory.

## Product lines

- [[lines/mitchells-wool-fat-formula-eras-established-2026-10-22|Mitchell's Wool Fat — formula eras (established 2026-10-22)]]
- [[lines/wholly-kaw-base-progression-established-2026-10-21-22|Wholly Kaw — base progression (established 2026-10-21/22)]]
- [[lines/cold-river-soap-works-lines-and-bases|Cold River Soap Works — lines & bases]]
- [[lines/seaforth|Seaforth!]]
- [[lines/black-ship-grooming|Black Ship Grooming]]
- [[lines/barrister-and-mann|Barrister and Mann]]
- [[lines/declaration-grooming|Declaration Grooming]]
- [[lines/barrister-and-mann-barristers-reserve-line-and-base-resolved-2026-10-21|Barrister and Mann — Barrister's Reserve®: line AND base, resolved 2026-10-21]]
- [[lines/barrister-and-mann-omnibus-transition-fall-2021|Barrister and Mann — Omnibus transition (fall 2021)]]
- [[lines/dr-jons-handcrafted-soap-co-formula-eras-and-lines-closed-2022|Dr. Jon's Handcrafted Soap Co. — formula eras & lines (closed 2022)]]
- [[lines/chatillon-lux-line-structure-2026-10-21|Chatillon Lux line structure (2026-10-21)]]
- [[lines/grooming-dept-base-system-2026-10-22|Grooming Dept base system (2026-10-22)]]
- [[lines/aion-skincare-era-products-post-rename-2024-see-lineages-md-catalog|Aion Skincare-era products (post-rename, 2024+, see lineages.md [catalog])]]
- [[lines/declaration-grooming-2|Declaration Grooming (lines)]]
- [[lines/dg-addendum-2026-11-07|DG addendum, 2026-11-07]]
- [[lines/dg-rename-era-loose-ends-resolved-2026-11-08-answers-backlog-items-b-d|DG rename-era loose ends RESOLVED 2026-11-08 (answers backlog items (b) + (d))]]
- [[lines/barrister-and-mann-base-eras-as-identity-established-2026-10-24|Barrister and Mann — base eras as identity (established 2026-10-24)]]
- [[lines/b-and-m-latha-addendum-established-2026-10-28-corrects-and-completes-the-entry|B&M Latha addendum (established 2026-10-28; corrects and completes the entry above)]]
- [[lines/b-and-m-soft-heart-release-list-established-2026-10-30-resolves-the-backlogs-b|B&M Soft Heart release list (established 2026-10-30; RESOLVES the backlog's "B&M Soft Heart release list"]]
- [[lines/long-rifle-black-label-line-formula-established-2026-10-23|Long Rifle "Black Label" line/formula (established 2026-10-23)]]
- [[lines/arko-men-after-shave-cream-50-ml|Arko Men After Shave Cream (50 ml)]]
- [[lines/asylum-shave-works|Asylum Shave Works]]
- [[lines/envy-shave|Envy Shave]]
- [[lines/original-formula|Original formula]]
- [[lines/formula-9-formula-10|Formula 9 / Formula 10]]
- [[lines/kokum-butter-vegan|Kokum-butter vegan]]
- [[lines/matilda-base|"Matilda" base]]
- [[lines/tradditional-vegan|"Tradditional Vegan"]]
- [[lines/sweet-almond-oil-vegan|Sweet-almond-oil vegan]]
- [[lines/mango-butter-vegan|Mango-butter vegan]]
- [[lines/betti-base|"Betti Base"]]
- [[lines/duck-fat-base|Duck-fat base]]
- [[lines/line-name|Line name]]
- [[lines/the-seven-soaps-maker-store-products-json-live-2026-11-07|The seven soaps (maker store, products.json live 2026-11-07)]]
- [[lines/one-shared-vegan-base|One shared vegan base]]
- [[lines/aftershave-toner-line-2026-expansion|Aftershave/toner line (2026 expansion)]]
- [[lines/maker|Maker (lines)]]
- [[lines/sunset|Sunset]]
- [[lines/quatre-cent-vingt|Quatre Cent Vingt]]
- [[lines/siberian-sunrise|Siberian Sunrise]]
- [[lines/muguet|Muguet]]
- [[lines/villains-rose-the-villains-rose|Villain's Rose / The Villain's Rose]]
- [[lines/eau-de-th|Eau de Thé]]
- [[lines/summer-solstice|Summer Solstice]]
- [[lines/caged|Caged]]
- [[lines/pommes-au-four|Pommes Au Four]]
- [[lines/greek-fire|Greek Fire]]
- [[lines/dark-roast|Dark Roast]]
- [[lines/guy-noir|"Guy Noir"]]
- [[lines/mal-asl-2023|"Mal ASL 2023"]]
- [[lines/forbidden-forest|"Forbidden Forest"]]
- [[lines/image-only-aftershave-tonic-scents|Image-only aftershave-tonic scents]]
- [[lines/irish-cream-as-a-cb-name-poster-paraphrase-only|"Irish Cream" as a CB name = poster paraphrase only (lines)]]
- [[lines/maggard-meetup-yearly-releases|Maggard Meetup yearly releases]]
