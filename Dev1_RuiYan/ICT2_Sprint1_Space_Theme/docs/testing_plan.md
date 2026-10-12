# Sprint 1 Testing Plan - Rui Yan / Dev1

**Scope:** US4 - Space Theme Ordering Game, parent #8 and child issues #2, #3 and #4.

This is a plan for future execution. All tests are **Planned**. No test run, screenshot, passed result or acceptance decision is asserted. Implementation and an accessible identified Space build are required before these checks can be performed.

## Execution Requirements

Rui Yan records the build commit or platform-export version, access steps, platform/browser version, viewport, input mode, test date and tester. Use the [acceptance criteria](acceptance_criteria.md) as the coverage register. Record actual results separately from expected results in `evidence/testing/` when execution occurs.

For ordering logic, use unit tests where source or platform tooling permits. Include correct order, reversed order, a swapped pair and an incomplete answer. Include duplicate or missing values where the platform permits those states. Verify that only valid complete orders receive success. Manual functional checks remain necessary for the rendered game and its feedback.

## Planned Test Cases

| Test ID | Area | Test / Expected Result | Status | Evidence |
| --- | --- | --- | --- | --- |
| S1-01 | Space theme / functional | Load all three levels. Space backgrounds and assets display consistently; controls and task objects remain distinct. Check TH-01 and TH-03. | Planned | Required: build identity, asset paths and observed screenshots. |
| S1-02 | Three-level journey | Enter and complete Size, Quantity and Number Ordering. Each level is identifiable; transitions and re-entry work. Check TH-02 and UX-02. | Planned | Required: journey steps, actual results and recording or screenshots. |
| S1-03 | Size comparison | Inspect the displayed objects and their intended size ranking. Visible sizes support one unambiguous smallest-to-biggest order. Check SZ-01. | Planned | Required: size ranking, asset references and visual observations. |
| S1-04 | Size ordering logic | Submit the correct size sequence, reversed order, a swapped pair and an incomplete answer. Accept only the correct complete order. Check SZ-02. | Planned | Required: submitted sequences, expected/actual results and build reference. |
| S1-05 | Quantity representation | Count objects in every group. Groups contain 1-5 objects with readable separation and no hidden or extra objects. Check QTY-01. | Planned | Required: group counts, screenshots and observations. |
| S1-06 | Quantity ordering logic | Arrange groups from fewest to most, then try reversed, swapped and incomplete orders. Accept only the correct complete sequence. Check QTY-02. | Planned | Required: input sequences, expected/actual results and build reference. |
| S1-07 | Number recognition | Check that cards show 1-5 once each and numerals are readable in the target viewport. Check NUM-01. | Planned | Required: card references, viewport and visual observations. |
| S1-08 | Number ordering logic | Submit 1,2,3,4,5; reversed and swapped orders; and an incomplete answer. Try missing/duplicate values if supported. Accept only the valid complete ascending sequence. Check NUM-02. | Planned | Required: inputs, expected/actual results and logic output where available. |
| S1-09 | Instruction clarity | Read the instruction in each level before and during interaction. It stays visible, states the task and gives the correct direction. Check SZ-03, QTY-03, NUM-03 and HI-01. | Planned | Required: instruction wording, screenshots and reviewer observations. |
| S1-10 | Hints / gentle retry | Request support or submit an incorrect answer in each level. Show a relevant simple hint or gentle retry message, allow rearrangement and avoid false success. Check SZ-04, QTY-04, NUM-04, HI-02, HI-03 and FB-02. | Planned | Required: trigger, actual message, retry steps and observed outcome. |
| S1-11 | Positive feedback / state | Submit correct answers, including after repeated retries. Show positive feedback only for correct orders, with no stale retry or success state. Check SZ-05, QTY-04, NUM-04, FB-01 and FB-03. | Planned | Required: inputs, feedback observations and screenshots or recording. |
| S1-12 | Basic usability / readability | Inspect all levels in the recorded mobile target viewport and input mode. Text, numbers, groups and controls remain legible, distinct and usable without clipping. Check TH-01, QTY-01, NUM-01, HI-01 and UX-01. | Planned | Required: environment details, screenshots and usability observations. |
| S1-13 | Cross-level consistency | Compare navigation, instructions, hint behaviour, retry and completion across all three levels. Use one consistent interaction pattern. Check TH-02, FB-03 and UX-02. | Planned | Required: comparison notes and per-level outcomes. |
| S1-14 | Interaction reliability | Arrange objects, retry and repeat each level. No cards disappear or duplicate; controls stay usable. Check SZ-04, HI-03, FB-02 and UX-03. | Planned | Required: reproduction steps, actual results and defect links if needed. |
| S1-15 | Learner usability | Observe instruction understanding and level completion. Record whether task assistance is needed and where confusion occurs. Check UX-04; state participant context and evidence limitations. | Planned | Required: observation notes, support provided and findings. |
| S1-16 | Integration / repository | Fetch current main, inspect the Dev1 PR diff, verify build/evidence paths and issue links, and check the integrated Dev1 build at review. Preserve Alpha and other developers' files. Check TH-03 and TEST-04. | Planned | Required: main and feature SHAs, diff summary, build check and reviewer record. |
| S1-17 | Regression / refactoring | After a defect fix or refactoring, repeat the affected functional, feedback and cross-level checks on the new build. Record results and outstanding defects. Check TEST-03. | Planned | Required: defect reference, fix commit and dated rerun results. |
| S1-18 | Acceptance review / coverage | Map every criterion to dated actual results and implementation evidence. Complete only when required checks pass and no acceptance-blocking defect remains. Check SZ-05, QTY-04, NUM-04 and TEST-01 to TEST-04. | Planned | Required: acceptance matrix, build identity and reviewer decision. |

## Result Records and Defect Handling

For every executed case, record Test ID, criterion IDs, date, tester, environment, build version, inputs/steps, expected result, actual result, Pass/Fail/Blocked, evidence paths and defect references. Keep older results when the build changes. Evidence must identify which build was tested.

A failed or blocked check keeps the related feature open. Link defects from the relevant Rui Yan issue; do not treat an expected result as an observed result. Repeat affected tests after fixes. Use peer review to confirm acceptance coverage and the limits of usability observations.

## Completion Gate

Sprint 1 Testing remains Todo while this plan has no execution records. It becomes In Progress when dated execution begins. It becomes Complete only when the planned scope has recorded results, relevant acceptance checks pass, blocking defects are resolved and the reviewer can inspect repository evidence.

Documentation verification for this cleanup is separate from game testing. Markdown links, backlog values and change scope can be checked without claiming S1-01 to S1-18 were executed.
