# Dev1 — ICT2 Beta completion and Assessment 2 evidence

**Recorded:** 5 November 2026 (Asia/Shanghai). **Developer:** Rui Yan / Dev1.

## Completion basis

In the current user request, Rui Yan explicitly confirms that US5 Candy and US6 Chinese Festival **game design, three-level KOPO implementation and game testing are completed**. The three levels are Size Ordering, Quantity Ordering and Number Ordering. This confirmation concerns the completed games, independently of the draft GitHub asset synchronisation PR.

**Game Testing: Completed — confirmed by Dev1 Rui Yan; supporting evidence links to be consolidated.**

The source Assessment 2 Group Report was inspected directly. The linked images below reproduce its actual Dev1 content; page numbers are 1-based PDF pages. They are evidence of what the report contains. No missing test dates, pass counts, execution logs or reviewer approvals have been supplied by inference.

## Section 1 — implemented functionality and screenshots

| Story | Verified report content | KOPO link | Repository evidence |
| --- | --- | --- | --- |
| US4 Space | pp. 2–3 describe all three ordering activities; p. 3 includes a Space Level 3 screenshot | [Space](https://www.kopo.com/g/game.php?gno=14378&lid=5377&thmno=5109) | [Report p. 3](report_section1_us4_us5.png); merged PR #21; remaining level images in PR #22 |
| US5 Candy | p. 3 describes the theme and contains Level 1, Level 2 and Level 3 gameplay screenshots | [Candy](https://www.kopo.com/g/game.php?gno=14378&lid=5381&thmno=5112) | [Actual three-level screenshots](report_section1_us4_us5.png); [theme assets](../../ICT2_Candy_Theme/) |
| US6 Chinese Festival | p. 4 describes the theme and contains Level 1, Level 2 and Level 3 gameplay screenshots | [Chinese Festival](https://www.kopo.com/g/game.php?gno=14378&lid=5391&thmno=5142) | [Dev1 portion of report p. 4](report_section1_us6.png); [theme assets](../../ICT2_Chinese_Festival_Theme/) |

Figure descriptions: p. 3 shows Candy's Size, Quantity and Number Ordering instructions, themed objects, answer targets and level indicators, with Space Level 3 above it. The p. 4 Dev1 crop shows Chinese Festival's three level screens and familiar themed objects; the following Dev2 section is excluded. The game URLs were also checked against the report's embedded links and open the named KOPO games.

## Section 2 — completed testing and evidence coverage

| Area | Completion / available evidence | Documentation limit |
| --- | --- | --- |
| Size, Quantity and Number Ordering — US5 and US6 | **Completed — developer confirmed.** Report pp. 3–4 show all six relevant level screens | A screenshot is not a complete per-case execution log. Detailed expected/actual outcomes and historical execution dates are not invented |
| Instructions, visual clarity and recognisable objects | Level instructions, themed images and answer targets are visible in the report screenshots; Candy Level 1 also rendered during the current targeted inspection | No new child-usability judgement or child UAT is claimed |
| Placement / Drop Box interaction | Report screenshots show an object positioned in a target; developer confirms completed game testing | Full drag/drop, invalid-placement and ordering-result logs are not individually documented in these excerpts |
| Positive and incorrect-answer feedback | Included within the developer-confirmed completed game testing | No separate correct/incorrect-answer execution record was located in the inspected Dev1 excerpts; supporting links remain to be consolidated |
| Candy Pause / Exit | Week 6 Activity 3 records duplicated icons; Activity 5 records a distinct Pause icon and **Retest result: Pass** | This is a reported historical retest. The document gives no precise execution date or pass count; none is added |
| Other controls / Chinese Festival controls | Overall testing is completed, developer confirmed; Week 6 Test 2 describes Restart as recognisable and functional | No new control-by-control acceptance log or independent approval is claimed |

Missing documentation links remain follow-up work. They do not change completed US5/US6 testing to Todo. The current repository task did not rerun a comprehensive three-level test suite.

## Section 3 — Candy Pause / Exit refinement

- [Week 6 Activity 3 — Before comparison, report p. 35](../refinement/week6_pause_exit_before.png): Pause and Exit shared the same door-and-arrow icon. The selected concern is semantic distinction and interaction clarity.
- [Week 6 Test 2 — report p. 36](../refinement/week6_restart_followup.png): Restart's border/decorative styling is a separate concern, explicitly deferred beyond this bounded change.
- [Week 6 Activity 5 — Before/After and retest, report p. 40](../refinement/week6_pause_exit_after_retest.png): the Pause icon is refined; Exit, Restart, Resume, frame geometry, logic, learning activities and overall mechanics are retained. The report records **Retest result: Pass**. Its last sentence continues on the source report's next page.

The current running Candy game loads KOPO image file ID `232120`. Its bytes exactly match [the local Pause sprite now preserved in the theme directory](../../ICT2_Candy_Theme/Candy_Themes_design/candy_pause_button.png): 324 × 115, 15,106 bytes, PNG palette transparency, three nonempty 108 × 115 frame cells, SHA-256 `8349165bd256dc9a5e7be94d43e66a6a89245a9e83559d936b8bb989e6ada1aa`. This resolves which of the supplied local Pause versions is active. No game asset or KOPO logic was changed by this repository update.

The original oversized ZIP image remains separate as source evidence. The runtime byte match, measured sprite properties and report's historical retest are distinct evidence types. [Validation and provenance](assessment2_evidence_validation.json) records those distinctions.

## Section 4 — actual repository coordination and approval

- [Asset and documentation PR #22](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/pull/22) contains only Dev1 changes and preserves per-theme commits.
- [US5 #23](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/23) and [US6 #24](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/24) record completed games. [Follow-up #25](https://github.com/Ray-Yan-Rui-14793817/ICT_Group3_Kopo_Game/issues/25) separately tracks asset synchronisation, evidence documentation and independent review.
- [Existing Project Board](https://github.com/users/Ray-Yan-Rui-14793817/projects/2) uses Todo / In Progress / Done; current release ownership is Rui Yan / Dev1, ICT2 Beta / Assessment 2. Shared project conventions and earlier US4 states are retained.
- Report p. 44 describes shared Candy UI review as a collaborative practice. This report description is not represented as a submitted approval on PR #22. No reviews were returned for that PR when inspected.

Remaining work is limited to the open PR/review, consolidating detailed existing test-document links, the formal Resume size rule, standalone tilemap usage and deferred Restart styling, as tracked in #25.
