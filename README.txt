AM/NS India — Confined Space & Gas Hazards Area Dashboard

TWO DASHBOARD VIEWS
1. Confined Space
2. Gas Hazards Area

DATA SOURCES
- Confined-space data: Updated CS Identification all.xlsx
- Gas-hazard data: AMNS_Pune_Gas_Hazardous_Area_Safety_Register.xlsx
- NGH source values are normalized and displayed as NGHA.
- Size values in the entry register are normalized to mm format.

AUTOMATIC EXCEL -> WEBSITE UPDATE
The repository includes .github/workflows/deploy-dashboard.yml.

When either workbook is changed on GitHub and the change is pushed to the
main or master branch, GitHub Actions automatically:
1. Reads the updated Excel workbook.
2. Runs tools/generate_data.py.
3. Runs tools/generate_gas_data.py.
4. Builds the current dashboard with the newly generated data.
5. Deploys the updated dashboard to GitHub Pages.

IMPORTANT: Editing an Excel file only on your iPhone/PC does NOT change the
live website. The updated Excel workbook must be uploaded/committed to the
GitHub repository (or pushed with git). Once GitHub receives that commit,
the workflow updates the live dashboard automatically.

FIRST-TIME GITHUB PAGES SETUP
1. Upload the contents of this folder to a GitHub repository.
2. Use the main branch (or master) for the repository.
3. In GitHub: Settings -> Pages -> Build and deployment, choose GitHub Actions.
4. Push/change either Excel workbook.
5. Open Actions and wait for 'Build and Deploy AMNS Safety Dashboard' to finish.
6. The Pages URL shown by the workflow is the live dashboard.

The workflow is intentionally triggered by Excel changes plus dashboard/tool
changes, so future workbook updates refresh the live site without manually
editing data.json or gas_data.json.

SAFETY NOTE
The blast/pressure animation is a visual safety simulation only. It does not
represent a real explosion or operating instruction.
