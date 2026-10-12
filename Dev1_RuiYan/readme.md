# Rui Yan / Dev1 - Ordering Game

## Role and project continuity

Rui Yan is the Product Manager, Product Marketing Manager and Ordering Game developer. Responsibilities include maintaining the Product Backlog, Sprint priorities and release plan; coordinating Sprint Planning and reviews; developing and testing the Ordering Game; and communicating progress and product value. Shared deliverables require evidence checks before submission.

CP5047 / ICT2 continues the CP5046 / ICT1 project for kindergarten students aged 4-6. The Animal Ordering Game provides the Alpha baseline. ICT2 extends this learning progression into Beta and Final development.

## Product Backlog and release boundary

| User story | Release | Status and evidence |
| --- | --- | --- |
| US1 - Animal Size Ordering | ICT1 Alpha | Alpha Completed, as recorded in Assessment 1. Existing Level 1 assets are preserved. |
| US2 - Animal Quantity Ordering | ICT1 Alpha | Alpha Completed, as recorded in Assessment 1. Existing Level 2 assets are preserved. |
| US3 - Animal Number Ordering | ICT1 Alpha | Alpha Completed, as recorded in Assessment 1. Existing Level 3 assets are preserved. |
| [US4 - Space Theme Ordering Game](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/8) | ICT2 Beta / Sprint 1 | Evidence Required. Planning and workflow records exist; Space implementation and testing evidence are missing. |
| US5 - Candy Theme Ordering Game | Later Beta | Planned. Outside the current Sprint Backlog. |
| US6 - Chinese Festival Theme Ordering Game | Later Beta | Planned. Outside the current Sprint Backlog. |

The historic Alpha status is retained from the supplied project plan. The repository holds its README, images and tilemap. This documentation update does not report a new Alpha test run or certify a complete runnable Alpha build. See [release traceability](ICT2_Sprint1_Space_Theme/docs/release_traceability.md).

## Sprint 1 scope and current status

| Sprint item | GitHub reference | Current status |
| --- | --- | --- |
| Space Theme Details | [US4 #8](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/8) | Todo |
| 4.1 Space Size Ordering | [Child #2](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/2) | Evidence Required |
| 4.2 Space Quantity Ordering | [Child #3](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/3) | Todo |
| 4.3 Space Number Ordering | [Child #4](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/4) | Todo |
| Hints and Instructions | [US4 #8](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/8) | Todo |
| Positive / Gentle Feedback | [US4 #8](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/8) | Todo |
| Sprint 1 Testing | [US4 #8](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/8) | Todo |

[PR #5](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/5) recorded Size Ordering as In Progress and Quantity and Number Ordering as Todo. Its single changed file was the Sprint README. It supports the agreed GitHub workflow, review visibility and traceability. It does not establish implementation, passed tests or US4 completion. The [Sprint 1 working document](ICT2_Sprint1_Space_Theme/Readme.md) explains the evidence behind each current status.

## Repository structure

```text
Dev1_RuiYan/
|-- readme.md
|-- ICT1_Ordering_Game/              Existing Alpha evidence
|   |-- Readme.md
|   |-- animal_Themes_level1/
|   |-- animal_Themes_level2/
|   |-- animal_Themes_level3/
|   `-- animal_theme_design/
`-- ICT2_Sprint1_Space_Theme/
    |-- Readme.md                   Sprint goal, scope and status
    |-- docs/
    |   |-- sprint1_backlog.md
    |   |-- acceptance_criteria.md
    |   |-- testing_plan.md
    |   |-- risk_and_mitigation.md
    |   `-- release_traceability.md
    `-- evidence/README.md          Evidence submission guide
```

The Sprint 1 folder currently contains documentation. Implementation exports and test records must be added when available. Evidence categories described in the guide are intended destinations, not existing test results.

## Status and completion rules

| Status | Meaning |
| --- | --- |
| Planned | A Product Backlog candidate or planned test; delivery has not been demonstrated. |
| Todo | Selected Sprint work with no supported implementation start. |
| In Progress | Active work supported by a linked implementation commit, export or other repository artefact. |
| Evidence Required | A progress or completion claim needs implementation, testing or acceptance evidence before it can be verified. |
| Complete | Implementation evidence, testing evidence and all relevant acceptance checks support completion and are visible in the repository. |

Tested means that a dated test record identifies the build, test cases, actual results and evidence. It is not implied by Complete-looking documentation or a merged pull request. No Sprint 1 feature is currently Complete or verified as tested.

## GitHub workflow and accountability

Fetch and pull the latest `main` before new work. Use a Rui Yan feature branch, small meaningful commits and regular pushes. Open a pull request into `main` and link the affected issues, acceptance criteria and testing evidence. Review the diff before integration. Use merges for repository synchronisation when a published feature branch falls behind; preserve history.

Keep changes within `Dev1_RuiYan/**`. Keep Rui Yan issue status and Sprint Backlog records consistent with repository evidence. Communicate important merges and blockers through the team's agreed channels. Recheck the current `main` after important merges. A documentation pull request must not automatically close implementation issues.

Before a feature is Complete, provide its implementation path and commit, dated test results, an acceptance check for every criterion and a visible repository update. Peer review must identify the build reviewed. [US4 #8](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/8) is the authoritative parent; duplicate #9 is retained in issue history for traceability.

## Assessment 1 alignment

The [Sprint Backlog](ICT2_Sprint1_Space_Theme/docs/sprint1_backlog.md) records the bounded seven-item scope and agreed estimates. [Acceptance criteria](ICT2_Sprint1_Space_Theme/docs/acceptance_criteria.md) and the [testing plan](ICT2_Sprint1_Space_Theme/docs/testing_plan.md) make quality checks visible. The [risk record](ICT2_Sprint1_Space_Theme/docs/risk_and_mitigation.md) preserves Rui Yan's stated risk judgements and distinguishes current controls from actions still required.

These records support release-oriented planning, scope and feasibility, quality and testing, and professional communication and accountability. They organise Rui Yan's evidence; they do not certify implementation or assessment submission readiness. Source documents and page references are recorded in release traceability.
