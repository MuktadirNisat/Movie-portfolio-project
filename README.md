# 🎬 Movie Industry Correlation Analysis in Python

## 📌 Project Overview
This project explores Kaggle's **Movie Industry Dataset** (`movies.csv`) to identify which factors have the strongest statistical correlation with a film's **gross box office revenue**. Built in Python using VS Code and Jupyter Notebook, the workflow covers data cleaning, type standardization, categorical encoding, regression plotting, and correlation matrix heatmaps.

---

## 🎯 Hypotheses & Objectives
1. **Production Budget Hypothesis:** Higher production budgets (`budget`) strongly correlate with higher box office earnings (`gross`).
2. **Production Company Hypothesis:** Major production studios (`company`) show a strong positive correlation with gross revenue.

---

## 🧹 Data Cleaning & Analysis Workflow
- **Missing Value Handling:** Removed incomplete rows (`dropna()`) to ensure accurate type casting and correlation calculations.
- **Data Type Formatting:** Converted `budget` and `gross` columns from `float64` to `int64`.
- **Year Standardization:** Extracted the accurate 4-digit release year from the `released` column into `yearcorrect`.
- **Visualizations:** Created Matplotlib scatter plots and Seaborn regression plots (`sns.regplot`) for `budget` vs. `gross`, alongside Pearson correlation heatmaps.
- **Categorical Encoding:** Converted non-numeric columns (`company`, `country`, `director`, `genre`, etc.) into numeric category codes (`.astype('category').cat.codes`) to evaluate correlations across all 15 features.

---

## 💡 Key Findings
- **Budget & Gross Revenue (`r = 0.71`):** Strong positive correlation—films with higher production budgets generate significantly higher box office returns.
- **Audience Votes & Gross Revenue (`r = 0.66`):** User engagement (`votes`) also shows a strong positive correlation with gross earnings.
- **Company Impact:** Contrary to the initial hypothesis, the production `company` alone has a very low correlation with gross earnings.

---

## 🛠️ Tech Stack
- **Language:** Python 3.x
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Environment:** VS Code & Jupyter Notebook (`.venv`)

---

## 🚀 How to Run Locally
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/MuktadirNisat/Movie-portfolio-project.git](https://github.com/MuktadirNisat/Movie-portfolio-project.git)
   cd Movie-portfolio-project