# Sprint 1 Acceptance Criteria - Rui Yan / Dev1

**Parent:** [US4 #8](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/8)

These working acceptance criteria translate the agreed seven-item Sprint Backlog into observable checks. They retain the size, quantity and number learning goals from the Alpha baseline. Confirm the checks during peer review before acceptance. All acceptance results are **Evidence Required**; no criterion has been verified as passed.

The planned test IDs refer to the [testing plan](testing_plan.md). Each acceptance record must identify the criterion, implementation path, build commit, test result, evidence and reviewer. Passing a document review alone does not pass a game criterion.

## Space Theme Details

| ID | Acceptance criterion | Planned tests |
| --- | --- | --- |
| TH-01 | All three levels use a consistent space background and visual style. Objects and controls remain distinguishable from the background. | S1-01, S1-12 |
| TH-02 | The game journey identifies Size, Quantity and Number Ordering. A user can reach and complete each level without a broken transition. | S1-02, S1-13 |
| TH-03 | Space assets and a build or platform export are stored under Dev1 with the version and access instructions needed to reproduce the journey. | S1-01, S1-16 |

## Space Size Ordering - Child #2

**Priority:** High. **Estimate:** 2. **Status:** Evidence Required.

| ID | Acceptance criterion | Planned tests |
| --- | --- | --- |
| SZ-01 | Space objects have clearly different visible sizes, with an unambiguous smallest-to-biggest sequence. | S1-03 |
| SZ-02 | The child can arrange the objects from smallest to biggest. The correct sequence is accepted; an incorrect or incomplete sequence is not accepted as correct. | S1-04 |
| SZ-03 | A short instruction stating the ordering direction is visible while the task is active. | S1-09 |
| SZ-04 | An incorrect order receives a gentle retry message or simple hint, and the child can change the order. | S1-10, S1-14 |
| SZ-05 | The correct order receives positive feedback. Results are supported by dated testing evidence for the identified build. | S1-11, S1-18 |

## Space Quantity Ordering - Child #3

**Priority:** High. **Estimate:** 2. **Status:** Todo.

| ID | Acceptance criterion | Planned tests |
| --- | --- | --- |
| QTY-01 | The level presents groups representing 1, 2, 3, 4 and 5 space objects. Objects are separated enough to count accurately. | S1-05, S1-12 |
| QTY-02 | The child can arrange groups from fewest to most. The correct sequence is accepted; incorrect or incomplete sequences are not accepted as correct. | S1-06 |
| QTY-03 | A short, visible instruction explains the direction and supports the counting task. | S1-09 |
| QTY-04 | Incorrect orders receive a simple counting hint or gentle retry. Correct orders receive positive feedback, with dated testing evidence. | S1-10, S1-11, S1-18 |

## Space Number Ordering - Child #4

**Priority:** High. **Estimate:** 2. **Status:** Todo.

| ID | Acceptance criterion | Planned tests |
| --- | --- | --- |
| NUM-01 | Number cards show 1, 2, 3, 4 and 5 once each. Numerals are large, readable and distinguishable from decorative artwork. | S1-07, S1-12 |
| NUM-02 | The child can arrange cards from smallest to largest. Only the complete ascending sequence 1, 2, 3, 4, 5 is accepted as correct. | S1-08 |
| NUM-03 | A short instruction states the ordering direction and stays visible during the task. | S1-09 |
| NUM-04 | An incorrect order receives gentle retry support; a correct order receives positive feedback. Dated tests verify both paths and the ordering logic. | S1-10, S1-11, S1-18 |

## Hints and Instructions

| ID | Acceptance criterion | Planned tests |
| --- | --- | --- |
| HI-01 | Each level shows a short instruction that names its learning task and ordering direction. It remains legible during interaction. | S1-09, S1-12 |
| HI-02 | A simple hint is available when support is needed or an incorrect order is submitted. It relates to size, counting or number order as appropriate. | S1-10 |
| HI-03 | After a hint or retry message, the child can continue arranging objects. The hint does not hide essential controls or trigger a false success. | S1-10, S1-14 |

## Positive / Gentle Feedback

| ID | Acceptance criterion | Planned tests |
| --- | --- | --- |
| FB-01 | Correct answers receive visible positive feedback in every level. Success feedback is tied to the correct ordering result. | S1-11 |
| FB-02 | Incorrect or incomplete answers receive supportive retry feedback without being counted as successful. The user can attempt the task again. | S1-10, S1-14 |
| FB-03 | Repeated retries followed by a correct answer produce the correct feedback state. Feedback wording and behaviour are consistent across all three levels. | S1-11, S1-13 |

## Basic Usability and Cross-Level Consistency

| ID | Acceptance criterion | Planned tests |
| --- | --- | --- |
| UX-01 | Instructions, objects, numerals and controls are readable and usable in the recorded target viewport and input mode. Essential content is not clipped or obscured. | S1-12 |
| UX-02 | Level entry, ordering direction, hints, retry and completion follow a consistent interaction pattern across the three-level journey. | S1-02, S1-13 |
| UX-03 | Arranging objects, retrying and repeating a level do not lose cards, duplicate answers or leave controls blocked. | S1-14 |
| UX-04 | Usability observations record whether a learner can understand the instruction and complete a level without task assistance. Any required assistance or confusion is recorded for review. | S1-15 |

An adult walkthrough can identify usability concerns, but does not establish that children aged 4-6 can complete a level independently. Record participant context and the limits of any usability evidence.

## Sprint 1 Testing and Acceptance Review

| ID | Acceptance criterion | Planned tests |
| --- | --- | --- |
| TEST-01 | A dated record covers every relevant acceptance criterion and states the build, environment, tester, inputs, expected result, actual result and evidence path. | S1-18 |
| TEST-02 | Functional ordering, instructions, hints, feedback, basic usability, cross-level consistency and integration are checked on an accessible Space build. | S1-01 to S1-18 |
| TEST-03 | Defects are recorded with affected criteria. Failed checks are fixed and repeated on the updated build before acceptance. | S1-17, S1-18 |
| TEST-04 | The acceptance reviewer can follow issue-to-implementation-to-test links. All required checks pass and no acceptance-blocking defect remains before an item becomes Complete. | S1-16, S1-18 |

## Completion Decision

Use the [evidence guide](../evidence/README.md) to attach implementation, testing, peer review, PR / commit and acceptance records. Update the affected child issue and parent #8 with those links. Keep a feature open if any required criterion lacks evidence or fails. Closing duplicate #9 is an administrative action and does not pass acceptance.
