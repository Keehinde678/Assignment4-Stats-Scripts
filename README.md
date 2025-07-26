# Statistics in Python

# Overview
Welcome to this Statistics in Python project!
Here, we explore foundational and advanced statistical techniques using real-world datasets such as the Iris and Brain Size datasets. This project is designed to guide you through data representation, hypothesis testing, regression modeling, and powerful visualization methods — all within Python’s robust scientific ecosystem.

Whether you are a student, researcher, or data enthusiast, this project equips you with practical skills and clear examples to master statistical analysis in Python.

# Project Objectives
Learn how to represent and manipulate data effectively using pandas DataFrames.

Understand and apply hypothesis testing methods including Student’s t-tests and paired tests.

Build and interpret linear regression models with multiple predictors and interaction terms using statsmodels.

Perform Analysis of Variance (ANOVA) and post-hoc hypothesis tests to analyze group effects.

Create meaningful, insightful visualizations using Seaborn, including pairplots and regression plots.

Develop reproducible, clean Python code for statistical modeling and plotting.

# Datasets Used
Iris Dataset: Classic dataset for exploring flower species classification based on sepal and petal measurements.

Brain Size Dataset: Contains IQ scores, body measurements, and demographic data, ideal for studying cognitive and physical variable relationships.

# Key Topics Covered
1. Data Representation and Interaction
Explore how to structure and interact with data, focusing on tabular formats.

2. Data as a Table & pandas DataFrame
Learn why dataframes are powerful tools for organizing, filtering, and manipulating data in Python.

3. Hypothesis Testing: Comparing Two Groups
Understand basic statistical testing principles and compare groups with confidence.

4. Student’s t-test and Paired Tests
Apply fundamental tests for both independent and repeated measurements.

5. Linear Models and Multiple Factors
Model relationships using regression, including multiple explanatory variables and interaction effects.

6. Statistical Formulas in Python
Use intuitive formula syntax to specify complex statistical models easily.

7. Analysis of Variance (ANOVA) & Post-hoc Testing
Analyze differences across multiple groups and conduct follow-up comparisons.

8. Advanced Visualization with Seaborn
Utilize Seaborn’s powerful visualization capabilities to uncover patterns and insights:

Pairplot: Visualize scatter matrices for variable relationships.

lmplot: Create univariate regression plots with confidence intervals.

9. Testing for Interactions
Detect and interpret how variables jointly affect outcomes.

10. Full Code and Exercises
Access complete code for all visualizations and statistical tests, plus detailed solutions to practice exercises for self-assessment.

Installation
To run this project locally, you need Python and several packages installed. The recommended way is to use the provided requirements.txt:

bash
Copy
Edit
pip install -r requirements.txt
Required packages include:

numpy

scipy

matplotlib

pandas

statsmodels

seaborn

We recommend using the Anaconda distribution for a hassle-free installation.

Usage
Clone this repository:

bash
Copy
Edit
git clone https://github.com/yourusername/statistics-python-project.git
cd statistics-python-project
Place your datasets (iris.csv and brain_size.csv) into the data/ folder.

Run the analysis scripts:

For Iris dataset analysis:

bash
Copy
Edit
python analyze_iris.py
For Brain Size dataset analysis:

bash
Copy
Edit
python analyze_brain_size.py
Explore output plots and regression summaries for insights.

Example Code Snippet: Linear Regression on Brain Size Dataset
python
Copy
Edit
import pandas as pd
from statsmodels.formula.api import ols

# Load data
brain = pd.read_csv('data/brain_size.csv', sep=';', na_values='.')

# Fit model with interaction between height and gender
model = ols('FSIQ ~ Height * Gender', data=brain).fit()

# Print results
print(model.summary())
Contributing
Contributions are highly welcome! Feel free to:

Report bugs or suggest features via GitHub issues

Submit pull requests to improve code, documentation, or add datasets

License
This project is open-source under the MIT License.

Contact
If you have questions, ideas, or want to collaborate, reach out:

Name: Kehinde Soetan

Email: soetan.6@osu.edu

GitHub: Keehinde678

