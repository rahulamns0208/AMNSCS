AM/NS India - Confined Space & Gas Hazards Area Dashboard
===============================================================

This GitHub Pages-ready dashboard contains:
- Common Safety Dashboard
- Confined Space Dashboard
- Gas Hazards Area Dashboard

Dashboard switch:
- Common Safety Dashboard = shared safety principles and animated safety graphics.
- Confined Space = existing confined-space identification and entry register.
- Gas Hazards Area = complete 16-area Gas Hazard Assessment Matrix from the gas Excel workbook.

Important terminology:
- "Gas Hazardous Area" and "Confined Space" are different safety classifications.
- A location can be both, but one term must not be used as a substitute for the other.

Source Excel files:
- Updated CS Identification all.xlsx
- AMNS_Pune_Gas_Hazardous_Area_Safety_Register.xlsx

Automatic GitHub update:
1. Replace/edit either Excel workbook in the repository.
2. Push the change to GitHub.
3. GitHub Actions runs both generator scripts.
4. data.json and gas_data.json are regenerated and committed automatically.
5. GitHub Pages then serves the updated dashboard.

SOP / HIRAC:
- Both dashboards use the same Open SOP / Open HIRAC response buttons in the record details.
- Add controlled document URLs in DOCUMENT_LINKS inside index.html, or place PDFs in a docs/ folder and use relative paths.
- Example:
  "HAZ-01": { SOP: "docs/HAZ-01-SOP.pdf", HIRAC: "docs/HAZ-01-HIRAC.pdf" }

Files:
- index.html
- data.json
- gas_data.json
- Updated CS Identification all.xlsx
- AMNS_Pune_Gas_Hazardous_Area_Safety_Register.xlsx
- tools/generate_data.py
- tools/generate_gas_data.py
- .github/workflows/update-data.yml
