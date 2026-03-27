# FTICRMS Molecular Visualization
**Author:** Nitish Kapur

A Python tool to plot and visualize FTICR-MS molecular data from Excel files. Generates multiple scatter and bar plots. Also compiles the graphs into PDF and DOCX files.

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
   
