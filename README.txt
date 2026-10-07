# AM/NS Confined Space Dashboard

Upload the contents of this package to the root of your GitHub repository.

Files:
- `index.html` — dashboard
- `amns-logo.png` — AM/NS logo
- `Updated CS Identification all.xlsx` — source workbook
- `data.json` — generated dashboard dataset
- `tools/generate_data.py` — Excel-to-JSON converter
- `.github/workflows/update-data.yml` — automatically regenerates `data.json` when the Excel file changes

## Updating Excel
Replace `Updated CS Identification all.xlsx` with the new workbook using the same filename and commit it. GitHub Actions will regenerate `data.json`.

## SOP / HIRAC links
Open `index.html` and find `DOCUMENT_LINKS`.
You can set:
- `defaultSOP`
- `defaultHIRAC`
or individual links under `records` keyed by Identification No.

Examples:
`defaultSOP: "docs/confined-space-sop.pdf"`
`defaultHIRAC: "docs/confined-space-hirac.pdf"`

The dashboard has no file-upload control for viewers.
