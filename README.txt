AM/NS India - Confined Space & Gas Hazards Area Dashboard
===============================================================

This GitHub Pages-ready dashboard now contains exactly TWO dashboard pages:
- Confined Space Dashboard
- Gas Hazards Area Dashboard

There is NO separate Common Safety Dashboard page.

Visual design:
- Light professional safety theme (blue / teal / green / amber / red accents)
- No black-heavy safety animation
- Animated atmosphere-monitoring, gas-detection and safety-control graphics
- Responsive layout for desktop and mobile

Important terminology:
- "Gas Hazardous Area" and "Confined Space" are different safety classifications.
- A location can be both, but one term must not be used as a substitute for the other.

Confined Space register:
- Source: Updated CS Identification all.xlsx
- Complete identification register and department entry registers are retained.
- GHA / NGHA is normalized to the dashboard labels GHA and NGHA.
- Current source count: 121 confined spaces = 64 GHA + 57 NGHA.
- The GHA / NGHA filter is directly above the identification table.

Gas Hazards Area register:
- Source: AMNS_Pune_Gas_Hazardous_Area_Safety_Register.xlsx
- Complete 16-area Hazard Assessment Matrix is displayed.
- Filters are directly above the master table.

Automatic GitHub update:
1. Replace/edit either Excel workbook in the repository.
2. Push the change to GitHub.
3. GitHub Actions runs both generator scripts.
4. data.json and gas_data.json are regenerated and committed automatically.
5. GitHub Pages then serves the updated dashboard.

SOP / HIRAC:
- Both dashboard pages use the same Open SOP / Open HIRAC response buttons in record details.
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
