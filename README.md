
# 🎬 Movie Dataset Analysis with Python

This project performs an in-depth data analysis of a movie dataset using Python. It includes cleaning raw data, converting types, handling missing values, deriving new features (like release year), and visualizing key trends. The goal is to identify insights about movie budgets, revenues, and top-performing production companies.

---

## 📁 Project Structure

```
.
├── Movies_Data_Analysis.ipynb   # Jupyter Notebook with full EDA and visualization
├── movies.csv                   # Raw movie metadata CSV file
└── README.md                    # Project documentation
```

---

## 📌 Key Objectives

- ✅ Load and inspect raw movie data
- ✅ Handle and remove missing values
- ✅ Convert columns (e.g., budget, gross, votes) to numeric
- ✅ Extract year from the release date
- ✅ Analyze correlations between numeric fields
- ✅ Identify top movie companies by average gross and budget
- ✅ Visualize insights with clear and styled plots

---

## 🧪 Libraries Used

- **pandas** – for data wrangling
- **matplotlib** – for visualizations
- **seaborn** – for statistical plots
- **Jupyter Notebook** – for step-by-step documentation and execution

---

## 📂 Dataset Overview

The dataset (`movies.csv`) contains the following features:

- `name`: Title of the movie
- `genre`, `director`, `writer`, `star`: Metadata on creators
- `budget`: Production budget in USD
- `gross`: Gross earnings in USD
- `votes`: IMDb votes
- `runtime`: Runtime in minutes
- `rating`: IMDb rating
- `released`: Release date (string)
- `company`: Production studio

---

## 🔍 Analysis Steps

### 🧹 1. Data Cleaning
- Dropped rows with null values using `dropna()`
- Converted `budget`, `gross`, `votes`, and `runtime` to `int64`
- Extracted year from the `released` column using regular expressions

### 📊 2. Exploratory Data Analysis
- **Scatter Plot** of Budget vs Gross earnings
- **Regression Plot** to visualize budget-gross correlation
- **Correlation Heatmap** for all numeric features (Pearson)
- **Bar Plots** for:
  - Top 10 companies by average gross revenue
  - Top 10 companies by average budget
  - Top 8 companies with highest grossing or budget-heavy films

### 📈 3. Insights Extracted
- Strong positive correlation between movie budget and gross revenue
- Some companies consistently invest in high-budget films
- Votes and ratings show moderate correlation with earnings

---

## 🖼️ Sample Visuals

- `Budget vs Gross` Scatter and Regression Plot  
- `Correlation Heatmap`  
- `Bar charts` of top companies by revenue and budget

---

## 🚀 How to Run the Project

1. Install dependencies:

```bash
pip install pandas matplotlib seaborn
```

2. Launch the notebook:

```bash
jupyter notebook Movies_Data_Analysis.ipynb
```

3. Run all cells to reproduce the visualizations and analysis

---

## 👩‍💻 Contributor
- [Azim Nahin](https://github.com/AzimNahin)
