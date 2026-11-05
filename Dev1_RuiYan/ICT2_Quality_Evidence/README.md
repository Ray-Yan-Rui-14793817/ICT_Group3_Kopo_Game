# Dev1 — ICT2 quality and completion evidence

**Current checkpoint:** 5 November 2026 (Asia/Shanghai). **Owner:** Rui Yan / Dev1. **Release:** ICT2 Beta / Assessment 2.

Rui Yan has explicitly confirmed that **US5 Candy and US6 Chinese Festival game design, implementation and game testing are completed**, including Size, Quantity and Number Ordering. Supporting detailed test-document links can be consolidated without changing completed game work back to Todo.

## Evidence index

- [Assessment 2 completion and testing record](testing/assessment2_completion.md): developer confirmation, report page references, actual gameplay images, Week 6 findings and precise documentation gaps.
- [Additional evidence validation](testing/assessment2_evidence_validation.json): report SHA-256, page/crop provenance, six additional PNG checks and the active Candy Pause byte comparison.
- [Original ZIP manifest](testing/asset_manifest.json) and [static validation](testing/asset_validation.json): historical source checkpoint for 78 PNGs and 2 JSON files, including 15 unchanged Space images. These records remain unchanged and retain the failed check for the unsuitable ZIP Pause image.

The source report is `CP5047 Assessment 2 Group Implementation and Demonstration Group3.pdf` (45 pages). Only Dev1 evidence is reproduced here; shared pages are cropped to exclude other developers' work. These images are rendered from existing report pages, not fabricated screenshots or new historical test executions.

## Current quality status

| Concern | Evidence and result | Current state |
| --- | --- | --- |
| US5/US6 game testing | Completed, explicitly confirmed by Dev1 Rui Yan; Section 1 shows all three levels for each theme | **Completed — developer confirmed; detailed supporting test links to be consolidated** |
| Candy Pause active version | `candy_pause_button.png` is 324 × 115, 15,106 bytes, transparent and contains three nonempty 108 × 115 cells. It is byte-identical to the image loaded by Candy (KOPO file ID 232120) | Active version identified; measured specification check Pass |
| Unsuitable ZIP Pause source | [Historical image](refinement/Candy%20Pause%20Button%20png.png): 1536 × 1024, 2,470,318 bytes | Historical source specification Fail retained; this is not the active game sprite |
| Candy Pause/Exit meaning | [Before](refinement/week6_pause_exit_before.png), [After and reported retest](refinement/week6_pause_exit_after_retest.png); Group Report Week 6 Activity 5 explicitly records Retest result: Pass | Refinement and reported retest completed; no fabricated execution date or fresh full-suite claim |
| Candy Restart styling | [Week 6 Test 2](refinement/week6_restart_followup.png) identifies style differences and records later improvement | **Deferred**; no new styling change claimed |
| Candy Resume size rule | Supplied and currently loaded sprite is 80,640 bytes: above 80,000 but below 81,920 | Formal upload-size requirement to confirm; game completion unchanged |
| Source tilemaps | Both preserved maps match the ICT1 blob and reference `background.png`; Chinese source package uses a differently named background | Standalone export usage/dependency follow-up; not evidence of an unfinished running game |
| Space Drop Box | Existing source bytes and original quality concern retained | Earlier variant selection / integration evidence can be consolidated separately |
| Required KOPO game-design review | Passed, confirmed by Dev1 Rui Yan for US4–US6 | Completed; no duplicate design review required |
| GitHub PR approval / integration | No formal PR approval required by the rules checked at merge; zero submitted reviews recorded | PR #22 merged; no GitHub approval invented |

## Tracking and scope

[US5 #23](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/23) and [US6 #24](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/24) describe completed game development/testing. [Follow-up #25](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/25) records the completed PR #22 merge and tracks evidence-document consolidation, source-package questions and deferred Restart styling. These remaining tasks are not requirements to redo the completed games.

The earlier asset-only checkpoint correctly stated that this repository update had not independently executed the three-level runtime test suite. The later developer confirmation and newly inspected report now establish the current completion record. Earlier commits and original static measurements are preserved. No other developer files, Issues, branches or PRs are modified.

## Main integration checkpoint

[PR #22](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/22) was merged using a merge commit on 5 November 2026. Merge SHA: [`15fe5b29b0c654d2b7e55bbebbfe4b388243e84f`](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/commit/15fe5b29b0c654d2b7e55bbebbfe4b388243e84f). Space Level 2–3, Candy (including the verified active Pause sprite), Chinese Festival and Assessment 2 evidence are present in main. Original Space assets, ICT1 Alpha and all other developer subtrees are unchanged. Design-review completion is the developer's confirmation; GitHub-specific approval requirements were checked separately and none blocked the merge.
