# Rui Yan — Dev1: KOPO Ordering Game

**Project:** CP5047 ICT2, Group 3

**Responsibility:** Ordering Game design and KOPO implementation; background, Drop Box, level images and UI controls.

**Current completion record:** 5 November 2026 (Asia/Shanghai). Dev1 Rui Yan explicitly confirms that **US5 Candy and US6 Chinese Festival game design, implementation and game testing are completed**. PR #22 is now merged into main. The required KOPO game-design review for US4–US6 has passed, as confirmed by Dev1 Rui Yan; no reviewer names or timestamps are inferred.

## Current release: ICT2 Beta / Assessment 2

| Story | Design | KOPO implementation | Game testing | Repository synchronisation | Review record |
| --- | --- | --- | --- | --- | --- |
| US4 — Space | Image Design: Completed | Three levels documented in Group Report Section 1, pp. 2–3; existing closed Issues retained | Refer to existing US4 records; no new full test run claimed here | All 25 Space PNGs in main: original 15 via PR #21, Level 2–3 via merged PR #22 | Design review passed — developer confirmed; no formal GitHub approval required |
| US5 — Candy | Game Design: Completed | Completed: Size, Quantity and Number Ordering | **Completed — confirmed by Dev1 Rui Yan; supporting detailed evidence links to be consolidated** | Assets, verified active Pause sprite and evidence in main via merged PR #22 | Design review passed — developer confirmed; no formal GitHub approval required |
| US6 — Chinese Festival | Game Design: Completed | Completed: Size, Quantity and Number Ordering | **Completed — confirmed by Dev1 Rui Yan; supporting detailed evidence links to be consolidated** | Theme sources and report screenshots in main via merged PR #22 | Design review passed — developer confirmed; no formal GitHub approval required |

The games are completed development work. Repository asset integration is also completed through [merged PR #22](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/22), merge commit [`15fe5b29b0c654d2b7e55bbebbfe4b388243e84f`](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/commit/15fe5b29b0c654d2b7e55bbebbfe4b388243e84f). Detailed test-document links and remaining packaging/quality follow-up are tracked separately in #25.

- [US5 Candy #23](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/23) and [US6 Chinese Festival #24](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/24) record completed game work.
- [Repository, evidence and review follow-up #25](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/25) records the completed merge and Restart styling repair, and tracks remaining evidence documentation and packaging questions.
- [Existing Project Board](https://github.com/users/Ray-Yan-Rui-14793817/projects/2) uses Todo / In Progress / Done. Its historic Sprint 1 title and shared field conventions are preserved. The current release is ICT2 Beta / Assessment 2; no unsupported sprint number or new shared milestone is invented.

## Three completed ordering levels and KOPO links

Every theme contains **Level 1 — Size Ordering**, **Level 2 — Quantity Ordering**, and **Level 3 — Number Ordering**.

| Story | KOPO game | Available implementation evidence |
| --- | --- | --- |
| US4 | [Space Ordering Game](https://www.kopo.com/g/game.php?gno=14378&lid=5377&thmno=5109) | Group Report pp. 2–3; [report p. 3](ICT2_Quality_Evidence/testing/report_section1_us4_us5.png) includes Space Level 3 |
| US5 | [Candy Ordering Game](https://www.kopo.com/g/game.php?gno=14378&lid=5381&thmno=5112) | [Report p. 3: all three Candy levels](ICT2_Quality_Evidence/testing/report_section1_us4_us5.png) |
| US6 | [Chinese Festival Ordering Game](https://www.kopo.com/g/game.php?gno=14378&lid=5391&thmno=5142) | [Report p. 4: all three Chinese Festival levels](ICT2_Quality_Evidence/testing/report_section1_us6.png) |

Both US5/US6 URLs match the hyperlinks embedded in the supplied Assessment 2 Group Report and open their named KOPO games. The current inspection confirmed Candy Level 1 rendering and identified its loaded Pause asset. This targeted check is separate from Rui Yan's previously completed three-level game testing.

## Asset index

| Theme | UI and design | Level 1: Size | Level 2: Quantity | Level 3: Number |
| --- | --- | --- | --- | --- |
| Space | [10 PNG](ICT2_Sprint1_Space_Theme/Space_Themes_design/) | [5 PNG](ICT2_Sprint1_Space_Theme/Space_Themes_level1/) | [5 PNG](ICT2_Sprint1_Space_Theme/Space_Themes_level2/) | [5 PNG](ICT2_Sprint1_Space_Theme/Space_Themes_level3/) |
| Candy | [9 usable design PNG + source JSON](ICT2_Candy_Theme/Candy_Themes_design/) | [5 PNG](ICT2_Candy_Theme/Candy_Themes_level1/) | [5 PNG](ICT2_Candy_Theme/Candy_Themes_level2/) | [5 PNG](ICT2_Candy_Theme/Candy_Themes_level3/) |
| Chinese Festival | [14 source PNG + source JSON](ICT2_Chinese_Festival_Theme/Chinese_Themes_design/) | [5 PNG](ICT2_Chinese_Festival_Theme/Chinese_Themes_level1/) | [5 PNG](ICT2_Chinese_Festival_Theme/Chinese_Themes_level2/) | [5 PNG](ICT2_Chinese_Festival_Theme/Chinese_Themes_level3/) |

The original ZIP's 78 PNGs and 2 JSON files were inspected; all 15 previously merged Space images match by Git blob SHA-1 and remain unchanged. See the [original ZIP manifest](ICT2_Quality_Evidence/testing/asset_manifest.json) and [original static checks](ICT2_Quality_Evidence/testing/asset_validation.json). The ZIP manifest and static checks remain historical snapshots. The current Restart sprite is a later developer-supplied replacement, documented separately; its previous bytes remain in Git history. Other source filenames and bytes are preserved, including `灯笼.png` and the two separately stored `orderingGameTilemap (2).json` files.

### Confirmed active Candy Pause sprite

The [current Pause PNG](ICT2_Candy_Theme/Candy_Themes_design/candy_pause_button.png) is **324 × 115, 15,106 bytes**, with three nonempty 108 × 115 cells and transparency. It matches the image loaded by the running Candy game byte for byte. The local source is `testing design/candy_pause_button.png`; observed KOPO asset file ID: `232120`. Its palette encoding is retained; compatibility is supported by its actual use in the running game.

The unsuitable 1536 × 1024 ZIP image remains in [historical refinement evidence](ICT2_Quality_Evidence/refinement/Candy%20Pause%20Button%20png.png). Its failed specification check remains a true finding about that source image; it is not the active Pause sprite.

## Testing, refinement and evidence

The [current Assessment 2 evidence record](ICT2_Quality_Evidence/testing/assessment2_completion.md) links Section 1 gameplay images, Week 6 Before/After evidence, the reported Pause/Exit retest Pass and documentation gaps. The [additional validation record](ICT2_Quality_Evidence/testing/assessment2_evidence_validation.json) identifies the source report, rendered page/crop provenance and active Pause hash comparison.

- US5/US6 testing is **Completed — developer confirmed**. Detailed dates, pass counts, per-case execution logs and independent acceptance are not invented where absent from the inspected evidence.
- Week 6 Activity 3 identifies duplicate Pause/Exit meaning; Activity 5 records a distinct Pause icon and **Retest result: Pass**. This is the report's recorded result, not a fresh full-suite execution by the repository update.
- **Candy Restart styling repair: Completed — confirmed by Dev1 Rui Yan.** The supplied final sprite replaces [candy_restart_button.png](ICT2_Candy_Theme/Candy_Themes_design/candy_restart_button.png): 324 × 115, 7,704 bytes, three nonempty 108 × 115 cells and transparency. [Revision validation](ICT2_Quality_Evidence/testing/candy_restart_refinement_validation.json) records the source-to-repository mapping and previous/current hashes. No new revision-specific KOPO retest is claimed by this upload. Candy Resume's formal size rule and standalone tilemap packaging remain in #25.
- The required KOPO game-design review has passed, as confirmed by Dev1 Rui Yan. At merge, main was unprotected, no active repository rulesets or required checks were present, and no formal GitHub PR approval was required. Zero submitted GitHub reviews were recorded; no approval is fabricated.

## Repository and Sprint history

- [Current asset and documentation PR #22](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/22): **Merged** using merge commit [`15fe5b29b0c654d2b7e55bbebbfe4b388243e84f`](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/commit/15fe5b29b0c654d2b7e55bbebbfe4b388243e84f); contains only `Dev1_RuiYan/**` changes.
- [Merged PR #21](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/21): 15 existing Space UI / Level 1 PNGs, preserved without duplicate upload.
- [Merged PR #5](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/5): earlier Sprint README update.
- [ICT1 Alpha assets and README](ICT1_Ordering_Game/) and [older Space Sprint 1 record](ICT2_Sprint1_Space_Theme/Readme.md) remain historical evidence.
- [Open documentation PR #20](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/20) reflects the earlier Sprint 1 checkpoint. Its earlier Planned statements about US5/US6 are historical and superseded by the current developer confirmation. That branch and its original commits are preserved.
- Existing US4 [parent #8](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/8) and [Size #2](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/2), [Quantity #3](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/3), [Number #4](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/4) remain closed with their history preserved. Duplicate #9 remains closed.
