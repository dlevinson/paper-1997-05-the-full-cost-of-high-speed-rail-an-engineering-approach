# The Full Cost Of High-Speed Rail: An Engineering Approach

## Contribution

This paper provides an engineering-based full-cost assessment of proposed high-speed rail between Los Angeles and San Francisco, combining infrastructure, fleet, operations, user time, noise, pollution, and accident costs. Its intermodal comparison finds high-speed rail better positioned against automobile travel in shorter markets than against air travel over the full corridor.

## Bibliographic Information

- Row ID: `paper-1997-05`
- Year: 1997
- Authors: David M. Levinson; Jean Michel Mathieu; David Gillen; Adib Kanafani
- Venue: The Annals of Regional Science 31(2):189-215 (1997)
- DOI: https://doi.org/10.1007/s001680050045
- Citation: Levinson, David M., Jean Michel Mathieu, David Gillen, and Adib Kanafani. (1997). "The Full Cost of High-Speed Rail: An Engineering Approach." The Annals of Regional Science 31(2):189-215. https://doi.org/10.1007/s001680050045

## Package Status

- Pipeline state: `UPLOADED`
- Package boundary: final paper reference plus locally retained HSR/full-cost analysis workbooks, model notes, table exports, and selected report/chapter lineage.
- Audit timestamp: 2026-05-17 06:17:02 AEST

## Paper-First Validation

The final paper was reread directly from `/Users/dlev2617/Documents/Papers/Published Papers/HighSpeedRail.pdf`. It uses a full-cost model for high-speed rail in the Los Angeles-San Francisco corridor, including infrastructure costs, carrier fleet/capital/operating costs, user time, social costs, demand forecasts from Leavitt et al. and Vaca et al., and a train-operations optimization simulation used to estimate trainsets and schedules. The demand, infrastructure, carrier-cost, SIMEX/MATISSE simulation, user-time, social-cost/noise, intermodal comparison, end-note, and reference sections were checked against the package boundary.

The package contains the retained local HSR cost workbooks, comparison tables, noise-model workbooks, and simulation/model notes that match that paper lineage. The SIMEX/MATISSE/CalSpeed-style operational simulation files themselves were not found in the staged local source set; they are documented as missing external dependencies rather than treated as files to upload.

## Contents

- `paper/`: final paper reference copy.
- `data/analysis_workbooks/original_legacy/`: original legacy Excel workbooks.
- `data/analysis_workbooks/modernized_xlsx/`: modern `.xlsx` conversions generated from readable legacy workbooks.
- `data/analysis_workbooks/csv_exports/`: per-sheet CSV exports for inspection.
- `data/legacy_model_files/`: Lotus/no-extension noise-model and HSR-noise originals retained without conversion.
- `documentation/legacy_model_and_report_notes/`: original legacy Word documents and extracted text for HSR simulation/report methods.
- `documentation/full_cost_report/`: report cover/table-of-contents reference for UCB-ITS-RR-96-3.
- `documentation/legacy_figure_sources/`: legacy route-map figure source files.
- `documentation/SOURCE_FILE_REVIEW.csv`: file-by-file inclusion/deduplication decisions.
- `documentation/EXCLUDED_SOURCE_MATERIALS.csv`: excluded drafts, proof notes, duplicate paper PDFs, correspondence, and broad context.
- `documentation/LEGACY_MODERNIZATION_REPORT.csv`: spreadsheet/text extraction report.
- `documentation/SHARED_FULL_COST_DEDUPLICATION_NOTE.md`: cross-package deduplication note for Full Cost Project assets also used by related papers.

## External Dependencies Not Bundled

The paper cites demand forecasts and simulation/model workflows from CalSpeed/California HSR studies and references a SIMEX workbook workflow in the retained run instructions. Those source workbooks/program files were not found in this package. This is documented for provenance but is not a blocker for uploading the retained legacy analysis workbooks and method notes; a future reproduction can either locate those original external model files or rebuild the simulation from the documented method and retained cost tables.

## Release Boundary

This package contains no human-subject microdata and no raw personally identifying data. It is intended for public GitHub upload review as a legacy analysis-workbook and documentation package. Publisher-formatted paper PDF rights should still be reviewed before final public release.

<!-- package-hardening-status:start -->
## Package Hardening Status

Generated: 2026-05-20 15:23:47 AEST

- Pipeline: `UPLOADED`
- Sidecars added/updated: `PACKAGE_STATUS.md`, `PACKAGE_MANIFEST.csv`, `LICENSE_STATUS.md`.
- Paper reference copies are for local audit convenience and are not public-upload assets without rights review.
- Final GitHub upload should use the manifest include statuses and the license-status note.
<!-- package-hardening-status:end -->
