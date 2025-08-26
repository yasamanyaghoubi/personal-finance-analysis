# personal-finance-analysis
data cleaning ,EDA and analysis of personal daily costs dataset (self-collected)


📊 Personal Daily Costs Analysis


📌 Project Overview

This project analyzes self-collected personal finance data from my daily spending notebook.
I transformed raw handwritten records into a structured dataset, cleaned it, and performed exploratory data analysis (EDA) to understand spending habits, savings rates, and opportunities to optimize costs.

The project demonstrates:

Real-world data collection (messy → structured)

Data cleaning & preprocessing in Python (dates, categories, reimbursements, etc.)

Exploratory data analysis (EDA) with pandas

Extracting financial insights & KPIs from raw transactions

🗂 Dataset

Source: My own spending records (not synthetic data)

Raw fields: date, month, day_of_week, amount, description

Cleaned fields: datetime, day_of_week, category, sub_category, amount, description

Period covered: 2025-03-28 → 2025-08-24

Size: 315 transactions

🧹 Data Cleaning

Main steps:

Date normalization: combined day/month into datetime column (year = 2025).

Amount normalization: all amounts positive; added type = expense/income.

Category/Subcategory mapping: built rulebook for groceries, cafes, utilities, gifts, etc.

Reimbursements handling: recorded as income → Reimbursements so net category spend is accurate.

Export: final cleaned dataset → data/processed/daily_costs_cleaned.csv.

📈 Exploratory Data Analysis (EDA)

Key summaries:

Overview

Total expenses: 68,396,000 Toman

Total income: 73,554,000 Toman

Net balance: +5,158,000 Toman

Avg expense: ~251,000 Toman | Median: 120,000 Toman
AVG income: ~1,711,000 Toman | Median: 400,000 Toman 


🛠 Tools & Libraries

Python (pandas, numpy)

Jupyter Notebook

Matplotlib / Seaborn (for visualization)

└── README.md
