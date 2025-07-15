# 📊 Bitcoin vs. S&P500: Excel Analysis Project

This Excel-based data analysis project compares the performance and volatility of Bitcoin with the S&P500 index for the year 2021. The project demonstrates data cleaning, exploratory analysis, pivot tables, and visual storytelling through charts — all done in Microsoft Excel.

---

## 📁 Dataset

The dataset (`data.csv` or `data-semicolon.csv`, depending on system locale) contains daily values for Bitcoin and the S&P500 index across 2021.

---

## 📝 Scenario

Manuela, Head of Finance, is considering the potential of Bitcoin. She's curious about its growth potential but cautious about its volatility. You have been asked to analyze Bitcoin’s 2021 performance and compare it with the S&P500 — the benchmark for stability.

---

## ✅ Tasks Completed

### 1. Import and Inspect the Data

- Imported dataset into `bitcoin-analysis.xlsx`.
- Trimmed whitespace from all text fields using `TRIM()` function.
- Checked for inconsistencies in text data (e.g., variations in symbol names) and resolved using formulas like `UPPER()` and `SUBSTITUTE()`.

![Trim Text Columns](screenshots/step2_trim.png)

- Checked for blanks in text columns using filters and `COUNTA()`.

- Checked for missing values in numeric and date fields using `COUNTBLANK()`.

- Identified any unusually high or low values that may require attention in further analysis.

---

### 2. Upside Analysis (Sheet: `Upside`)

- Identified first and last trading days of 2021 for both Bitcoin and S&P500.
- Recorded opening and closing values.
- Calculated percentage change using:

```excel
= (Closing - Opening) / Opening
```
