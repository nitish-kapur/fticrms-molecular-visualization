# FTICR-MS Molecular Visualization

A Python tool to generate molecular plots from FTICR-MS data stored in Excel files. It produces 15 types of visualizations per intensity column, including Aromaticity Index, H/C, O/C, DBE, Kendrick Mass Defect, and normalized intensity graphs. Output is saved as PNG, PDF, and DOCX.

## Author

**Nitish Kapur**  
GitHub: [github.com/nitish-kapur](https://github.com/nitish-kapur)

## Project Overview

This repository contains a Python script, `fticrms_molecular_visualization.py`, designed for visualizing FTICR-MS molecular data. It reads Excel files with specific columns and automatically generates comprehensive plots for chemical analysis, including Kendrick Mass Defect calculations and class-based color coding. The tool is suitable for chemists, material scientists, and anyone working with high-resolution mass spectrometry data.

## Expected Input Format

The script expects an `.xls` or `.xlsx` Excel file. Each sheet in the workbook represents one sample, corresponding to a different FTICR-MS ionisation mode (e.g. ESI+, ESI−, APPI+, APPI−, etc.). The snippet can be used as a blueprint for structuring the data in the excel file:

| Calc m/z | #C | #H | #O | #N | #Na | O/C | H/C | N/C | DBE | AI | N-BO-1 | N-BO-2 | N-BO-3 | ... |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 109.026001 | 4 | 6 | 2 | 0 | 1 | 0.5 | 1.5 | 0 | 2 | 0.333 | ... | ... | ... | ... |
| 109.076025 | 6 | 8 | 0 | 2 | 0 | 0 | 1.333 | 0.333 | 4 | 0.6 | ... | ... | ... | ... |
| 110.06004 | 6 | 7 | 1 | 1 | 0 | 0.167 | 1.167 | 0.167 | 4 | 0.6 | ... | ... | ... | ... |
| ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |

> **Note:** The script requires the following columns to be present: `#C`, `#H`, `#O`, `#N`, `Calc m/z`, `AI`, `H/C`, `O/C`, `N/C`, and `DBE`. Columns prefixed with `N-BO` are used as intensity values for scatter plot sizing. Any sheet missing these columns will raise an error.
> 
## Features

- Generates 15 types of plots per data column (AI vs #C, H/C vs DBE, DBE vs KMD, etc.)
- Supports plotting by intensity or user-defined columns
- Adds color mapping and class-based coloring
- Produces a combined PDF and DOCX report
- Automatically organizes output in timestamped folders

## Requirements

- Python 3.x
- Pandas
- Matplotlib
- python-docx

Install dependencies via pip:

```bash
pip install pandas matplotlib python-docx

## Usage

1. Run the Python script:
  ```bash
   python fticrms-molecular-visualization.py
2. Select the excel file.
3. Select the output folder where the files are to be saved. 
   
