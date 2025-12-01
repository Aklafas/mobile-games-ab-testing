# 📱 Mobile Games A/B Testing: Cookie Cats

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Library-Pandas%20|%20Scipy%20|%20Seaborn-orange)
![Status](https://img.shields.io/badge/Status-Completed-green)

## 📌 Project Overview
**Cookie Cats** is a popular mobile puzzle game. This project analyzes the results of an A/B test where the first gate in the game was moved from level 30 to level 40.

**Goal:** Determine if moving the gate affects player retention (1-day and 7-day).

## 📊 Data & Methods
The dataset contains **90,189 players**.
Key steps taken:
1.  **Data Cleaning:** Removing outliers (players with impossible number of rounds).
2.  **EDA:** Analyzing distribution of game rounds and retention rates.
3.  **Statistical Analysis:** Using **Bootstrap Analysis** (non-parametric method) to assess the statistical significance of the difference between groups.

## 📈 Key Findings
- **Retention 1-day:** No significant difference between groups.
- **Retention 7-day:** The control group (Gate at level 30) showed **higher retention** compared to the test group (Gate at level 40).
- **Probability:** There is a **99.8% probability** that retention is higher when the gate is at level 30.

## 💡 Recommendation
**Do not move the gate to level 40.**
Keeping the gate at level 30 results in better long-term player engagement. This can be explained by the "hedonic adaptation" theory — forcing a break earlier keeps players more eager to return.

## 🛠️ Tech Stack
- **Python** (Pandas, NumPy)
- **Stats** (SciPy, Bootstrapping)
- **Visualization** (Matplotlib, Seaborn)

## 🚀 How to Run
1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
3. Open AB_Test_Cookie_Cats.ipynb in Jupyter Notebook.
