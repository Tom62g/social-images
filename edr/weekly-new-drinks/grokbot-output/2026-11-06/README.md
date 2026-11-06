# EDR catch-up kit — 2026-11-06 (v3)

**DRAFT ONLY.** Do not publish, schedule, or post from this folder.

**Saved for review in pull request #1** on branch `cursor/edr-weekly-catchup-review-7eaa`. This folder is the review copy for that pull request. It is not on `main`, and it is not a local-only kit.

These files are the supplied v3 scene composites. They replace the earlier white-card graphics in this same folder. The source commit is still `fd89ef3d8a364b87a4cb60a842b7e55b721688e9`. `edr/weekly-new-drinks/latest/` and `archive/` are unchanged.

## What the source batch is

Catalog-add catch-up, separate from the Monday 10:00 launch posts.

| Field | Value |
| --- | --- |
| status | `new-drinks` |
| runDate | `2026-11-06` |
| count | 58 |
| weekLabel | Oct 23 to Nov 6 |
| windowStart | `2026-10-23` |
| dateBasis | day the drink was added to the catalog (catch-up run; publish day can be later) |
| datePublished on the 58 | `2026-10-23` through `2026-11-05` |
| liveDetectedOn | `2026-11-06` for all 58 |

The manifest note also says `datePublished` is the day the drink went live for visitors. Captions were left as written. They say the drinks were added to the catalog between Oct 23 and Nov 6, which matches `weekLabel` and `dateBasis`.

`source/new-drinks.json` is unchanged from the previous review commit. It matches `latest/new-drinks.json` and `archive/2026-11-06/new-drinks.json` at `fd89ef3` (sha256 `53af5567dbbf1dbdd53fa3021ce7d0280d356df006ec5a3d94237d183e1f7d13`).

Public manifest: https://raw.githubusercontent.com/Tom62g/social-images/main/edr/weekly-new-drinks/latest/new-drinks.json

## Coverage: 20 of 58

Five themed graphics, four unique drinks each. Twenty drinks are pictured. The other thirty-eight stay in the manifest only.

| Graphic | On-image headline | Drinks |
| --- | --- | --- |
| 01 Winter & dessert | Which winter flavor are you curious about? | Red Bull The Winter Edition, Pistachio & Berries; Celsius Spritz Vibe Sparkling Shirley Temple; Monster Energy Vanilla Shot; Sparkling Candy Apple (Gorgie) |
| 02 Fresh faces | Which new face would you try first? | Angry Angel Fuel Peach Ginger; Hawk Energy Ultra Lightning Lemonade; Be Love Lemonade Lift; Gym Soda Rainbow Sherbet |
| 03 Zero-sugar | Which zero-sugar pick are you eyeing? | LIFEAID FocusAid Zero Sugar Kiwi Strawberry; Monster Energy Zero Sugar Vanilla Shot; Red Bull The Winter Edition Sugarfree, Pistachio & Berries; Hiball Energy Watermelon Mint |
| 04 Citrus & lemonade | Which citrus flavor would you try? | Rip It Power Sharp Citrus; El Jefe Phantom Lemonade; Yesly Lime; Accelerator Cherry Limeade |
| 05 Tropical fruit | Which tropical can are you reaching for? | SpaceTime Orange Mango; LIFEAID FITAID Energy Tropical Breeze; Xrave Mood Energy Tropical Bliss; El Jefe Baja Orange |

## Design stored here

v3, as supplied: real cans in a cohesive scene, natural shadows, a short question headline, and no white product cards. Caffeine and sugar stay in the captions and metadata. Each square is its own layout. The headline, Energy Drink Ratings line, and footer are visible on all five squares and all five Pinterest masters.

## Files in this folder

- `drafts.md` — v3 platform copy, copied unchanged
- `social-drafts.json` — the same copy as structured metadata, copied unchanged
- `source/new-drinks.json` — source manifest at `fd89ef3`, preserved
- `graphics/` — ten canonical images (Pinterest 1000×1500 and square 1000×1000)
- `graphics/contact-sheet-5-pinterest-v3.jpg` — preview of the five Pinterest masters (1920×628)

Not committed: the kit zip, `source/archive-card-grid-v1-v2/`, background plates, can files, v3 cutouts, scripts, and other source working files. `drafts.md` and `social-drafts.json` still name `source/archive-card-grid-v1-v2/`. That path is the local archive of the old white-card graphics. Those old images are not in this pull request. None of the ten canonical files match those archived bytes.

## Captions and links

Captions, titles, alt text, and URLs in `drafts.md` and `social-drafts.json` are the v3 kit text. Threads lengths are 345, 307, 325, 295, and 310. Drink names, brands, dates, label facts, `whatsNew`, and page URLs in the metadata match the manifest. No caption was rewritten.

Each platform link uses:

- `https://energydrinkratings.com/new`
- `utm_medium=social`
- `utm_campaign=edr_catalog_additions_2026_11_06`
- `utm_source` = `facebook`, `threads`, or `pinterest`
- `utm_content` = the graphic id (`01-winter-dessert` through `05-tropical-fruit`)

Alt text describes the v3 scenes and the question headlines, not the old white-card grids.

Those links are internally consistent. They are not the per-drink `trackedUrl` values in the manifest (`utm_source=grok`, `utm_campaign=edr_new_weekly_2026-11-06`, `utm_content` = slug, path `/drinks/<slug>`). Left as written for review.

`drafts.md` names the existing Pinterest board owner handle. That is not a credential. It was left in the copied draft.

## Review notes

**Fresh faces / new listings.** Graphic 02 asks “Which new face would you try first?” The four drinks are marked in the manifest:

- Angry Angel Fuel Peach Ginger — tag `new brand`; whatsNew: “New brand on the site: Angry Angel (5 flavors added in this update).”
- Hawk Energy Ultra Lightning Lemonade — tag `new brand`; whatsNew: “New brand on the site: Hawk Energy (2 flavors added in this update).”
- Be Love Lemonade Lift — tag `new brand`; whatsNew: “New brand on the site: Love energy (7 flavors added in this update).” The catalog brand string is `Love energy`. The drink name is Be Love Lemonade Lift.
- Gym Soda Rainbow Sherbet — tag `new brand`; whatsNew: “First GYM Soda drink on the site.”

This repository’s weekly folder has no earlier run to recount brand history independently. The newness wording rests on those manifest fields. Graphic 02 is four of those entries. The same manifest also marks Hi ball energy, X mood drinks, Space Time Energy, Positive Energy, and Ciclon Energy Drinks as new or first listings.

**Zero sugar.** All four drinks on graphic 03 have `sugarG` 0 and `sugarFree` true, including Hiball Energy Watermelon Mint.

**Cutout leftovers, stored as supplied.** On graphic 02, the Be Love Lemonade Lift can has a white jagged remnant along its lower-left edge, on both the Pinterest master and the square. On graphic 05, the LIFEAID FITAID Energy Tropical Breeze can has a missing section on its right edge, on both sizes. These were not redrawn.

## Verification

All ten canonical graphics are JPEG. Pinterest masters are 1000×1500. Squares are 1000×1000. None match the previous white-card files.

| File | sha256 |
| --- | --- |
| `01-winter-dessert-pinterest-1000x1500.jpg` | `9544c0dc2c29cdd8668e78a07b1fa427fef5a5871bc2abe7049a9ce83735ce0a` |
| `01-winter-dessert-square-1000.jpg` | `51d92c0d1b4970f8eddf2ec1fdf174413b3a01fcdec059328069d03dce3a0af4` |
| `02-new-brands-pinterest-1000x1500.jpg` | `9da6e185a43c5c07a1fc13b3dc8f266de40a23f95c12d953a028109b5cdc4534` |
| `02-new-brands-square-1000.jpg` | `148e79d8ffdeaa179e8452afa436fa0df5b74f0247f078d72bf25aaaec8032e6` |
| `03-zero-sugar-pinterest-1000x1500.jpg` | `878228287cd6e79252362efc640a3bbf5dead5c58553f6905b3a303f9909f217` |
| `03-zero-sugar-square-1000.jpg` | `f3a4e6d31d17d42490927f11342b103c4a5a3aa8d3be8badf88d664f889607df` |
| `04-citrus-lemonade-pinterest-1000x1500.jpg` | `c7889d48b92e3879a6306b562fbb8c7995aa22f736015641ae0f45758108d6f5` |
| `04-citrus-lemonade-square-1000.jpg` | `9111d3ccb4dd61b415c89f3920a315bd556bb3c117bed075836f92ee627b21a7` |
| `05-tropical-fruit-pinterest-1000x1500.jpg` | `a46bdd68ef2c3ddb681598933887e524e164ef2099268a7eb4f53a6f02bdcb74` |
| `05-tropical-fruit-square-1000.jpg` | `3d7cd3731e08880b86b2107d490a473a4763c3cf87825b55daacb8182e6b87b2` |
| `contact-sheet-5-pinterest-v3.jpg` | `e8aa3e73263331afc31ff521fc4a64563b4325951150a809b7528c95d5d9fd7a` |

Text files were scanned for credentials, private keys, email addresses, and phone numbers. None were found.

No workflows, schedules, or executable code were added.
