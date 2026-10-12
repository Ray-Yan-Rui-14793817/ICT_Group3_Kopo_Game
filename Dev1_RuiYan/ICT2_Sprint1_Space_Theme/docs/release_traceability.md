# Release Traceability - Rui Yan / Dev1

**Evidence checkpoint:** 12 October 2026 (Asia/Shanghai).

## Source Records

The supplied `Copy of CP5047 Assessment 1 Group 3 Project Plan.pdf` records Rui Yan's roles on page 1, Alpha-to-Beta Product Backlog on pages 3-4 and 15-16, seven-item Sprint Backlog in Table 2 on pages 18-19, and branch / pull request / synchronisation evidence on pages 22 and 24-27. The assessment rubric appears on pages 31-32.

The supplied `CP5047 Assessment 1 Individual Risk Analysis Reflection_Rui Yan.pdf` records the same Sprint Backlog in Table 1 on page 2, PR #5's workflow meaning on page 3, and Rui Yan's three risk judgements and mitigations on pages 4-5. These are planning and reflection sources. Repository artefacts and dated test records determine verified delivery status.

The source PDFs are not copied into the repository. Their recorded roles, scope, estimates and risk ratings are the basis for this Dev1 documentation.

## Product Backlog: Alpha to Beta and Final

| User story | Release position | Status | Repository evidence and remaining requirement |
| --- | --- | --- | --- |
| US1 - Animal Size Ordering | ICT1 Alpha baseline | Alpha Completed, recorded in Assessment 1 | [Level 1 assets](../../ICT1_Ordering_Game/animal_Themes_level1/) and the [Alpha README](../../ICT1_Ordering_Game/Readme.md) are preserved. No new execution or acceptance result is claimed. |
| US2 - Animal Quantity Ordering | ICT1 Alpha baseline | Alpha Completed, recorded in Assessment 1 | [Level 2 assets](../../ICT1_Ordering_Game/animal_Themes_level2/) are preserved. Historic status comes from the supplied plan. |
| US3 - Animal Number Ordering | ICT1 Alpha baseline | Alpha Completed, recorded in Assessment 1 | [Level 3 assets](../../ICT1_Ordering_Game/animal_Themes_level3/) and [shared Animal design assets](../../ICT1_Ordering_Game/animal_theme_design/) are preserved. |
| [US4 - Space Theme Ordering Game #8](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/8) | ICT2 Beta / Sprint 1 | Evidence Required | Sprint planning and workflow documentation exist. Space implementation, dated tests and acceptance review are missing. |
| US5 - Candy Theme Ordering Game | Later Beta | Planned | Listed in the source Product Backlog. No implementation or release acceptance is evidenced. Outside Sprint 1. |
| US6 - Chinese Festival Theme Ordering Game | Later Beta | Planned | Listed in the source Product Backlog. No implementation or release acceptance is evidenced. Outside Sprint 1. |

ICT2 continues into Final development, but no completed Final release or fixed Final schedule is established by this checkpoint. The Alpha learning progression supports a bounded Beta extension; it does not automatically verify the new theme.

## US4 Sprint Backlog Traceability

| Sprint item | Issue / owner | Acceptance criteria | Planned testing | Status / evidence gap |
| --- | --- | --- | --- | --- |
| Space Theme Details | #8 / Rui Yan | TH-01 to TH-03 | S1-01, S1-02, S1-12, S1-13, S1-16 | Todo. Space assets and the three-level journey are required. |
| 4.1 Space Size Ordering | [#2](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/2), parent #8 / Rui Yan | SZ-01 to SZ-05 | S1-03, S1-04, S1-09 to S1-11, S1-14, S1-18 | Evidence Required. The historical In Progress report lacks implementation and testing records. |
| 4.2 Space Quantity Ordering | [#3](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/3), parent #8 / Rui Yan | QTY-01 to QTY-04 | S1-05, S1-06, S1-09 to S1-12, S1-18 | Todo. Groups, logic and execution results are required. |
| 4.3 Space Number Ordering | [#4](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/4), parent #8 / Rui Yan | NUM-01 to NUM-04 | S1-07 to S1-12, S1-18 | Todo. Cards, logic and execution results are required. |
| Hints and Instructions | #8 / Rui Yan | HI-01 to HI-03 | S1-09, S1-10, S1-12, S1-14 | Todo. Implemented instructions and hints must be checked in every level. |
| Positive / Gentle Feedback | #8 / Rui Yan | FB-01 to FB-03 | S1-10, S1-11, S1-13, S1-14 | Todo. Correct, incorrect and repeated-retry outcomes require evidence. |
| Sprint 1 Testing | #8 / Rui Yan | TEST-01 to TEST-04; UX-01 to UX-04 across the levels | S1-01 to S1-18 | Todo. Test execution, defect reruns and acceptance review are required. |

The supporting theme, instructions, feedback and testing items remain explicit parent checklist items. Child issues #2-#4 retain the three core ordering activities. [Duplicate #9](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/9) is retained in history and closed as a duplicate of #8. Its closure is an administrative cleanup, not US4 completion.

## Inspection and Workflow Evidence

| Record | Verified evidence | Interpretation |
| --- | --- | --- |
| Fetched origin/main | `8c2c2a39bbd20c4a49ea0db0c2fe0d4aa37888b8` | Shared baseline used before this documentation work. |
| Existing Dev1 feature branch | `Dev1-RuiYan-Space-Theme-Ordering` at `4d6af61689d5a05dd314b7d065c9a5c00963063e`; zero ahead, three behind origin/main at inspection | Historical work remains intact. Repository synchronisation is necessary before continuing from that branch. |
| [Merged PR #5](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/5) | One commit, one changed file, six added README lines; merged on 29 September 2026. Merge commit `ee65db070f98348aad32704d68b10f01a870bde9`. | Evidence of the agreed GitHub workflow, review visibility and traceability. The discussion includes a Codex review summary; no Space functional testing or feature acceptance is established. |
| Prior Sprint README | Size Ordering: In Progress; Quantity and Number Ordering: Todo | Historical reported states. Size progress is now Evidence Required because the inspected branch and main contain documentation without a Space implementation. |
| Original Space folder | `Dev1_RuiYan/ICT2_Sprint1_Space_Theme/Readme.md` was its only tracked file | No Space assets, runnable export, source or test execution record was present at inspection. |
| Alpha preservation baseline | `ICT1_Ordering_Game` tree `2603204ae56b3fa490f87245dfa0e56c770bf724` | Existing Alpha files remain unchanged. New documentation does not replace or certify historic evidence. |
| Current documentation branch | `Dev1-RuiYan-Sprint1-Documentation`, created from fetched origin/main with zero ahead / behind | Dedicated Dev1 change scope with small commits and a new pull request for review. The new PR records documentation and issue alignment. |

## Evidence Chain and Review Gate

For each feature, keep the chain visible: **Assessment 1 scope -> Sprint Backlog -> issue -> implementation commit/export -> dated test result -> acceptance review -> pull request**. Use [criterion IDs](acceptance_criteria.md) and [test IDs](testing_plan.md) in the records. The [evidence guide](../evidence/README.md) defines required fields and intended destinations.

Do not use automatic issue-closing keywords for documentation-only changes. Keep #8 and #2-#4 open until implementation, testing and acceptance evidence support completion. PR #5 and the new documentation PR are workflow records; neither establishes full Space delivery.

## Assessment Alignment and Remaining Evidence

This record supports release-oriented planning through the preserved Alpha baseline, current US4 and deferred US5-US6. The bounded backlog supports scope and feasibility. Criterion-to-test mapping supports quality and testing. Named ownership, issue links and branch / PR records support professional communication and accountability.

Remaining evidence includes an accessible Space build or platform export, versioned assets and ordering logic, a confirmed test environment, dated actual results, defect and rerun records, peer acceptance and Dev1 Project board reconciliation. Final release readiness remains subject to those checks.
