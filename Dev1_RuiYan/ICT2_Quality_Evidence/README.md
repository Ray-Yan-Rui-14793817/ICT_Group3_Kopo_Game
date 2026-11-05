# Dev1 — ICT2 asset quality and evidence

**Checkpoint:** 5 November 2026 (Asia/Shanghai). **Owner:** Rui Yan / Dev1.

## Evidence actually available

Source: the user-supplied `ICT2_Kopo_Image_Design.zip` and `CP5047_Ass2_Dev1_RuiYan_GitHub_Update_Plan.md`. The ZIP SHA-256 is recorded in the validation output. The plan is a source of reported design progress and earlier quality concerns; it is not an executed test log.

- [Asset manifest](testing/asset_manifest.json): original ZIP paths, repository paths, byte sizes, Git blob hashes and whether the asset was already present in main.
- [Static validation](testing/asset_validation.json): 78 PNGs verified and fully decoded with Pillow; 2 JSON maps parsed and tile-layer lengths checked. Button dimensions, alpha extrema and file sizes are measured. A 324 × 115 image can fit three 108 × 115 cells; visible pixels in each cell do not independently establish correct frame order or icon meaning.
- The 15 Space PNGs already in main match the source ZIP byte for byte by Git blob SHA-1 and are unchanged.
- All 80 source assets are preserved across the theme folders and refinement evidence. There are 65 newly added source files: 62 theme PNGs, 1 unsuitable Pause PNG retained as evidence, and 2 JSON files.

These are automated static asset checks. No KOPO interaction tests, child UAT, independent human review or peer acceptance were performed during this update. No screenshots or review comments absent from the supplied files have been fabricated.

## Quality record

| Concern | Expected | Observed evidence | Action in this update | Status / next step |
| --- | --- | --- | --- | --- |
| Candy Pause final export | Per supplied plan: transparent 324 × 115 PNG, three 108 × 115 cells, ≤80,000 bytes, distinct Pause meaning | Source is RGBA, 1536 × 1024, 2,470,318 bytes; it cannot meet the specified cell geometry | Preserve [the exact source image](refinement/Candy%20Pause%20Button%20png.png) outside the Candy theme asset directory | Specification check failed; Rui Yan to supply/confirm the actual final sprite, then perform visual and runtime checks |
| Candy Resume size | Actual KOPO limit must be confirmed | 80,640 bytes: exceeds 80,000 but fits 80 KiB | Preserve original bytes and document both thresholds | Pending limit confirmation; compress only if the true limit requires it |
| Candy Pause / Exit distinguishability | Clear, distinct Pause and Exit meaning | Earlier duplication and refinement are reported in the supplied plan; this ZIP does not establish a verified final Pause export or executed retest | Record the concern; do not label the supplied image as an approved After version | Visual and runtime retest pending; no reviewer named |
| Candy Restart styling | Consistent controls | Deferred styling concern reported in the supplied plan | Preserve the source sprite; no styling change performed | Deferred follow-up; no Complete or Retest Pass claim |
| Space Drop Box visibility | Clearly visible target in the active game | Existing source image available; earlier alternative comparisons are reported but not attached in this ZIP | Preserve existing Space bytes and record the evidence gap | Selection and KOPO placement testing pending |
| Chinese Festival active design variants | Identify assets actually used in KOPO | Two Drop Box PNGs plus a generically named PNG are supplied; no usage map | Preserve both variants and original names | Owner confirmation and platform compatibility check pending |
| Tilemap provenance / dependency | Confirm export actually used and resolve referenced image | Both maps use Git blob `088394b2e3300d9e177683ff56fe2ec46d8e56de`, also present in ICT1. Both reference `background.png`; Chinese Festival provides a differently named background | Preserve original JSON beside each theme's source designs | Not an integration-ready export; confirm use and resolve the Chinese reference before import |

## Assessment 2 traceability

The theme folders and asset PR support the image-design contribution in Section 1. The measurements and open concerns above support static quality findings for Section 2. The unsuitable Pause image supports an observed specification failure, but this update supplies no corrected After asset or runtime retest for Section 3. A future independent PR review can support Section 4 only after it actually occurs.

## Remaining evidence

Rui Yan should identify active KOPO versions, confirm the Pause sprite and tilemap usage, and supply actual test records where available. A future test record should identify the version, date, tester, expected and actual behaviour, result and evidence URL. A teammate's review and acceptance decision should be linked only after that review occurs.

PR #20 remains a separate historical documentation proposal. No shared Project Board fields, other developer content or earlier issue states are changed by the asset files in this branch.
