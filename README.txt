AM/NS India — Confined Space & Gas Hazards Area Dashboard

This version contains exactly two dashboard views:
1. Confined Space
2. Gas Hazards Area

Visual update:
- Retains the AM/NS red-and-white safety theme.
- Gas Hazards Area uses industrial safety animations: flowing gas particles, live detector pulse, respirator/PPE worker visual, isolation valve and controlled pressure/blast rings.
- No black dashboard animation panels are used.

Data:
- Confined-space data is sourced from Updated CS Identification all.xlsx.
- GHA/NGHA terminology is normalized in the generated dashboard data; NGH source values are displayed as NGHA.
- Gas-hazard data is sourced from AMNS_Pune_Gas_Hazardous_Area_Safety_Register.xlsx.

GitHub:
- tools/generate_data.py regenerates confined-space data.
- tools/generate_gas_data.py regenerates gas-hazard data.
- Keep the existing GitHub Actions workflow from the previous package when deploying. It should regenerate data.json and gas_data.json whenever either workbook changes.

Safety note:
The blast/pressure animation is a visual safety simulation only. It does not represent a real explosion or operating instruction.
