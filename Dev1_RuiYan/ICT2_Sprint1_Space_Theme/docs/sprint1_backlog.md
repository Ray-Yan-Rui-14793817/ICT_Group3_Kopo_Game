# Sprint 1 Backlog - Rui Yan / Dev1

- **Parent:** [US4 - Space Theme Ordering Game #8](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/8)
- **Owner:** Rui Yan / Dev1
- **Release:** ICT2 Beta / Sprint 1
- **Status checkpoint:** 12 October 2026 (Asia/Shanghai)

## Agreed Sprint Backlog

The feature descriptions, priorities and estimates match Table 2 in the supplied Assessment 1 Group 3 Project Plan, pages 18-19. They also match Table 1 in Rui Yan's Individual Risk Analysis Reflection, page 2. Medium is written as Med in those tables. Estimates total 10; the source does not specify an estimate unit.

| Feature | Description | Priority | Estimate | Status |
| --- | --- | --- | --- | --- |
| Space Theme Details | Create a consistent space background, visual style and three-level game journey. | High | 1 | Todo |
| [4.1 Space Size Ordering #2](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/2) | Create clearly different-sized space objects and allow children to arrange them from smallest to biggest. | High | 2 | Evidence Required |
| [4.2 Space Quantity Ordering #3](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/3) | Create groups containing 1-5 space objects and allow children to arrange them from fewest to most. | High | 2 | Todo |
| [4.3 Space Number Ordering #4](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/4) | Create large and readable number cards 1-5 and allow children to arrange them from smallest to largest. | High | 2 | Todo |
| Hints and Instructions | Provide short instructions and simple hints when the child needs support or selects an incorrect order. | Medium | 1 | Todo |
| Positive / Gentle Feedback | Provide positive feedback for correct answers and gentle retry feedback for incorrect answers. | Medium | 1 | Todo |
| Sprint 1 Testing | Test all three levels, hints, feedback and basic usability before review. | Medium | 1 | Todo |

## Status evidence

The inspected `main` and original Dev1 branch contain a Sprint README rather than a Space implementation. [PR #5](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/5) reported Size Ordering as In Progress, but changed only that README. Size Ordering therefore requires implementation evidence to verify progress. Quantity and Number Ordering were recorded as Todo. The remaining four items are agreed scope without implementation or test execution evidence.

No item is Complete. The [working document](../Readme.md#sprint-1-scope-and-current-status) records the evidence for each row. Planned, Todo, In Progress, Evidence Required and Complete follow the [Dev1 status rules](../../readme.md#status-and-completion-rules).

## Dependencies and scope control

Space Theme Details supplies the shared visual and three-level journey baseline. Each ordering level requires its own assets and correct logic. Instructions, hints and feedback must be checked within all three levels. Sprint 1 Testing depends on an accessible identified build; planned checks should guide implementation from the start.

US5 Candy and US6 Chinese Festival remain Planned in the Product Backlog. New visual or interaction ideas require scope review before entering Sprint 1. The existing Alpha learning progression provides a reference, while new Space assets and behaviour still require verification.

At Sprint review, Rui Yan should reconcile this table with #8, child issues #2-#4 and the Dev1 Project board items. Attach implementation and testing evidence before changing a feature to Complete. A documentation merge is a planning checkpoint and must not close the feature issues.
