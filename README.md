# Exploratory Data Analysis (EDA) on Tree Diameters Dataset

This repository presents a detailed exploratory analysis of tree growth patterns over time using climate variables and diameter observations. The dataset is stored in an Excel file and analyzed using Python libraries such as Pandas, NumPy, Seaborn, and Matplotlib.

---

## Files

- `Exploratory_Data_Analysis.ipynb` – Jupyter notebook with complete EDA process.
- `tree_diameters.xlsx` – Input dataset containing yearly tree diameter and climate data.

---

## Dataset Overview

The dataset includes the following features:

- `ID`: Unique identifier for trees
- `yr`: Year of observation
- `cm`: Diameter measurement (in centimeters)
- `annualprec`: Annual precipitation
- `summerpdsi`: Palmer Drought Severity Index for summer
- `wintertemp`: Average winter temperature
- Additional computed features: `cm_growth`, `Tree_size_category`

---

##  Key Analyses Performed

### General Exploration

- Displaying dataset shape and head
- Counting unique tree IDs and year-wise observation distribution

###  Derived Features

- Computed `cm_growth` as year-on-year percentage diameter growth for each tree
- Categorized trees into size classes:
  - Seedlings
  - Saplings
  - Poletimbers
  - Sawtimbers

### Statistical Summaries

- Central tendency: Mean vs Median comparison
- Detection of skewness in `cm` distribution
- Group-wise mean statistics using `groupby` for categories across years

### Correlation Analysis

- Generated correlation matrix using `.corr()`
- Visualized correlations using Seaborn heatmap

### Visualization

- Histogram of tree diameters
- Pair plots for all variables
- Correlation heatmaps
- Line plots and trend analysis (computed growth by category over time)

---

##  Requirements

Install the necessary libraries using:

```bash
pip install pandas numpy matplotlib seaborn plotly openpyxl
```

## How to Run
Make sure tree_diameters.xlsx is in the same directory.
Launch the notebook:
```bash
jupyter notebook Exploratory_Data_Analysis.ipynb
```