# 🌍 Countries Economic Analysis

This project analyzes worldwide economic indicators to uncover how GDP, inflation, unemployment, debt, and other macroeconomic variables interact across regions.  
The data was analyzed in **Python (pandas, seaborn, scikit-learn)** and visualized through regression, clustering, and exploratory techniques.

---

## 📁 Dataset Overview

-  **Source:** Public dataset of world economic and geographic indicators (compiled from open sources).
-  **Rows:** 173 countries
-  **Columns:** 19 variables including:
   -  `name` — country name
   -  `currency` — main currency
   -  `capital` — capital city
   -  `languages` — official or main languages
   -  `latitude`, `longitude` — geographic coordinates
   -  `area` — land area (sq. km)
   -  `region`, `subregion` — geographic classification
   -  `borders` — neighboring countries (if any)
   -  `GDP` — gross domestic product per capita (USD)
   -  `GDP Growth` — annual GDP growth rate (%)
   -  `Interest Rate` — central bank interest rate (%)
   -  `Inflation Rate` — annual inflation (%)
   -  `Jobless Rate` — unemployment rate (%)
   -  `Gov. Budget` — government budget balance (% of GDP)
   -  `Debt/GDP` — public debt as % of GDP
   -  `Current Account` — current account balance (% of GDP)
   -  `Population` — total population

Some columns contain missing values, particularly `GDP Growth`, `Interest Rate`, and `borders`. These were handled or noted where relevant in the analysis.

---

## 🧹 Data Preparation (Python Notebook)

Performed using **pandas**:

1. Inspected structure and null values.
2. Renamed columns for readability and ensured numeric types.
3. Created derived fields such as land vs island (`borders` null check).
4. Standardized quantitative variables for clustering analysis.
5. Removed or imputed missing values when appropriate.

📓 _See full process and explanations in `Countries_Analysis.ipynb`._

---

## 📊 Key Insights

-  Wealthier countries tend to have **lower inflation and unemployment**, though the correlation is weak.
-  Larger countries generally have **larger populations**, but the relationship is **sublinear** — population increases slower than area.
-  **Land countries** show higher median GDP than islands, likely benefiting from connectivity and trade.
-  **Clustering analysis** reveals four main groups:  
   **GDP Titans**, **Inflationary countries**, **Low-development countries**, and **Average countries** — each with distinct economic profiles.

---

## 🧠 Tools & Skills Demonstrated

| Category                 | Tools / Libraries                                 |
| ------------------------ | ------------------------------------------------- |
| Data Cleaning & Analysis | pandas, numpy                                     |
| Visualization            | seaborn, matplotlib, plotly                       |
| Machine Learning         | scikit-learn (KMeans, Linear Regression, scaling) |
| Data Storytelling        | Markdown, Tableau (planned)                       |

---

## 🖼️ Interactive Dashboard (coming soon)

An interactive Tableau dashboard will be available here once published:  
👉 [View on Tableau Public](https://public.tableau.com/app/profile/lucio.colombo/viz/CountriesEconomydatadashboard/Dashboard1)

---

## 🚀 How to Reproduce

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/countries-analysis.git
   ```
