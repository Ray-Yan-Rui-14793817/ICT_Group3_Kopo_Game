# Risk and Mitigation - Rui Yan / Dev1

**Owner:** Rui Yan / Dev1. **Scope:** US4 / Sprint 1.

The three risks, types, likelihoods and impacts below reproduce Rui Yan's stated judgements in the supplied Individual Risk Analysis Reflection, pages 4-5. The mitigation actions follow that reflection and the group plan. Current controls are assessed against the inspected repository and must not be confused with completed implementation or testing.

| Risk | Risk type | Likelihood | Impact | Mitigation | Evidence / current control |
| --- | --- | --- | --- | --- | --- |
| R1 - Scope drift and weak acceptance traceability | Process | Medium | High | Maintain one authoritative Sprint scope and clear ownership, priority and acceptance criteria. Review new ideas before adding them to Sprint 1. Check repository evidence before changing status to Complete. | Parent #8 and child issues #2-#4 identify Dev1 scope. The Sprint Backlog and acceptance register cover all seven items. Implementation and acceptance evidence remain required. |
| R2 - Inconsistent quality across the three Space Ordering levels | Technical and quality | Medium | Medium to High | Use the Animal Alpha learning progression as a reference. Establish one Space interaction pattern for instructions, feedback, navigation, scale and file organisation. Test each level and record evidence before completion. | Alpha assets are preserved. Criterion groups TH, HI, FB and UX and planned tests S1-01 to S1-15 define shared checks. No Space build or executed consistency tests are available. |
| R3 - Outdated branch state and asynchronous integration | Collaboration and integration | Medium | Medium to High | Fetch and pull current main before new work. Use separate feature branches, small meaningful commits and PR review. Communicate important merges and check the current baseline before integration. | PR #5 records the historic Dev1 workflow. The new documentation branch starts at fetched origin/main `8c2c2a3`; the old Dev1 branch was three commits behind that baseline. The baseline must be checked again before integration. |

## R1 - Scope and Traceability Control

The broader Beta theme includes three learning activities, hints, feedback and testing. Additional ideas can consume Sprint capacity and delay quality checks. Retain the seven-item [Sprint Backlog](sprint1_backlog.md), and keep US5 Candy and US6 Chinese Festival as Planned later Beta work.

Use [US4 #8](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/8) as the parent and #2, #3 and #4 as the core child issues. Record any scope adjustment with its rationale, owner and acceptance impact. Reconcile Rui Yan's Project board items against issues and repository evidence during review. Board reconciliation is still required; no current board change is asserted here.

## R2 - Quality Control

The completed Alpha learning progression provides a useful reference, but new Space assets can affect scale, screen balance and interaction clarity. Use the [acceptance criteria](acceptance_criteria.md) across all three levels. Execute the [testing plan](testing_plan.md) on an identified build, record defects and repeat affected checks after fixes or refactoring.

This documentation establishes the checks and evidence requirements. The shared interaction pattern, Space build, actual test outcomes and peer acceptance remain to be demonstrated.

## R3 - Repository Synchronisation Control

Team members may merge at different times, causing work to continue from an outdated `main` branch. At the 12 October 2026 checkpoint, the original `Dev1-RuiYan-Space-Theme-Ordering` branch remained at `4d6af61`, while `origin/main` was `8c2c2a3`. This is direct evidence that a previously merged feature branch can retain an older baseline.

The new `Dev1-RuiYan-Sprint1-Documentation` branch was created from the freshly fetched `origin/main`, with zero commits ahead or behind at creation. Before integration, fetch again and review any baseline changes. If an active published branch falls behind, merge the current `origin/main`, review affected Dev1 files and repeat relevant checks. Preserve history and keep other developers' work outside this change.

## Review and Escalation

Rui Yan should review scope/status discrepancies, repeated cross-level defects and branch divergence at each Sprint checkpoint. Record the affected issue, evidence gap, required action and owner. Raise blockers through the team's agreed communication channels. These controls remain ongoing responsibilities; a documentation merge does not retire the risks.
