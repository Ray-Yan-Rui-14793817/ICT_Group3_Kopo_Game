# ICT2 Sprint 1 - Space Theme Ordering Game

- **Developer:** Rui Yan / Dev1
- **Release:** Beta / Sprint 1
- **Parent:** [US4 #8](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/8)
- **Evidence checkpoint:** 12 October 2026 (Asia/Shanghai)
- **Overall status:** Evidence Required

## Sprint Goal

Extend the ICT1 Animal Ordering Alpha learning progression into a consistent three-level Space Theme Ordering Game. Develop size, quantity and number ordering with short instructions, hints and positive / gentle feedback. Record functional, usability and acceptance testing evidence before review.

## User Story

> As a Kindergarten Student, I want to play a Space Theme Ordering Game so that I can practise size comparison, quantity comparison, and number recognition and ordering through an engaging space theme.

## Sprint 1 Scope and Current Status

| Item | Priority | Estimate | Current status | Evidence supporting the status |
| --- | --- | --- | --- | --- |
| Space Theme Details | High | 1 | Todo | Included in Assessment 1 and the US4 checklist. No Space background, visual assets or three-level journey export found. |
| [4.1 Space Size Ordering #2](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/2) | High | 2 | Evidence Required | PR #5 and the prior README reported In Progress. Their change is documentation only; no implementation or test artefact supports verification. |
| [4.2 Space Quantity Ordering #3](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/3) | High | 2 | Todo | PR #5 reported Todo. No Space quantity implementation or testing evidence found. |
| [4.3 Space Number Ordering #4](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/4) | High | 2 | Todo | PR #5 reported Todo. No Space number implementation or testing evidence found. |
| Hints and Instructions | Medium | 1 | Todo | Included in the agreed Sprint Backlog. No implemented Space instructions, hints or test records found. |
| Positive / Gentle Feedback | Medium | 1 | Todo | Included in the agreed Sprint Backlog. No implemented Space feedback or observed outcomes found. |
| Sprint 1 Testing | Medium | 1 | Todo | Test execution records and acceptance results are missing. The testing plan below is planned work. |

Estimates reproduce the project plan values and total 10. The source does not specify an estimate unit. US5 Candy and US6 Chinese Festival remain Planned later Beta work and are outside Sprint 1. The [Sprint Backlog](docs/sprint1_backlog.md) records descriptions and dependencies.

## Acceptance Criteria

The [acceptance register](docs/acceptance_criteria.md) provides individual criterion IDs and test links. The working checks cover:

- **Space Theme Details:** a consistent space background, visual style and identifiable three-level journey.
- **Space Size Ordering:** clearly different sizes can be arranged from smallest to biggest; incorrect orders receive gentle retry support and correct orders receive positive feedback.
- **Space Quantity Ordering:** countable groups represent 1-5 objects and can be arranged from fewest to most.
- **Space Number Ordering:** readable cards 1-5 can be arranged from smallest to largest with correct ordering logic.
- **Hints and Instructions:** short instructions remain visible; simple hints support retry without blocking interaction.
- **Positive / Gentle Feedback:** correct and incorrect outcomes are accurate, supportive and consistent across the three levels.
- **Basic usability:** instructions, cards and controls remain readable in the recorded target environment; the three-level journey and retry flow can be completed without blocked controls.
- **Sprint 1 Testing:** dated functional, usability, consistency and integration records support each criterion before acceptance.

These are testable working checks derived from the supplied scope. Peer confirmation and execution remain required. No criterion has been marked as passed.

## Evidence Required Before Completion

Every feature requires:

1. Implementation evidence: repository paths, a commit SHA and a runnable build or platform export with access instructions.
2. Testing evidence: test IDs, build identity, environment, date, tester, actual results and supporting records.
3. An acceptance-criteria check: criterion IDs linked to results, with unresolved defects stated.
4. A visible repository update: linked issues and a pull request that identifies the implementation and evidence reviewed.

Use the [evidence guide](evidence/README.md). A screenshot alone does not verify ordering logic. A merged documentation pull request does not complete US4. No new implementation, screenshots or test results are supplied by this documentation update.

## Status Rules

**Planned** identifies later Product Backlog items and unexecuted tests. **Todo** identifies selected work with no supported start. **In Progress** requires linked active implementation. **Evidence Required** identifies claims awaiting implementation, testing or acceptance records. **Complete** requires all completion checks above. The [Dev1 overview](../readme.md#status-and-completion-rules) defines these states.

The earlier In Progress wording for Size Ordering is preserved in [PR #5](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/5) and Git history. This checkpoint uses Evidence Required because the inspected repository cannot verify that claim. Planning documentation is available; feature delivery remains unverified.

## Testing Plan

The [testing plan](docs/testing_plan.md) covers functional checks, ordering logic, instruction clarity, feedback behaviour, basic usability, cross-level consistency and integration. Every test is Planned. Testers must record actual results against an identified build and repeat affected checks after defects or refactoring.

## GitHub Workflow

1. Fetch `origin` and pull the latest `main` with `git pull --ff-only origin main` before new work.
2. Create a Rui Yan feature branch from the synchronised `main`. Keep changes within `Dev1_RuiYan/**`.
3. Make small meaningful commits. Link issues and record the purpose of each change.
4. Push the feature branch regularly so progress is visible.
5. Open a pull request into `main` with scope, acceptance checks, testing evidence and remaining gaps.
6. Review before integration. Synchronise after important merges; merge the latest `origin/main` into an active published branch when needed, without rewriting history.

The documentation branch is `Dev1-RuiYan-Sprint1-Documentation`, created from fetched `origin/main` at `8c2c2a39bbd20c4a49ea0db0c2fe0d4aa37888b8`. Its starting commit matched `origin/main` with zero commits ahead or behind. The original `Dev1-RuiYan-Space-Theme-Ordering` branch is retained. [PR #5](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/5) evidences the agreed workflow, review visibility and traceability of a README update.

## Integration Risk

Team members may merge at different times, causing work to continue from an outdated `main` branch. Fetch and pull the latest `main`, use separate feature branches and small meaningful commits, review pull requests, and communicate important merges. These controls work together; branch isolation alone does not keep the baseline current.

The [risk and mitigation record](docs/risk_and_mitigation.md) also covers scope drift and inconsistent quality across the three Space Ordering levels.

## Release Traceability and Remaining Gaps

[Release traceability](docs/release_traceability.md) connects the preserved Alpha US1-US3, current US4 and planned US5-US6 to issues and repository evidence. Issue #8 is the authoritative parent; #2, #3 and #4 remain its child issues. Duplicate #9 is an administrative duplicate, not delivered scope.

Remaining work includes Space implementation and platform exports, a confirmed test environment, dated test execution, acceptance review and evidence links. GitHub Project board status must be checked against these records at review. No current board update or full Beta release is claimed here.
