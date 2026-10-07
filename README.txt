AMNS Confined Space Dashboard

Files to upload to the ROOT of the GitHub Pages repository:
- index.html
- Updated CS Identification all.xlsx
- .nojekyll

Important:
1. index.html must remain exactly this name.
2. Keep the Excel file name exactly: Updated CS Identification all.xlsx
3. GitHub Pages should be configured from the repository root (/).
4. The dashboard is self-contained and does NOT depend on a CDN or Python.
5. The dashboard first displays the embedded workbook snapshot, then reads the current Excel file from the same GitHub Pages folder.
6. When the Excel file is replaced and committed, use Refresh Excel or wait for the automatic refresh.
7. If Excel cannot be read, the existing dashboard data remains visible instead of going blank.
8. For local/offline use, use Load Excel File to select the workbook.
9. SOP/HIRAC URLs can be added in the SOP_LINKS and HIRAC_LINKS objects near the top of the script in index.html, keyed by Identification No.
