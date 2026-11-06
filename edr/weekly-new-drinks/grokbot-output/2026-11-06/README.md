# EDR catch-up kit — 2026-11-06 (final review)

**DRAFT ONLY.** Do not publish, schedule, or post from this folder.

**Saved for review in pull request #1** on branch `cursor/edr-weekly-catchup-review-7eaa`. This folder is the review copy for that pull request. It is not on `main`.

These are the final scene composites supplied for review. They keep the approved scene approach and replace the earlier can cutouts. `edr/weekly-new-drinks/latest/` and `archive/` are unchanged.

## Source

Catalog-add catch-up from commit `fd89ef3d8a364b87a4cb60a842b7e55b721688e9`.

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

`source/new-drinks.json` is the manifest at that commit (sha256 `53af5567dbbf1dbdd53fa3021ce7d0280d356df006ec5a3d94237d183e1f7d13`). It matches `latest/new-drinks.json` and `archive/2026-11-06/new-drinks.json`. The kit’s copy parses to the same document and differs only by JSON unicode escaping.

Public manifest: https://raw.githubusercontent.com/Tom62g/social-images/main/edr/weekly-new-drinks/latest/new-drinks.json

## Coverage: 20 of 58

Five themed graphics, four unique drinks each. The other thirty-eight stay in the manifest. Selection details are in `source/batches-plan.json`.

| Graphic | On-image headline | Drinks |
| --- | --- | --- |
| 01 Winter & dessert | Which winter flavor are you curious about? | Red Bull The Winter Edition, Pistachio & Berries; Celsius Spritz Vibe Sparkling Shirley Temple; Monster Energy Vanilla Shot; Sparkling Candy Apple (Gorgie) |
| 02 Fresh faces | Which new face would you try first? | Angry Angel Fuel Peach Ginger; Hawk Energy Ultra Lightning Lemonade; Be Love Lemonade Lift; Gym Soda Rainbow Sherbet |
| 03 Zero-sugar | Which zero-sugar pick are you eyeing? | LIFEAID FocusAid Zero Sugar Kiwi Strawberry; Monster Energy Zero Sugar Vanilla Shot; Red Bull The Winter Edition Sugarfree, Pistachio & Berries; Hiball Energy Watermelon Mint |
| 04 Citrus & lemonade | Which citrus flavor would you try? | Rip It Power Sharp Citrus; El Jefe Phantom Lemonade; Yesly Lime; Accelerator Cherry Limeade |
| 05 Tropical fruit | Which tropical can are you reaching for? | SpaceTime Orange Mango; LIFEAID FITAID Energy Tropical Breeze; Xrave Mood Energy Tropical Bliss; El Jefe Baja Orange |

## Files

- `drafts.md` — platform copy
- `social-drafts.json` — the same copy as metadata (`designVersion` `v4-scene-composite-manual-outline`)
- `source/new-drinks.json` — source manifest, unchanged
- `source/batches-plan.json` — the 20-drink selection with label facts
- `graphics/` — five Pinterest masters (1000×1500) and five dedicated squares (1000×1000)
- `graphics/contact-sheet-FINAL-2026-11-06.jpg` — review preview of all ten graphics (1932×1050)

The earlier v3 preview file is removed. Captions and alt text are unchanged from the previous review copy. Design notes now describe the hand-set outlines.

## Captions and links

Threads lengths are 345, 307, 325, 295, and 310. Drink names, brands, dates, label facts, and page URLs in the metadata and in `source/batches-plan.json` match the manifest.

Each platform link uses `https://energydrinkratings.com/new` with `utm_medium=social`, `utm_campaign=edr_catalog_additions_2026_11_06`, platform `utm_source`, and graphic `utm_content`.

Those links are not the per-drink `trackedUrl` values (`utm_source=grok`, `utm_campaign=edr_new_weekly_2026-11-06`, path `/drinks/<slug>`). Left as written.

## Can limits, from the source photos

Outlines use the original product-photo colors. These limits are in the source files and were not redrawn:

- **Gym Soda** (`latest/images/gym-soda-rainbow-sherbet.jpg`, 400×1000) is cropped through the cone and the volume line. The graphic bottom is a curved trim of that photo, not a silver base rim.
- **Hawk Energy** (`hawk-energy-ultra-lightning-lemonade.jpg`, 600×882) already cuts the top banner and the bottom volume line. The composite keeps those source pixels, so the top reads as a partial “LYTES • 5,000MG CREA…” line and the base line is clipped.
- **Be Love** no longer shows the earlier white remnant on the pin or the square.
- **LIFEAID FITAID Tropical Breeze** no longer shows the earlier missing section on the right edge.
- **SpaceTime** (`spacetime-orange-mango.jpg`, 280×680) includes an orange slice in front of the can’s lower right. That slice is in the source photo.
- **Rip It** (`rip-it-power-sharp-citrus.jpg`, 208×488) is the smallest source photo, so the enlarged can is softer than the others.
- **El Jefe** Phantom Lemonade and Baja Orange use the prior cutout tightened by 1 px, as stated in `social-drafts.json`. The visible edge is tight and the old table background is gone. A 1 px choke is not measurable by eye beyond that.

## Verification

| File | Pixels | sha256 |
| --- | --- | --- |
| `01-winter-dessert-pinterest-1000x1500.jpg` | 1000×1500 | `4575b470fcd39e758fa442b51c5853b9af89fae2e98ddf8b648a6570105afbc6` |
| `01-winter-dessert-square-1000.jpg` | 1000×1000 | `b1557916b10b063e3b8a1d1e37b544d8b678dea8fdc4b19282d04f775bfa5606` |
| `02-new-brands-pinterest-1000x1500.jpg` | 1000×1500 | `af476cf69ddacb01403e9c5103d3593219d3b1a0cf02bc19e524afaedc52c31c` |
| `02-new-brands-square-1000.jpg` | 1000×1000 | `a46cd13ad5d3253a969059a24460959cadc0f887f7d5300b90f1bd87709ab2d9` |
| `03-zero-sugar-pinterest-1000x1500.jpg` | 1000×1500 | `f3ad0e5598ec0edbc07adc8a3f1b201f7bb620e3d052524d0a1d22924e28389c` |
| `03-zero-sugar-square-1000.jpg` | 1000×1000 | `db1ac68cec964e06651be90f893ec256f4f051ffa3ad5bc1f7e7add19948d2dd` |
| `04-citrus-lemonade-pinterest-1000x1500.jpg` | 1000×1500 | `8920c9757570d64dd1ff52daba5a4c7a1b1a3af7cf6db555a044e8a38ee0acab` |
| `04-citrus-lemonade-square-1000.jpg` | 1000×1000 | `ae58514031526d38171800c136499b89916c933a21a9eb75f06e45ec17127d31` |
| `05-tropical-fruit-pinterest-1000x1500.jpg` | 1000×1500 | `bd884f33a4bfa250d350625165303738cdf85123e386a4b6552ab98e4284b847` |
| `05-tropical-fruit-square-1000.jpg` | 1000×1000 | `475971fb99312b2d104ac3d254f62e4950280dbe771ac45a0e3b2b00e6e12ad7` |
| `contact-sheet-FINAL-2026-11-06.jpg` | 1932×1050 | `b6b7a602ee57990e92aa5fbe3bfabdb60113d14b2ac0e5d6a5d79bff0e68270e` |

All five squares show the question headline and the footer. Graphic 03 drinks still have `sugarG` 0 and `sugarFree` true, including Hiball Energy Watermelon Mint. Graphic 02’s “new face” line still rests on the manifest `new brand` / first-listing text for Angry Angel, Hawk Energy, Love energy (drink name Be Love Lemonade Lift), and GYM Soda.

No credentials, private keys, email addresses, or phone numbers are in the kit text. No workflows or schedules were added.
