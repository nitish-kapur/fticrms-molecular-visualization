# FTICR-MS Molecular Visualization

A Python tool to generate molecular plots from FTICR-MS data stored in Excel files. It produces 15 types of visualizations per intensity column, including Aromaticity Index, H/C, O/C, DBE, Kendrick Mass Defect, and normalized intensity graphs. Output is saved as PNG, PDF, and DOCX.

## Project Overview

This repository contains a Python script, `fticrms_molecular_visualization.py`, designed for visualizing FTICR-MS molecular data. It reads Excel files with specific columns and automatically generates comprehensive plots for chemical analysis, including Kendrick Mass Defect calculations and class-based color coding. The tool is suitable for chemists, material scientists, and anyone working with high-resolution mass spectrometry data.

## Author

**Nitish Kapur**  
GitHub: [github.com/nitish-kapur](https://github.com/nitish-kapur)

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
   
