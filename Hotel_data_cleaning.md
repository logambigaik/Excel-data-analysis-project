# Excel Data Cleaning and Formatting Project

This project involved importing and cleaning booking data in Excel, preparing it for analysis by handling whitespace, missing values, formatting issues, and identifying inconsistencies.

---

## 📥 Step 1: Import Bookings CSV

- Imported the CSV file using `,` as the delimiter.
- Ensured data started at cell `A1`.
- Renamed the sheet to `bookings`.

![Step 1 - Import CSV](screenshots/step1_import_csv.png)

---

## ✂️ Step 2–4: Trim Whitespace

- Trimmed whitespace in the `hotel`, `status`, and `day` columns using the `TRIM()` formula.
  - `F2 = TRIM(A2)`
  - `G2 = TRIM(B2)`
  - `H2 = TRIM(D2)`

![Step 2 - Trim Columns](screenshots/step2_trim_columns.png)

---

## 🔤 Step 5: Normalize Hotel Data

- Created a one-letter hotel code in column `I` to ensure consistent encoding.
  - `I2 = LEFT(F2,1)`

![Step 5 - Normalize Hotel Column](screenshots/step5_normalize_hotel.png)

---

## 🔍 Step 6: Check for Missing Data

- Applied filters to each column and checked for `(Blanks)`.
- Documented findings in the `Import and Inspect` sheet.

![Step 6 - Missing Data](screenshots/step6_missing_data.png)

---

## ⚠️ Step 7–8: Check for Outliers

- Sorted the `arrival` column to find suspicious dates.
- Sorted `special requests` and recorded any abnormal values in the summary table.

![Step 7 - Suspicious Dates](screenshots/step7_arrival_sort.png)

![Step 8 - Special Requests Outliers](screenshots/step8_special_requests.png)

---

## 🧮 Step 9: Format Percentages

- Applied percentage formatting (no decimals) to the top summary table in the `Format Numbers` sheet.

![Step 9 - Format Percentages](screenshots/step9_percentage_format.png)

---

## 📅 Step 10: Format Dates

- Re-formatted reservation dates from number format to `Short Date`.

![Step 10 - Format Dates](screenshots/step10_format_dates.png)

---

## 📊 Step 11: Sort Table

- Sorted the second table on the `Format Numbers` sheet to improve readability.

![Step 11 - Sort Final Table](screenshots/step11_sort_table.png)

---

## ✅ Summary

- Cleaned and normalized data for consistency.
- Identified missing and suspicious values.
- Applied appropriate formatting for reports and presentation.
- Ensured the dataset is now ready for further analysis or visualization.

---
