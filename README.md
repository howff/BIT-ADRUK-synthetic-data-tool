# BIT and ADR UK Synthetic Data Tool

This tool was developed as a component of the [*Accelerating public policy research with synthetic data* report](https://www.adruk.org/fileadmin/uploads/adruk/Documents/Accelerating_public_policy_research_with_synthetic_data_December_2021.pdf) written by [BIT for ADR UK](https://www.adruk.org/news-publications/news-blogs/report-investigates-how-synthetic-data-can-be-used-in-government/).

It consists of a Jupyter notebook that will generate low fidelity synthetic data from a single flat file table.  Low fidelity synthetic data preserves the format of the data and attempts to reproduce the distributions of values *within* individual columns but not between them.  This means that it is very unlikely to reproduce individual records from the original data set.  More information can be found in the User Guide.

**Caution:** If this tool is being used to generate synthetic data from a source containing personal or other sensitive information, the synthetic data output should still be subject to a disclosure control process before release. This is because misconfiguration of the tool, random chance, and the nature of the original data can occasionally lead to disclosive information still being present in the synthetic output (see 'Why is disclosure control still needed' in the User Guide).  Proceed with care.

## Prerequisites

This notebook requires that the following are installed:
- A version of Python, ideally Python3.
- Software for viewing, editing and running `.ipynb` files, such as VSCode or Jupyter.
- The following libraries:
    - numpy
    - pandas
    - pyreadstat (optional: this is needed only if you have Python 3 and want to read/preserve metadata from .sav files)

Further discussion may be found in the 'Troubleshooting' section of the [*User Guide*] (https://www.adruk.org/fileadmin/uploads/adruk/Documents/User-Guide-Synthetic-Data-Tool.pdf).


