# Assignment4-Stats-Scripts

## Overview

Welcome to the Assignment4-Stats-Scripts repository! This project is designed to explore fundamental statistical concepts and data visualization techniques using Python. We work with datasets, perform hypothesis testing, regression analyses, and create insightful visualizations to understand complex relationships in data.

The main focus is on developing reproducible, well-documented scripts and notebooks that enhance your data analysis skills while providing a strong foundation in applied statistics.

Repository Contents
Notebooks: contains Jupyter Notebooks that guide you step-by-step through the statistical analyses and visualizations.

stats_python.ipynb: main notebook with detailed code examples, comments, and markdown explanations.

environment.yml / requirements.txt
These files specify the software dependencies and packages required to run the analyses in a reproducible environment.

.gitignore
Specifies files and folders (like temporary files, checkpoints) to be excluded from version control.

README.md
This document that outlines the project, setup instructions, and usage.

## Setup on Ascend Desktop
Ascend Desktop supports Python and Jupyter notebooks but may not have Conda installed by default. Here are instructions to get your environment ready:

Using pip (recommended for Ascend Desktop)
Create and activate a Python virtual environment (optional but recommended):

python3 -m venv assignment4-env
source assignment4-env/bin/activate   # On Windows: assignment4-env\Scripts\activate
Install required packages with pip:

pip install -r requirements.txt
Using Conda (if available)
If Conda is installed or can be installed on Ascend Desktop, use:

conda env create -f environment.yml
conda activate assignment4-env

## Key features
Load datasets

Explore data structure and variables

Perform statistical tests such as t-tests and regression analyses

Visualize data through scatter plots, box plots, and regression plots

Understand interaction effects in regression models

Save your progress and commit your changes regularly for version control.

Key Features and Highlights
Data Loading & Cleaning: Demonstrates how to load CSV files, handle missing values, and inspect data shapes and types.

Statistical Testing: Includes examples of one-sample, independent, and paired t-tests using scipy.stats.

Regression Modeling: Covers linear regression, multiple regression, and testing interaction terms with statsmodels.

Data Visualization: Uses matplotlib and seaborn to create insightful visualizations like scatter matrices, boxplots, regression plots, and pairplots.

Reproducibility: Environment files ensure consistent package versions across setups.

Detailed Documentation: Code cells have comprehensive comments and markdown cells explain the rationale behind each step.

Folder Structure

Assignment4-Stats-Scripts/

├── notebooks/
│   └── stats_python.ipynb      # Main notebook with detailed examples
│
├── environment.yml             # Conda environment specification file
├── requirements.txt           # Pip requirements file (alternative)
├── .gitignore                 # Git ignore rules
└── README.md                  # This README file
