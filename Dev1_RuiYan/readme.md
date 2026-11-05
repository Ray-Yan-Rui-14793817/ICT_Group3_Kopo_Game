# Rui Yan — Dev1: KOPO Ordering Game

**Project:** CP5047 ICT2, Group 3
**Contribution:** Ordering Game image, background, Drop Box, level assets and UI button design
**Asset checkpoint:** 5 November 2026 (Asia/Shanghai)

## ICT2 theme designs: US4–US6

The supplied Dev1 update plan reports image-design work completed for all three themes. Each theme has three sets of five level images: **Level 1 — Size**, **Level 2 — Quantity**, and **Level 3 — Number**. The repository preserves the supplied source images; deployment in KOPO and functional acceptance require separate evidence.

| Story / theme | Image-design record | Assets on this branch | KOPO runtime testing | Peer acceptance |
| --- | --- | --- | --- | --- |
| US4 — Space | Completed, as reported in the supplied plan | 25 PNG: 15 already in main via PR #21; 10 Level 2–3 images added | Not performed during this update | No new review recorded |
| US5 — Candy | Completed, as reported; final Pause export remains unresolved | 23 theme PNG + 1 source JSON; original Pause PNG isolated as evidence | Not performed during this update | No new review recorded |
| US6 — Chinese Festival | Completed, as reported; active variants need owner confirmation | 29 PNG + 1 source JSON | Not performed during this update | No new review recorded |

Files added on this branch are **pending merge into main**. Image design, repository synchronisation, static asset checks, runtime tests and peer acceptance are separate statuses.

## KOPO game links

These URLs are reproduced from the supplied update plan, which attributes them to the Group Report. They have not been functionally tested during this repository update. Use the in-game navigation to identify each level; no additional level URLs have been inferred.

| Story | Theme | Game |
| --- | --- | --- |
| US4 | Space | [Open Space Ordering Game](https://www.kopo.com/g/game.php?gno=14378&lid=5377&thmno=5109) |
| US5 | Candy | [Open Candy Ordering Game](https://www.kopo.com/g/game.php?gno=14378&lid=5381&thmno=5112) |
| US6 | Chinese Festival | [Open Chinese Festival Ordering Game](https://www.kopo.com/g/game.php?gno=14378&lid=5391&thmno=5142) |

## Asset index

| Theme | UI and design | Level 1: Size | Level 2: Quantity | Level 3: Number |
| --- | --- | --- | --- | --- |
| Space | [10 PNG](ICT2_Sprint1_Space_Theme/Space_Themes_design/) | [5 PNG](ICT2_Sprint1_Space_Theme/Space_Themes_level1/) | [5 PNG](ICT2_Sprint1_Space_Theme/Space_Themes_level2/) | [5 PNG](ICT2_Sprint1_Space_Theme/Space_Themes_level3/) |
| Candy | [8 PNG + source JSON](ICT2_Candy_Theme/Candy_Themes_design/) | [5 PNG](ICT2_Candy_Theme/Candy_Themes_level1/) | [5 PNG](ICT2_Candy_Theme/Candy_Themes_level2/) | [5 PNG](ICT2_Candy_Theme/Candy_Themes_level3/) |
| Chinese Festival | [14 PNG + source JSON](ICT2_Chinese_Festival_Theme/Chinese_Themes_design/) | [5 PNG](ICT2_Chinese_Festival_Theme/Chinese_Themes_level1/) | [5 PNG](ICT2_Chinese_Festival_Theme/Chinese_Themes_level2/) | [5 PNG](ICT2_Chinese_Festival_Theme/Chinese_Themes_level3/) |

The Candy Pause source image is in [refinement evidence](ICT2_Quality_Evidence/refinement/), outside the Candy integration directory. Its dimensions do not meet the stated button specification. No replacement has been invented or represented as the version used in KOPO.

Original filenames, image bytes and JSON bytes are preserved. Source directories are mapped into Dev1 theme directories; the exact source-to-repository mapping and Git blob hashes are in the [asset manifest](ICT2_Quality_Evidence/testing/asset_manifest.json). The Chinese filename `灯笼.png` is retained. Folder mapping:

- `Space Theme Design/*` → `ICT2_Sprint1_Space_Theme/*`.
- `Candy Theme Design/Candy theme design/` → `ICT2_Candy_Theme/Candy_Themes_design/`; the three Candy level directory names are retained.
- `Chinese Image Design/Design/` → `ICT2_Chinese_Festival_Theme/Chinese_Themes_design/`; `Level1`, `Level2` and `level3` → the corresponding `Chinese_Themes_level1`, `Chinese_Themes_level2` and `Chinese_Themes_level3` directories.

## Asset checks and unresolved quality concerns

The [static validation record](ICT2_Quality_Evidence/testing/asset_validation.json) records successful decoding of all 78 source PNGs, parsing of both JSON files and identical Git blob hashes for all 15 existing Space images. These checks do not establish correct gameplay or final integration.

- **Candy Pause / Exit:** the supplied Pause image is 1536 × 1024 and 2,470,318 bytes. It fails the plan's 324 × 115, three 108 × 115 frame cells and ≤80,000-byte target. The plan reports an earlier Pause/Exit icon refinement, but no verified final sprite or actual runtime retest accompanies this ZIP. Final export and semantic review remain pending.
- **Candy Resume:** 324 × 115, RGBA, 80,640 bytes; above 80,000 bytes but below 80 KiB (81,920 bytes). Confirm the actual platform limit before integration. The source has not been recompressed.
- **Candy Restart:** the supplied sprite is preserved. Styling consistency is a reported deferred concern; no new refinement or retest is claimed.
- **Space Drop Box:** the existing image is unchanged. The plan reports earlier visual alternatives, but selection and KOPO placement verification are not established by these files.
- **Chinese Festival variants:** both Drop Box images and the generically named design image are retained as supplied; their active use needs owner confirmation. Palette PNGs decode and retain transparency; KOPO compatibility remains untested.
- **Tilemaps:** both `orderingGameTilemap (2).json` files are identical to the existing ICT1 tilemap blob. They are preserved separately beside each theme's design sources. Both refer to `background.png`; Candy has that filename, while Chinese Festival has `chinese_cultural_background_800x432.png`. The Chinese relative reference is unresolved. Neither JSON is represented as a verified current KOPO export.

See the [quality and evidence record](ICT2_Quality_Evidence/README.md) for observed results and next steps. No child UAT, runtime Pass or teammate review has been created by this upload.

## Repository history and tracking

- [ICT1 Alpha assets and original README](ICT1_Ordering_Game/) are retained unchanged.
- [ICT2 Sprint 1 Space record](ICT2_Sprint1_Space_Theme/Readme.md) retains the earlier progress snapshot and adds the current asset checkpoint.
- [Merged PR #5](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/5) records the earlier Sprint README update.
- [Merged PR #21](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/21) added the 15 existing Space images. They are not uploaded again.
- [Open PR #20](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/20) contains historical Sprint 1 documentation. Reconcile its earlier status statements before a future merge; it is not merged or altered by this asset branch.
- Existing US4 records: [parent #8](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/8), [Size #2](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/2), [Quantity #3](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/3), [Number #4](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/4). All were already closed when inspected on 5 November 2026. Their existing states are preserved; this update adds no functional acceptance evidence. Duplicate [#9](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/9) remains closed.

This branch changes only `Dev1_RuiYan/**`. Review the asset PR's commit list for the Space, Candy, Chinese Festival and documentation changes.

Current asset update: [draft PR #22](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/22) records the new files, validation and unresolved integration concerns. New theme tracking is assigned to Rui Yan: [US5 Candy #23](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/23) and [US6 Chinese Festival #24](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/24).
