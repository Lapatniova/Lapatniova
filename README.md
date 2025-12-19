# Hello! 👋

I am **Alena Lapatniova**, Assistant Engineer at Progedo (CNRS).  
I work on the documentation of statistical surveys and historical data using the **DDI** standard, and I develop **R scripts** to automate this process.  
I am passionate about sailing and enjoy hiking.

---

## Badges  
[![ORCID](https://img.shields.io/badge/ORCID-0000--0001--8485--2371-green)](https://orcid.org/0000-0001-8485-2371)  
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17752420.svg)](https://doi.org/10.5281/zenodo.17752420)

This repository is archived and citable via Zenodo (DOI above).

---

## Skills  
- R, data processing and automation  
- DDI (Data Documentation Initiative) documentation  
- Management of historical data and statistical surveys  
- Passion for sailing and hiking

---

## Project: `inject_categories`  

`inject_categories` is an R script that allows users to inject variable categories from an Excel file into an existing XML file.  
It is designed for easy updating of questionnaires or datasets in XML format.

### Usage Example
```r
inject_categories(
  xml_path = "data/input.xml",
  excel_path = "data/categories.xlsx",
  output_xml_path = "data/output.xml"
)
``` 

---
## Project : `insert_universe`

insert_universe is an R script that automates the insertion of DDI <universe> metadata at the variable level in a DDI XML file exported from Nesstar or NADA.
It is designed to avoid manually filling the Universe / Filter field by using an Excel mapping file.

---
### Usage Example
```r
insert_universe(
  xml_path = "data/input.xml",
  excel_path = "data/universe_mapping.xlsx",
  output_xml_path = "data/output_universe.xml"
)

---

The Excel file must contain two columns:
variable → variable name (must match the XML)
universe → universe or filter text to insert

The script creates a <universe> tag if it does not exist, or updates it if it does.


Thanks for visiting my GitHub profile! 🚀



