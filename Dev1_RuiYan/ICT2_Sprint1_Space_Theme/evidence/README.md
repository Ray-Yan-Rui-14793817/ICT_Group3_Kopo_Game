# Sprint 1 Evidence Guide - Rui Yan / Dev1

**Scope:** US4 parent #8; Size #2, Quantity #3 and Number #4; theme details, instructions, feedback and Sprint 1 Testing.

This folder currently provides the evidence structure and submission rules. It contains no Space implementation export, game screenshot, test execution record or passed acceptance result. The documentation does not prove delivery.

## Intended Evidence Categories

Create the category folders when real evidence is available. The paths below are intended destinations; they are not claims that records already exist.

| Category | Intended path under this folder | Evidence to provide |
| --- | --- | --- |
| Implementation | `implementation/` | Asset or source manifest, platform export/build reference, version or commit, access steps and a mapping to issues and criteria. Keep actual implementation within Dev1. |
| Testing | `testing/` | Dated test records with build identity, environment, inputs, expected and actual results, Pass/Fail/Blocked and supporting observations or screenshots. |
| Peer review | `peer-review/` | Reviewer identity, review date, build or commit reviewed, findings, decisions and follow-up links. Distinguish automated document review from game acceptance. |
| PR / commit | `pr-commit/` | Links to implementation and evidence commits, feature branch, pull request, review activity and integration outcome. Describe exactly what each change establishes. |
| Acceptance check | `acceptance/` | Criterion-by-criterion mapping to implementation and dated test records, unresolved defects and the reviewer's acceptance decision. |

Use a clear filename such as `S1-04_YYYY-MM-DD_build-version.md`. Replace placeholders only when recording an actual test. Keep prior evidence when builds change so the reviewed version remains traceable.

## Minimum Record Fields

| Record | Required fields |
| --- | --- |
| Implementation | Feature / issue; repository path; commit SHA or export version; platform; access/run instructions; related criterion IDs. |
| Test execution | Test ID; criterion IDs; tester; date; build version; environment; inputs and steps; expected result; actual result; outcome; evidence paths; defect references. |
| Peer review | Reviewer; date; build or commit; scope reviewed; findings; follow-up actions; decision and limitations. |
| Acceptance | Criterion ID; implementation link; dated test link; actual outcome; outstanding defect; reviewer and date; acceptance decision. |
| PR / commit | URL and SHA; branch and baseline; files changed; issue links; testing scope; review and merge state. |

Link [acceptance criteria](../docs/acceptance_criteria.md) and [planned tests](../docs/testing_plan.md) by their IDs. Expected results are instructions for testing, not observed results. Screenshots support visual claims but do not independently prove ordering logic or independent learner completion.

## Existing Workflow Evidence

[PR #5](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/5) changed only the Sprint README. Its commit `4d6af61689d5a05dd314b7d065c9a5c00963063e`, review discussion and merge record support the agreed GitHub workflow, review visibility and traceability. They do not establish Space implementation or game testing.

The existing Animal Alpha evidence remains in `Dev1_RuiYan/ICT1_Ordering_Game/`. Do not relabel Animal assets as Space implementation. The [release traceability record](../docs/release_traceability.md) identifies the preserved Alpha tree and the inspected main / branch baseline.

## Completion Gate

Before changing any Sprint feature to Complete:

1. Link its actual implementation and the build reviewed.
2. Provide dated testing evidence and actual outcomes for every relevant criterion.
3. Record the acceptance check and resolve acceptance-blocking defects.
4. Make the evidence visible through repository updates and a linked pull request.
5. Reconcile the affected child issue, parent #8 and Rui Yan's Project board status.

Keep work Todo, In Progress or Evidence Required when the corresponding evidence gate has not been met. A documentation merge and duplicate-issue closure do not complete a feature. No fake screenshots, test results or acceptance decisions should be added.
