<div align="center">

# 📚 Books Data Analysis

### Exploratory Data Analysis of Book Sales, Ratings, Authors & Publishers

<p>
  <img src="https://img.shields.io/badge/status-completed-brightgreen?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/type-EDA-blue?style=for-the-badge" alt="Type">
  <img src="https://img.shields.io/badge/license-MIT-yellow?style=for-the-badge" alt="License">
</p>

<p>
  <a href="https://www.python.org/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python" width="55" height="55"/></a>&nbsp;&nbsp;
  <a href="https://pandas.pydata.org/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" alt="Pandas" width="55" height="55"/></a>&nbsp;&nbsp;
  <a href="https://numpy.org/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" alt="NumPy" width="55" height="55"/></a>&nbsp;&nbsp;
  <a href="https://matplotlib.org/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/matplotlib/matplotlib-original.svg" alt="Matplotlib" width="55" height="55"/></a>&nbsp;&nbsp;
  <a href="https://seaborn.pydata.org/"><img src="https://seaborn.pydata.org/_images/logo-mark-lightbg.svg" alt="Seaborn" width="55" height="55"/></a>&nbsp;&nbsp;
  <a href="https://jupyter.org/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jupyter/jupyter-original-wordmark.svg" alt="Jupyter" width="55" height="55"/></a>&nbsp;&nbsp;
  <a href="https://git-scm.com/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="Git" width="55" height="55"/></a>&nbsp;&nbsp;
  <a href="https://github.com/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" width="55" height="55"/></a>
</p>

</div>

---

## 📖 Overview

This project explores a dataset of **1,070 books** to uncover patterns in **publishing trends, genres, author ratings, languages, sales and publisher revenue**. Using Python's data science stack, the notebook cleans the data, answers key business questions and visualizes the results.

## 🎯 Objectives

- 🧹 Clean and prepare the dataset for analysis
- 📈 Understand publishing trends across the years
- 🏷️ Compare genres by popularity and reader engagement
- ✍️ Identify top authors by rating and gross sales
- 💰 Analyze the relationship between price and units sold
- 🏢 Evaluate publisher revenue and language distribution

## 🗂️ Dataset

**File:** `Books_Data_Clean.csv` &nbsp;|&nbsp; **Rows:** 1,070 &nbsp;|&nbsp; **Columns:** 15

| Column | Description |
|---|---|
| `Publishing Year` | Year the book was published |
| `Book Name` | Title of the book |
| `Author` | Author(s) of the book |
| `language_code` | Language of the book |
| `Author_Rating` | Author category (e.g. Novice, Intermediate) |
| `Book_average_rating` | Average reader rating |
| `Book_ratings_count` | Number of ratings received |
| `genre` | Book genre |
| `gross sales` | Total gross sales |
| `publisher revenue` | Revenue earned by the publisher |
| `sale price` | Price the book was sold at |
| `sales rank` | Sales ranking |
| `Publisher` | Publishing company |
| `units sold` | Number of units sold |

## 🔍 Analysis Workflow

1. **Load data** with Pandas
2. **Inspect** structure using `info()`, `head()`, `describe()`
3. **Clean** invalid records (filtered `Publishing Year > 1900`) and check for missing values
4. **Explore** unique values and group-level statistics
5. **Visualize** trends and distributions with Matplotlib & Seaborn

## 📊 Key Visualizations & Insights

### 📈 Total Units Sold Over the Years
<p align="center">
  <img src="units_sold_over_years.png" alt="Total units sold over the years" width="600">
</p>

> Sales stay low for most of the 20th century, start growing from the 1980s and **peak around 2012 (~770K units)**. The drop after 2012 is likely due to fewer records in the dataset for the latest years.

---

### 📦 Units Sold by Author Rating
<p align="center">
  <img src="units_sold_by_author_rating.png" alt="Box plot of units sold by author rating" width="600">
</p>

> **"Excellent" authors have by far the widest spread**, with the top quarter of their books selling around 30K+ units. Intermediate authors show many high-selling outliers, while most books in every group sell fewer than ~6K units.

---

### 💰 Sale Price vs Units Sold
<p align="center">
  <img src="price_vs_units_sold.png" alt="Scatter plot of sale price vs units sold" width="600">
</p>

> **Price alone doesn't explain sales.** Books split into two clear groups: low sellers (under ~7K units) and bestsellers (28K to 61K units), and both groups exist at almost every price point. Very expensive books (above $15) rarely sell many units.

---

### 🗒️ All Charts in the Notebook

| Chart | What it shows |
|---|---|
| 📊 Histogram | Distribution of publishing years |
| 📊 Bar chart | Number of books per genre |
| 📦 Box plot | Ratings count by genre |
| 🔵 Scatter plot | Sale price vs. units sold |
| 🥧 Pie chart | Language distribution of books |
| 🔵 Scatter plot | Average rating vs. ratings count |
| 📊 Bar chart | Top 20 authors by total gross sales |
| 📦 Box plot | Units sold by author rating |
| 📈 Line chart | Total units sold over the years |

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) | Core programming language |
| ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) | Data loading, cleaning & aggregation |
| ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square&logo=plotly&logoColor=white) | Basic plotting |
| ![Seaborn](https://img.shields.io/badge/Seaborn-4C9BBF?style=flat-square&logo=python&logoColor=white) | Statistical visualization |
| ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white) | Interactive notebook environment |

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
```

### 2. Install dependencies

```bash
pip install pandas matplotlib seaborn jupyter
```

### 3. Launch the notebook

```bash
jupyter notebook Notebook.ipynb
```

> 💡 Make sure `Books_Data_Clean.csv` is in the same folder as the notebook.

## 📁 Project Structure

```
📦 books-data-analysis
 ┣ 📓 Notebook.ipynb
 ┣ 📄 Books_Data_Clean.csv
 ┣ 🖼️ images/
 ┗ 📄 README.md
```

## 🔮 Future Improvements

- Add a correlation heatmap for numeric features
- Build a predictive model for `units sold`
- Create an interactive dashboard (Plotly / Streamlit)
- Clean multi-author and language-code inconsistencies

## 🤝 Contributing

Contributions, issues and feature requests are welcome! Feel free to open an issue or submit a pull request.

## 📬 Contact

**Your Name** &nbsp;·&nbsp; [GitHub](https://github.com/Abdullahstack24) &nbsp;·&nbsp; [LinkedIn](https://linkedin.com/in/abdullah-mehmood-/) 

---

<div align="center">

⭐ If you found this project useful, please give it a star! ⭐

</div>
