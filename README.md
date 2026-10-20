 <div align="center">

# 🌸 Iris Dataset — Exploratory Data Analysis (EDA)

### 📊 Data Cleaning • Statistical Analysis • Data Visualization

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge)](https://seaborn.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge)](https://matplotlib.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)

**A practical Python project exploring the Iris dataset through data inspection, duplicate handling, descriptive statistics, and visualization.**

</div>

---

## 📌 Table of Contents

- [🌟 About the Project](#-about-the-project)
- [🎯 Project Objectives](#-project-objectives)
- [📂 Dataset Overview](#-dataset-overview)
- [🛠️ Technologies Used](#️-technologies-used)
- [📁 Project Structure](#-project-structure)
- [🔍 Analysis Workflow](#-analysis-workflow)
- [📊 Key Findings](#-key-findings)
- [⚙️ Installation and Setup](#️-installation-and-setup)
- [🚀 Running the Notebook](#-running-the-notebook)
- [💡 Future Improvements](#-future-improvements)
- [📚 References](#-references)
- [👨‍💻 Author](#-author)

---

## 🌟 About the Project

Welcome to my **Iris Dataset Exploratory Data Analysis (EDA)** project!

Exploratory Data Analysis is an important part of the data science workflow. It helps us understand data structure, identify data-quality issues, summarize numerical measurements, and discover patterns through visualization.

In this project, I use Python and its data analysis libraries to explore the Iris dataset. The notebook covers initial data inspection, missing-value checks, duplicate detection and removal, descriptive statistics, and visualizations of flower measurements.

The project focuses on fundamental data analysis techniques and demonstrates how a structured dataset can be explored before attempting more advanced analysis.

### ✨ Project Highlights

| Feature | Description |
|---|---|
| 📥 Data Loading | Load the Iris dataset using Seaborn |
| 🔎 Data Inspection | Review dataset dimensions, columns, and data types |
| 🧹 Data Cleaning | Check missing values and remove duplicate records |
| 📈 Statistics | Generate descriptive statistics for numerical features |
| 🎨 Visualization | Create scatter plots, a histogram with KDE, and box plots |
| 📝 Documentation | Explain the project, findings, and setup process |

## 🎯 Project Objectives

The main objectives of this project are to:

- ✅ Load and inspect a dataset using Python.
- ✅ Understand its structure, dimensions, and feature types.
- ✅ Check for missing values and duplicate records.
- ✅ Remove duplicate rows when they are identified.
- ✅ Calculate descriptive statistics for numerical measurements.
- ✅ Visualize relationships between selected features.
- ✅ Explore the distributions of flower measurements.
- ✅ Practice using Pandas, Seaborn, Matplotlib, and Jupyter Notebook.

## 📂 Dataset Overview

This project uses the classic **Iris dataset**, which contains measurements of flowers belonging to three species:

- 🌼 *Iris setosa*
- 🌼 *Iris versicolor*
- 🌼 *Iris virginica*

The notebook loads the dataset directly through Seaborn:

```python
iris_df = sns.load_dataset('iris')
```

### 📋 Dataset Features

| Column | Description | Type |
|---|---|---|
| `sepal_length` | Length of the sepal | Numerical |
| `sepal_width` | Width of the sepal | Numerical |
| `petal_length` | Length of the petal | Numerical |
| `petal_width` | Width of the petal | Numerical |
| `species` | Iris flower species | Categorical |

### 📊 Dataset Summary

| Metric | Result |
|---|---:|
| Initial records | 150 |
| Total columns | 5 |
| Numerical features | 4 |
| Categorical features | 1 |
| Missing values reported | 0 |
| Duplicate rows identified | 1 |
| Records after duplicate removal | 149 |

The counts above reflect the notebook's recorded analysis.

### 🔗 Dataset Sources

- **Seaborn Example Data Repository:** [View repository](https://github.com/mwaskom/seaborn-data)
- **Iris CSV file:** [View dataset](https://github.com/mwaskom/seaborn-data/blob/master/iris.csv)
- **Original dataset reference:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/iris)

> **Note:** The notebook uses Seaborn's dataset loader rather than a separate local CSV file. An internet connection may be required if the dataset is not already cached locally.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| 🐍 [Python](https://www.python.org/) | Core programming language |
| 🐼 [Pandas](https://pandas.pydata.org/) | Data inspection and statistical summaries |
| 🎨 [Seaborn](https://seaborn.pydata.org/) | Dataset loading and statistical visualization |
| 📈 [Matplotlib](https://matplotlib.org/) | Plot creation and display |
| 📓 [Jupyter Notebook](https://jupyter.org/) | Interactive coding and analysis |

## 📁 Project Structure

The project folder contains the following files:

```text
iris-eda/
├── README.md
├── iris_eda.ipynb
├── requirements.txt
└── .gitignore
```

### 📄 File Descriptions

| File | Purpose |
|---|---|
| `README.md` | Project overview, analysis details, and setup instructions |
| `iris_eda.ipynb` | Notebook containing the Python code, analysis, and visualizations |
| `requirements.txt` | Python dependency list used for environment setup |
| `.gitignore` | Rules for excluding selected files from Git version control |

**Dataset storage:** There is no separate `data/iris.csv` file in this project structure. The notebook retrieves the dataset using Seaborn.

## 🔍 Analysis Workflow

The notebook follows a straightforward exploratory data analysis process.

### 1️⃣ Data Loading and Initial Inspection

The dataset is loaded into a Pandas DataFrame.

The notebook inspects the data by:

- Previewing the first few records.
- Checking the total number of records and features.
- Reviewing the column names and data types.
- Examining the DataFrame information.

### 2️⃣ Missing-Value and Duplicate Checks

The notebook checks the dataset for missing values and duplicate rows.

**Recorded results:**

- The initial dataset contains 150 records.
- The missing-value check reports zero missing values across the five columns.
- One duplicate row is identified.
- The duplicate row is removed before calculating the subsequent statistical summary.

### 3️⃣ Descriptive Statistical Analysis

After duplicate removal, the notebook generates a descriptive statistical summary for the numerical columns.

This provides information about:

- Count
- Mean
- Standard deviation
- Minimum and maximum values
- Quartiles and median

The resulting summary contains 149 records for each numerical feature.

### 4️⃣ 📍 Scatter Plot — Sepal Measurements

The notebook creates a scatter plot comparing **sepal length** and **sepal width**, with observations colored by species.

This visualization helps explore the relationship between the two measurements and observe how the species are distributed.

### 5️⃣ 📊 Histogram with KDE — Petal Length

A histogram with a Kernel Density Estimate (KDE) curve is used to visualize the distribution of petal length.

This plot provides an overview of the observed measurement frequencies and the overall shape of the distribution.

### 6️⃣ 📦 Box Plots — Data Spread and Potential Outliers

The notebook creates horizontal box plots for the numerical features.

These visualizations help examine measurement distributions, compare their spread, and identify observations that may warrant further investigation.

> The box plots are used for exploratory inspection. Potential outliers are not automatically evidence of incorrect data.

## 📊 Key Findings

Based on the notebook's recorded output and visualizations:

| # | Finding | Observation |
|---:|---|---|
| 1 | Dataset size | 150 initial records and 5 columns |
| 2 | Missing values | None reported by the initial check |
| 3 | Duplicate records | One duplicate row identified and removed |
| 4 | Cleaned dataset | 149 records remain after duplicate removal |
| 5 | Species visualization | *Iris setosa* appears more distinct in the sepal-measurement scatter plot |
| 6 | Feature distributions | The histogram and box plots provide a visual overview of numerical measurements |

### 🧠 What I Learned

This project provides practical experience with:

- Loading and inspecting structured data.
- Checking missing values and duplicate records.
- Cleaning a dataset before statistical analysis.
- Summarizing numerical features.
- Creating and interpreting exploratory visualizations.
- Organizing an analysis in a Jupyter Notebook.

**Project scope:** This is an exploratory data analysis project. It does not train or evaluate a machine-learning classification model.

## ⚙️ Installation and Setup

Follow these steps to run the project locally.

### 📌 Prerequisites

Make sure you have:

- Python installed on your computer.
- A terminal or command prompt.
- An internet connection if Seaborn needs to retrieve the dataset.
- The project files extracted into a folder.

### Step 1: Open the Project Folder

Download the project ZIP, extract it, and open a terminal in the extracted `iris-eda` folder.

If you have uploaded the project to GitHub, you can also clone your repository using its actual URL:

```bash
git clone <YOUR_REPOSITORY_URL>
cd iris-eda
```

Replace `<YOUR_REPOSITORY_URL>` with your real repository URL before running the command.

### Step 2: Create a Virtual Environment

A virtual environment helps isolate the dependencies for this project.

**Windows:**

```bash
python -m venv .venv
.venv\Scripts\activate
```

**macOS / Linux:**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### Step 3: Install Dependencies

Use the project's existing `requirements.txt` file:

```bash
python -m pip install -r requirements.txt
```

This installs the packages listed in that file. Ensure the dependency list matches the libraries required by the notebook.

## 🚀 Running the Notebook

Once the environment is ready, launch the notebook:

```bash
jupyter notebook iris_eda.ipynb
```

Then:

1. 🌐 Open the notebook in your browser.
2. 📂 Select `iris_eda.ipynb` if it does not open automatically.
3. ▶️ Run the cells in order.
4. 📊 Review the outputs, statistical summaries, and plots.

**Important:** If the notebook cannot retrieve the Iris dataset, check your internet connection and Seaborn installation.

## 💡 Future Improvements

The following improvements could extend the current project:

- 📊 **Species-wise statistics:** Compare numerical measurements across the three Iris species.
- 🔥 **Correlation heatmap:** Visualize relationships between numerical features.
- 🔎 **Outlier investigation:** Examine potential outliers using a documented statistical method.
- 🧪 **Data validation:** Add checks for expected columns, data types, and row counts.
- 🖼️ **Plot exports:** Save selected visualizations in an `images/` directory.
- 📝 **Expanded analysis:** Add further observations supported by additional analysis.

These are suggestions for future development, not features claimed to be implemented in the current notebook.

## 🤝 Feedback and Contributions

Feedback and suggestions that improve the project's documentation, analysis, or visualizations are welcome.

If you notice an issue or have an idea for an improvement, you can use the repository's GitHub Issues feature when it is available.

When proposing changes, please keep the project focused on exploratory data analysis and document any meaningful modifications.

## 📚 References

- 🌐 [Seaborn Example Data Repository](https://github.com/mwaskom/seaborn-data)
- 📄 [Iris Dataset CSV](https://github.com/mwaskom/seaborn-data/blob/master/iris.csv)
- 🏛️ [UCI Machine Learning Repository — Iris Dataset](https://archive.ics.uci.edu/ml/datasets/iris)
- 🐼 [Pandas Documentation](https://pandas.pydata.org/docs/)
- 🎨 [Seaborn Documentation](https://seaborn.pydata.org/)
- 📈 [Matplotlib Documentation](https://matplotlib.org/stable/)
- 📓 [Jupyter Documentation](https://docs.jupyter.org/)

## 👨‍💻 Author

**Ahmad Ammar**

Computer Science student interested in Python, data science, and artificial intelligence.

🔗 **GitHub:** [AAmmar2005](https://github.com/AAmmar2005)

---

<div align="center">

### 🌱 Learning Through Data

*An educational project exploring the fundamentals of Python-based data analysis.*

⭐ If you find this project useful, consider starring the repository.

</div>
