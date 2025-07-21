# Assignment 4 – Python Statistics Walkthrough
### Overview
This assignment is a guided walkthrough of fundamental statistical techniques and visualization methods using Python. It is based on the Scipy Lectures: Statistics in Python, which covers key packages such as NumPy, SciPy, Pandas, Seaborn, Statsmodels, and Matplotlib. The purpose of this walkthrough is to build practical experience with statistical modeling, data transformation, and data visualization.

This repository contains:

Jupyter Notebook that follows and extends the online tutorial

Custom data wrangling example (airline fare data for 2000 and 2001)

Configuration files for reproducibility

Git best practices (including .gitignore)

 Repository Structure
vbnet
Copy
Edit

Assignment4-Stats-Scripts/

1. notebooks/
2. stats_python.ipynb      <- Jupyter notebook with step-by-step code and comments
3. .gitignore                  <- Excludes unnecessary files (e.g., checkpoints, pycache)
4. environment.yml            <- Conda environment with required dependencies
5. requirements.txt           <- Optional: alternative pip-based setup
6. README.md                  <- You're here!

Setup Instructions
Clone the repository:

bash
Copy
Edit
git clone https://github.com/Keehinde678/Assignment4-Stats-Scripts.git
cd Assignment4-Stats-Scripts
Create environment:

Using Conda:

bash
Copy
Edit
conda env create -f environment.yml
conda activate stats_env
Or using pip:

bash
Copy
Edit
pip install -r requirements.txt
Launch Jupyter Notebook:

bash
Copy
Edit
jupyter notebook
Navigate to notebooks/stats_python.ipynb to explore the analysis.

 What You'll Learn
In this notebook, I explored the following:

1. Descriptive Statistics
Mean, median, standard deviation

Percentiles

Covariance and correlation matrices

2. Visualization
Histograms

Boxplots

Scatter matrices

Seaborn regression plots (lmplot)

Heatmaps with correlation matrices

3. Inferential Statistics
Linear regression using statsmodels

Interpreting model summary output

Confidence intervals

 Custom Work – Airline Fare Dataset
In addition to the tutorial, I included a section where I worked with airline fare data for the years 2000 and 2001. I performed the following:

Flattened the hierarchical data structure using reset_index()

Selected and renamed relevant columns for both years

Created consistent column names (city1, city2, fare, nb_passengers)

Added a year column to distinguish between datasets

Concatenated the two yearly datasets into a single DataFrame

This transformation demonstrates real-world data cleaning and merging skills.

python
Copy
Edit
# Combine and label flight data for two years
data_flat = data.reset_index()

# Process 2000 data
data_2000 = data_flat[['city1', 'city2', 'pop1', 'pop2', 'dist', 'fare_2000', 'nb_passengers_2000']]
data_2000.columns = ['city1', 'city2', 'pop1', 'pop2', 'dist', 'fare', 'nb_passengers']
data_2000['year'] = 2000

# Process 2001 data
data_2001 = data_flat[['city1', 'city2', 'pop1', 'pop2', 'dist', 'fare_2001', 'nb_passengers_2001']]
data_2001.columns = ['city1', 'city2', 'pop1', 'pop2', 'dist', 'fare', 'nb_passengers']
data_2001['year'] = 2001

# Combine both
data_flat = pandas.concat([data_2000, data_2001])
 Files Included
File	Description
notebooks/stats_python.ipynb	The main notebook with code, comments, and insights
.gitignore	Prevents unnecessary files from being tracked
environment.yml	Defines the Conda environment for reproducibility
requirements.txt	Lists required packages for pip users
README.md	Assignment overview and instructions

 Packages Used
numpy

pandas

matplotlib

seaborn

statsmodels

scipy

You can update the environment file with:

bash
Copy
Edit
conda env export > environment.yml
Or for pip:

bash
Copy
Edit
pip freeze > requirements.txt
 Notes
Every section in the notebook is annotated with markdown explanations and detailed comments inside code cells.

Errors and unexpected behaviors were addressed and resolved (e.g., indexing issues and plot rendering).

The tutorial and custom work together provide a comprehensive practice on data cleaning, statistical modeling, and data visualization in Python.

 References
 Scipy Statistics Tutorial

 Pandas Documentation

 Seaborn Documentation
