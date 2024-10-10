# datafun-07-applied

In this module, I created a guided project to explore machine learning concepts, without a strict specification. The project involved using Jupyter Notebook for analysis and visualization, focusing on topics like simple linear regression, multiple linear regression, and exploratory data analysis (EDA) using real-world datasets such as NYC January temperatures and the California Housing dataset.

## Project Overview

### Part 1 - Chart a Straight Line

In this part, we used Python to create a conversion chart between Fahrenheit and Celsius. We generated temperature values, converted them using the formula C = (F - 32) × 5/9, and visualized the data using a line plot.

### Part 2 - Predicting Average High Temperature in NYC

We used historical data of average high temperatures in NYC during January to predict future temperatures using linear regression. This part involved:

- Data Acquisition: Loading the dataset from a CSV file.

- Data Cleaning: Renaming columns and extracting the year from the date.

- Building the Model: Using SciPy's linregress to calculate the slope and intercept for the best-fit line.

- Prediction and Visualization: Predicting the temperature for 2024 and visualizing the trend using Seaborn.

### Part 3 - Prediction with Scikit-Learn

We applied the Scikit-Learn library to build a linear regression model for predicting NYC temperatures. The steps included:

- Data Splitting: Splitting the dataset into training and testing sets.

- Model Training: Using LinearRegression to fit the model.

- Model Testing and Prediction: Evaluating the model using R² score and predicting the temperature for 2024.

### Part 4 - Insights

We compared the two approaches used in Parts 2 and 3:

- SciPy Linear Regression: Quick and straightforward, but lacks model validation.

- Scikit-Learn Linear Regression: More robust due to training/testing split and model evaluation using R² score.

### Part 5 - Bonus: California Housing Dataset

We explored the California Housing dataset to practice multiple linear regression:

- Data Loading and Exploration: Loaded the dataset using fetch_california_housing() and explored it with Pandas.

- Data Visualization: Created scatter plots to visualize the relationships between features and the target variable.

- Model Training and Testing: Built a linear regression model and evaluated its performance.

- Model Comparison: Compared different models (LinearRegression, ElasticNet, Lasso, Ridge) using cross-validation to determine the best fit.

## Installation and Setup

### Create a GitHub Repository

Create a new repository on GitHub, including a README file.
Clone the repository to your local machine

```bash
git clone https://github.com/bware7/datafun-07-applied.git
```

### Add a .gitignore File

Ensure the following entries are added to your .gitignore file to exclude unnecessary files from being committed:

```bash
# Python virtual environment
.venv/

# Visual Studio Code settings and workspace
.vscode/

# Compiled Python files
__pycache__/

# Jupyter notebook checkpoints
.ipynb_checkpoints/
```

### Create and Activate a Virtual Environment

Create a virtual environment:

```bash
python -m venv .venv
```

Activate the virtual environment:

```bash
.\.venv\Scripts\activate
```

### Install Dependencies

Add requirements.txt file, it will be used to install with the necessary libraries.

Add the following libraries to your requirements.txt file:

```bash
jupyterlab
numpy
pandas
pyarrow
matplotlib
seaborn
scipy
sklearn
```

Install into your active project virtual environment with this command:

```bash
py -m pip install -r requirements.txt
```

### Stage and Push Files to GitHub

Use the following Git commands to stage and commit changes:

```bash
git add .
git commit -m "initial commit"
git push origin main
```

## Running the Project

Open the project folder in VS Code, activate the virtual environment, and run JupyterLab to start exploring the project notebooks:

```bash
jupyter lab
```

## Summary

This project provided hands-on experience with machine learning concepts, specifically linear regression. We used different Python libraries, including Pandas, SciPy, and Scikit-Learn, to analyze and predict data trends. Additionally, we explored multiple regression techniques with the California Housing dataset, gaining insights into the importance of model validation and comparison.