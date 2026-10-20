# 🌸 Exploratory Data Analysis (EDA) on the Iris Dataset

<p align="center">
  <strong>A beginner-friendly data analysis project using Python, Pandas, Seaborn, and Matplotlib.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-Data%20Analysis-blue?logo=python" alt="Python Data Analysis" />
  <img src="https://img.shields.io/badge/Pandas-Data%20Manipulation-150458?logo=pandas" alt="Pandas" />
  <img src="https://img.shields.io/badge/Seaborn-Visualization-76B900" alt="Seaborn" />
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-orange" alt="Matplotlib" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter" alt="Jupyter Notebook" />
</p>

---

## 📌 Table of Contents

- [📖 About the Project](#-about-the-project)
- [🎯 Project Objectives](#-project-objectives)
- [📊 Dataset Overview](#-dataset-overview)
- [🛠️ Technologies and Libraries](#️-technologies-and-libraries)
- [📁 Project Structure](#-project-structure)
- [⚙️ Getting Started](#️-getting-started)
- [🔍 Analysis Workflow](#-analysis-workflow)
- [📈 Visualizations](#-visualizations)
- [🚀 Future Improvements](#-future-improvements)
- [👨‍💻 Author](#-author)

---

## 📖 About the Project

This project explores the classic **Iris flower dataset** through Exploratory Data Analysis (EDA) using Python.

The notebook demonstrates a practical data analysis workflow, starting with dataset loading and initial inspection, followed by data-quality checks, duplicate removal, descriptive statistics, and visual exploration of flower measurements.

The analysis uses **Pandas** for data manipulation and **Seaborn** and **Matplotlib** for visualization.

This project is intended to demonstrate fundamental data analysis techniques in a Jupyter Notebook.

## 🎯 Project Objectives

The main objectives are to:

- Load and inspect the Iris dataset.
- Understand the dataset's dimensions, columns, and data types.
- Check for missing values and duplicate records.
- Remove duplicate records when present.
- Generate descriptive statistics for numerical features.
- Explore relationships between flower measurements.
- Visualize distributions and feature ranges.
- Document the analysis workflow in a Jupyter Notebook.

## 📊 Dataset Overview

The notebook loads the Iris dataset using Seaborn's built-in dataset loader:

```python
iris_df = sns.load_dataset('iris')
```

The dataset initially contains **150 records and 5 columns**.

| Column | Description |
|---|---|
| `sepal_length` | Sepal length measurement |
| `sepal_width` | Sepal width measurement |
| `petal_length` | Petal length measurement |
| `petal_width` | Petal width measurement |
| `species` | Iris flower species |

The four measurement columns are numerical features, while `species` identifies the flower species.

**Dataset availability:** This project does not include a separate local CSV file. Seaborn loads the dataset through `sns.load_dataset('iris')`, so an internet connection may be needed when the dataset is not already cached.

## 🛠️ Technologies and Libraries

The project uses the following tools and Python libraries, as listed in `requirements.txt`.

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data inspection, cleaning, and descriptive statistics |
| Seaborn | Statistical data visualization and dataset loading |
| Matplotlib | Plot creation and customization |
| Jupyter | Interactive notebook environment |

## 📁 Project Structure

The project files covered by this README are organized as follows:

```text
iris-eda/
├── README.md
├── iris_eda.ipynb
└── requirements.txt
```

| File | Description |
|---|---|
| `README.md` | Project documentation and setup instructions |
| `iris_eda.ipynb` | Notebook containing the analysis, Python code, and visualizations |
| `requirements.txt` | List of required Python libraries |

## ⚙️ Getting Started

Follow these steps to run the project locally.

### 1. Clone the Repository

Replace the placeholder with your actual GitHub repository URL.

```bash
git clone <YOUR_REPOSITORY_URL>
```

Navigate to the project directory:

```bash
cd iris-eda
```

### 2. Create a Virtual Environment (Recommended)

Create an isolated Python environment:

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

On macOS or Linux:

```bash
source .venv/bin/activate
```

### 3. Install Dependencies

Install the libraries listed in `requirements.txt`:

```bash
python -m pip install -r requirements.txt
```

The dependency file contains:

```text
pandas
seaborn
matplotlib
jupyter
```

### 4. Launch Jupyter Notebook

Run:

```bash
jupyter notebook iris_eda.ipynb
```

Open the notebook in your browser and execute the cells sequentially, from top to bottom.

**Note:** A compatible Python installation is required. The dependency file does not pin specific package versions.

## 🔍 Analysis Workflow

The notebook follows these main stages.

### 1. Import Libraries and Configure Visualization

- Import Pandas, Seaborn, and Matplotlib.
- Configure Seaborn's plotting theme.
- Define a color palette for the scatter plot.

### 2. Load and Inspect the Dataset

- Load the Iris dataset into a Pandas DataFrame.
- Preview the initial records using `head()`.
- Inspect the number of records and features.
- Review column data types and non-null counts using `info()`.

### 3. Check Data Quality and Prepare the Data

- Check each column for missing values using `isnull().sum()`.
- Identify duplicate rows using `duplicated().sum()`.
- Remove duplicate records when they are present.
- Generate descriptive statistics using `describe()`.

### 4. Explore the Data Visually

Create visualizations to examine relationships between measurements, the distribution of petal length, and the spread of numerical features.

### 5. Review the Analysis

The notebook concludes by discussing the purpose of the data-quality checks and visualizations, along with possible directions for further analysis.

## 📈 Visualizations

The notebook includes three types of visualizations.

### 1. Scatter Plot: Sepal Length vs. Sepal Width

A scatter plot compares sepal length and sepal width, using flower species to distinguish data points by color.

**Purpose:** Explore the relationship between the two measurements and observe how the species appear in the plotted feature space.

### 2. Histogram: Petal Length Distribution

A histogram displays the distribution of petal length, with a Kernel Density Estimate (KDE) curve.

**Purpose:** Examine the spread and distribution patterns of petal-length measurements.

### 3. Horizontal Box Plots: Feature Ranges

Horizontal box plots display the distributions and ranges of the numerical features.

**Purpose:** Compare feature spreads and inspect potential outliers.

## 🚀 Future Improvements

The notebook identifies several possible extensions for future work:

- Add species-wise descriptive statistics.
- Create a correlation heatmap.
- Investigate potential outliers more systematically.
- Extend the exploratory analysis with additional visualizations.

These are possible improvements, not features claimed to be implemented in the current notebook.

## 👨‍💻 Author

**Ahmad Ammar**

- GitHub: [@AAmmar2005](https://github.com/AAmmar2005)

---

<p align="center">
  Built as a hands-on project to practice Python-based exploratory data analysis.
</p>
