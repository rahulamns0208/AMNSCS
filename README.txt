AM/NS India - Confined Space Dashboard
======================================

Files:
- index.html — responsive dashboard UI
- data.json — generated dashboard dataset
- Updated CS Identification all.xlsx — source workbook
- tools/generate_data.py — GitHub Actions data generator
- amns-logo.png — AM/NS India logo

Entry register data:
- CRM: 5
- PICKLING: 7
- ARP: 15
- CGL: 36
- CCL: 56
- UTILITY: 12
- ADMIN: 41

The CRM C.S.ENTRY worksheet contains CRM, PICKLING and ARP records. The generator splits those records into their correct department tabs using the identification number/content, so the dashboard does not incorrectly show all 27 records as CRM.

The UI includes the AM/NS India Our Values showcase, responsive layouts for desktop/tablet/mobile, working department entry tabs, and search/department/GHA filters.
