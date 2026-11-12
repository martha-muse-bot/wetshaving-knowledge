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
**Sunny Lane [catalog]:**

**Figarose [catalog]:**

**Method notes:** (1) Row-level base-tag counts are contaminated — "Reserve" 11/22 and "Omnibus" 20 for these scents were all other-products-in-the-row; only field-scoped counts (base word inside the same soap/aftershave string as the scent) are evidence. (2) A retailer's created_at + published_at pair dates the LISTING, and a same-day publication cluster across scents (Jan 5, 2026) is a retailer push, not a launch wave — the maker store's absence + zero in-hands tags keep the reissue-vs-migration question open. (3) A scent-profile rework note on maker copy ("rework the original fragrance profile") is a scent change, not a base change — record it as such even when the scent+base key stays.
**Special Sessions Series (2026) [catalog]:** a four-scent blues-tribute line, all four authored by outside perfumer **Cécile Hua** (see people.md) — a first for B&M, whose scents are normally Will Carius's own compositions. Maker copy (barristerandmann.com, live 2026-11-11) + dataset census (full corpus, field-scoped):

**Method notes:** (1) A meetup-exclusive launch can leave zero dataset trace for months — the Sessions census proves the general-release date, not the meetup date, is what dataset rows attest; a "first use" is a first-USE date, never a launch date, for channel-exclusive releases. (2) A $2.50 price premium over the house base price is LE pricing until an INCI says otherwise — price is not base evidence. (3) "Five musicians, four sets" is a counting trap resolved by reading the tribute list, not by hunting a missing fifth product.
**CORRECTION to the 03:06 Sessions entry [catalog] — the "Maggard meetup exclusive → sets sold to attendees" launch arc is WRONG and is superseded here.** Firsthand dataset evidence — _walden_, 2026-10-09, quoting Will Carius's reply email verbatim: at the April 2026 Maggard Meetup (Adrian, MI), B&M had **SIX new scents**; attendees smelled them **BLIND** (no names, no notes) and ranked them; the best would become released products. The September 2026 Sessions Series = the top four (Waits, Two Walters, King, Kanno); the other two scents were cut and remain unnamed/unknown. gcgallant 2026-10-09 corroborates (Waits was his top-ranked meetup evaluation; "my top ranking choice when I evaluated the fragrance at the Maggard Meetup"). **Nothing was sold at the meetup per either firsthand note — there is no meetup-only variant; the meetup scents ARE the Sessions scents, tested blind and unnamed.** The "exclusive" gloss came from an unboxing video's loose wording ("presented exclusively at the Maggard Razors meetup") — retire it; an unboxing video is not a launch record. The September general release (soaps + splashes published 2026-09-22; samples created 2026-10-16, published 2026-10-21) is the ONLY release; first SOTD strings (Oct 9, 2026) are the general release. The rest of the 03:06 entry stands: four-scent blues tribute, all authored by Cécile Hua; base still UNPINNED (never default to Omnibus); Kanno soap + all four aftershaves still owed. **NEW NARROW LEAD (c4-narrow-32):** the two cut scents' identities — unnamed at the meetup by design; only Will could name them. **Method note:** a "first use" is a first-USE date, never a launch date — and a meetup *tasting* leaves no dataset trace at all; the Sessions census proves the general-release date, not the meetup date.

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
- [[lines/b-and-m-cologne-russe|B&M Cologne Russe]]
- [[lines/b-and-m-feb-2024-trim|B&M Feb-2024 trim]]
- [[lines/b-and-m-behold-the-whatsis|B&M "Behold the Whatsis!"]]
- [[lines/b-and-m-hand-and-body-soap-line|B&M Hand & Body Soap line]]
- [[lines/b-and-m-samhain|B&M Samhain]]
- [[lines/b-and-m-full-measure-of-a-man|B&M "Full Measure of a Man"]]
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
- [[lines/launch-mar-2020-excelsior-base|Launch Mar 2020, Excelsior base]]
- [[lines/dataset-283-rows-59-authors|Dataset: 283 rows / 59 authors]]
- [[lines/omnibus-era|Omnibus era]]
- [[lines/no-sunny-lane-edt|No Sunny Lane EdT]]
- [[lines/catalog|Catalog (lines)]]
- [[lines/launch-aug-2021-soft-heart-base|Launch Aug 2021, Soft Heart base]]
- [[lines/dataset-203-rows-35-authors|Dataset: 203 rows / 35 authors]]
- [[lines/omnibus-era-at-retail|Omnibus era at retail]]
- [[lines/catalog-2|Catalog (lines 2)]]
- [[lines/launch-arc-maggard-meetup-exclusive-maker-site-general-release|Launch arc: Maggard meetup exclusive → maker-site general release]]
- [[lines/the-four-scents-maker-copy-verbatim-notes|The four scents (maker copy, verbatim notes)]]
- [[lines/five-great-musicians-four-sets|"Five great musicians" = four sets]]
- [[lines/pricing-availability-maker-store-live-2026-11-11|Pricing/availability (maker store, live 2026-11-11)]]
- [[lines/base-unpinned-catalog|BASE UNPINNED [catalog]]]
- [[lines/catalog-gaps-catalog|Catalog gaps [catalog]]]
