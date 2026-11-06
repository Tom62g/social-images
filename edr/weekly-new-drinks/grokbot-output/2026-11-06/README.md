# EDR catch-up kit — 2026-11-06

**DRAFT ONLY.** Manual review copy. Do not publish, schedule, or post from this folder.

**Interim old design.** These ten graphics are the existing reviewed kit, stored for review before a visual redesign. Thomas asked for a redesign of all five posters: no large white cards, cohesive scenes, real cans, natural shadows, strong question headlines, and fewer words. The replacement images will be added to this same branch and pull request when the updated kit is supplied. This commit does not redraw the posters.

`edr/weekly-new-drinks/latest/` and `edr/weekly-new-drinks/archive/` are unchanged.

## What the source batch is

Catalog-add catch-up from commit `fd89ef3d8a364b87a4cb60a842b7e55b721688e9` (`edr/weekly-new-drinks/latest/new-drinks.json`). It is the Sunday catalog-add batch, separate from the Monday 10:00 launch posts.

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

The manifest note also says `datePublished` is the day the drink went live for visitors, and that the site keeps no separate publish timestamp. Captions were left as written. They say the drinks were added to the catalog between Oct 23 and Nov 6, which matches `weekLabel` and `dateBasis`.

Snapshot copied here: `source/new-drinks.json` (same bytes as `latest/new-drinks.json` and `archive/2026-11-06/new-drinks.json` at this commit, sha256 `53af5567dbbf1dbdd53fa3021ce7d0280d356df006ec5a3d94237d183e1f7d13`). The kit’s own `source/new-drinks.json` parses to the same document; it only differs by JSON unicode escaping and a trailing newline.

Public manifest: https://raw.githubusercontent.com/Tom62g/social-images/main/edr/weekly-new-drinks/latest/new-drinks.json

## Coverage: 20 of 58

Five themed graphics, four unique drinks each. Twenty drinks are pictured. The other thirty-eight stay in the manifest only. This is a themed selection, not an equal split of the 58.

| Graphic | Drinks |
| --- | --- |
| 01 Winter & dessert | Red Bull The Winter Edition, Pistachio & Berries; Celsius Spritz Vibe Sparkling Shirley Temple; Monster Energy Vanilla Shot; Sparkling Candy Apple (Gorgie) |
| 02 New brands | Angry Angel Fuel Peach Ginger; Hawk Energy Ultra Lightning Lemonade; Be Love Lemonade Lift; Gym Soda Rainbow Sherbet |
| 03 Zero-sugar | LIFEAID FocusAid Zero Sugar Kiwi Strawberry; Monster Energy Zero Sugar Vanilla Shot; Red Bull The Winter Edition Sugarfree, Pistachio & Berries; Hiball Energy Watermelon Mint |
| 04 Citrus & lemonade | Rip It Power Sharp Citrus; El Jefe Phantom Lemonade; Yesly Lime; Accelerator Cherry Limeade |
| 05 Tropical fruit | SpaceTime Orange Mango; LIFEAID FITAID Energy Tropical Breeze; Xrave Mood Energy Tropical Bliss; El Jefe Baja Orange |

## Files in this folder

- `drafts.md` — platform copy, copied unchanged from the kit
- `social-drafts.json` — the same copy as structured metadata, copied unchanged
- `source/new-drinks.json` — source manifest at the commit above
- `graphics/` — ten canonical images (Pinterest 1000×1500 and square 1000×1000 for each theme)

Not committed: the zip, `*-v2.jpg` twins, background plates, can cutouts, the Claude catch-up poster, and `batches-plan.json`. The twenty can files in the kit match `latest/images/` byte for byte. The kit poster matches `latest/poster.png` and `archive/2026-11-06/poster.png` (1080×1350).

## Citrus files

The corrected citrus assets are the v2 files (pale frosted header and footer, dark type, and a square layout that keeps the header and footer). In the kit, each canonical citrus filename is byte-identical to its `-v2` twin. This folder keeps one file per size under the canonical name and leaves the duplicate `-v2` names out.

| Canonical file | sha256 | Size |
| --- | --- | --- |
| `graphics/04-citrus-lemonade-pinterest-1000x1500.jpg` | `36079ac2d86e8874959b7ff3587f4e9b4f254b07d2bc2b759633139b19ab6cb4` | 1000×1500 |
| `graphics/04-citrus-lemonade-square-1000.jpg` | `b3b8ff18f2d54f569000ec734266476ec2ac5c69fd15dd6e8cc0efb7b1f273b2` | 1000×1000 |

`drafts.md` and `social-drafts.json` still mention the `*-v2.jpg` attachment names. Those names are the same bytes as the canonical files above. The other four themes were copied unchanged.

## Captions and links

Captions, titles, alt text, and URLs in `drafts.md` and `social-drafts.json` are the kit text, including Threads lengths 351, 315, 330, 304, and 310. No caption was rewritten.

Each platform link uses:

- `https://energydrinkratings.com/new`
- `utm_medium=social`
- `utm_campaign=edr_catalog_additions_2026_11_06`
- `utm_source` = `facebook`, `threads`, or `pinterest`
- `utm_content` = the graphic id (`01-winter-dessert` through `05-tropical-fruit`)

Those links are internally consistent. They are not the per-drink `trackedUrl` values in the manifest (`utm_source=grok`, `utm_campaign=edr_new_weekly_2026-11-06`, `utm_content` = slug, path `/drinks/<slug>`). The folder readme allows changing `utm_source` and says to leave the other tags as they are. Campaign and path differ here. Left as written for review.

`drafts.md` and `social-drafts.json` still say the kit was local only and not written to GitHub. That described the kit before this review copy. This folder is still draft only.

`drafts.md` names the existing Pinterest board owner handle. That is not a credential. It was left in the copied draft.

## Review notes

**New brands.** The four drinks on graphic 02 are marked in the manifest, so the claim is not an extra invention:

- Angry Angel Fuel Peach Ginger — tag `new brand`; whatsNew: “New brand on the site: Angry Angel (5 flavors added in this update).”
- Hawk Energy Ultra Lightning Lemonade — tag `new brand`; whatsNew: “New brand on the site: Hawk Energy (2 flavors added in this update).”
- Be Love Lemonade Lift — tag `new brand`; whatsNew: “New brand on the site: Love energy (7 flavors added in this update).” The catalog brand string is `Love energy`. The drink name is Be Love Lemonade Lift. The caption uses the drink name.
- Gym Soda Rainbow Sherbet — tag `new brand`; whatsNew: “First GYM Soda drink on the site.”

This repository’s weekly folder has no earlier run to recount brand history independently. The “new brand” wording rests on those manifest fields. Graphic 02 is four of the new-brand entries, not every one. The same manifest also marks Hi ball energy, X mood drinks, Space Time Energy, Positive Energy, and Ciclon Energy Drinks as new or first listings. Some of those drinks appear on other graphics without a “new brands” headline.

**Zero sugar.** All four drinks on graphic 03 have `sugarG` 0 and `sugarFree` true, including Hiball Energy Watermelon Mint.

**Square crops.** On themes 01, 02, 03, and 05, the square file is a tight crop: the theme title and the footer line are cut off. The citrus square keeps a pale header and footer. Those files were stored as they are. The requested redesign is waiting on the updated kit.

**On-graphic facts checked against the manifest.** Citrus: Rip It 160 mg / 48 g sugar; El Jefe Phantom Lemonade 150 mg / 0 g; Yesly Lime 114 mg / 0 g; Accelerator Cherry Limeade 200 mg / 0 g. Winter: Red Bull 80 mg / 26 g; Celsius 200 mg / 0 g; Monster Vanilla Shot 160 mg / 53 g; Sparkling Candy Apple 150 mg / 0 g. New brands: Angry Angel 120 mg / 0 g; Hawk 300 mg / 1 g; Be Love 80 mg / 0 g; Gym Soda 114 mg / 3 g. Tropical: SpaceTime 50 mg / 2 g; FITAID Tropical Breeze 150 mg / 0 g; Xrave Tropical Bliss 225 mg / 0 g; El Jefe Baja Orange 150 mg / 0 g.

## Verification

All ten graphics are JPEG. Pinterest masters are 1000×1500. Squares are 1000×1000.

| File | sha256 |
| --- | --- |
| `01-winter-dessert-pinterest-1000x1500.jpg` | `854df140b92a60200c320267acf97739595eaa2e5422357adc0848900d37869f` |
| `01-winter-dessert-square-1000.jpg` | `7b8a6e756d9f6d509de3efdd5eb13be4bd39250cb428f4a6d0340faeb4f8a3c2` |
| `02-new-brands-pinterest-1000x1500.jpg` | `e9e8db0a52225cdc7975c71cc4e6a2b810be10729984bdb164fe49e127f59d93` |
| `02-new-brands-square-1000.jpg` | `eaf184c7a29ad65c5069e04f74dec3216b89e1aa3d3a567d90c4c1df64198d47` |
| `03-zero-sugar-pinterest-1000x1500.jpg` | `724e6c40b07c3d124591a058743fa40b70cbaef40e74b82344e866b854318120` |
| `03-zero-sugar-square-1000.jpg` | `0d3f8373791f2e7e6d5c0dd94a477359d2de9344ad2a4b3c8c95786c1b7d9060` |
| `04-citrus-lemonade-pinterest-1000x1500.jpg` | `36079ac2d86e8874959b7ff3587f4e9b4f254b07d2bc2b759633139b19ab6cb4` |
| `04-citrus-lemonade-square-1000.jpg` | `b3b8ff18f2d54f569000ec734266476ec2ac5c69fd15dd6e8cc0efb7b1f273b2` |
| `05-tropical-fruit-pinterest-1000x1500.jpg` | `ddae1722a7a901b4347c51525c455042b44cf35301d18cd19444f42198319880` |
| `05-tropical-fruit-square-1000.jpg` | `f4cf2e0151fd16e76f57077db80ac3f2647d5a6e98ee55bbe483ee82cad67062` |

Public URL checks returned HTTP 200: `https://energydrinkratings.com/new` (including the Facebook UTM form), each of the 20 featured drink pages, each featured can on raw GitHub under `latest/images/`, the raw manifest, and `latest/poster.png`. Text files in the kit were scanned for credentials, private keys, email addresses, and phone numbers. None were found.

No workflows, schedules, or executable code were added.
