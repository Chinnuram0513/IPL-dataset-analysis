📊 IPL Ball-by-Ball Data Cleaning & Analysis (2008–2025)
Infosys Springboard Internship — Data Analytics Project

This repository contains the full workflow for cleaning, preprocessing, and analyzing the IPL Ball-by-Ball dataset (2008–2025).
All work was performed in Google Colab using Python (Pandas, NumPy, Matplotlib, Seaborn).

The project includes:

Cleaned IPL dataset

Outlier detection

Visualizations

Player-wise & season-wise insights

Summary statistics in JSON

Fully documented cleaning notebook

📁 Repository Structure
ipl-analysis/
├── data/
│   ├── ipl_deliveries_cleaned.csv
│   ├── summary_stats.json
│   └── season_wise_runs.json
│
├── plots/
│   ├── histogram_total_runs.png
│   ├── boxplot_total_runs.png
│   ├── batsman_runs_hist.png
│   └── economy_rate_hist.png
│
├── notebooks/
│   └── ipl_cleaning_and_analysis.ipynb
│
└── README.md

🧹 Data Cleaning Steps
✔ Cleaning & Standardizing Columns

Fixed inconsistent column names

Converted datatypes (e.g., date → datetime)

Calculated missing total_runs

Removed or corrected invalid entries

✔ Handling Missing Values

Checked nulls per column

Addressed unnecessary empty fields

Ensured structural consistency

✔ Outlier Detection

Visualized using:

Boxplots

Histograms

Player run distribution

Economy rate curves

✔ Final Deliverables

Cleaned CSV

JSON summaries

Player season-wise stats

Plots folder with exported charts

📊 Generated Data & Files
📁 data/
File	Description
ipl_deliveries_cleaned.csv	Final cleaned dataset
summary_stats.json	Min, max, mean, std summary stats
season_wise_runs.json	Year-wise run totals per batsman
🖼 plots/

Includes all exported charts:

total runs histogram

total runs boxplot

batsman runs histogram

economy rate distribution

📒 Notebook

The complete cleaning + EDA code is available here:

notebooks/ipl_cleaning_and_analysis.ipynb


This notebook includes:

Data loading

Cleaning workflow

Summary creation

Visualization code

Exporting final outputs

🚀 How to Use
Load the cleaned data:
import pandas as pd
df = pd.read_csv("data/ipl_deliveries_cleaned.csv")

Load season-wise stats:
import json

with open("data/season_wise_runs.json") as f:
    season_stats = json.load(f)

🛠 Tools & Technologies Used
Tool	Purpose
Python	Data preprocessing & EDA
Pandas	Data manipulation
NumPy	Numerical operations
Matplotlib / Seaborn	Visualizations
Google Colab	Development environment
GitHub	Version control & project hosting
