# datafun-07-applied

In this module, I am creating a guided project without a strict specification. Throughout the module, I will explore topics such as machine learning. The project will also involve using Jupyter for analysis and visualization.

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