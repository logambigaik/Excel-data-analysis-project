# 📊 Hotel Reservation Data Analysis Project

**Tool Used:** Microsoft Excel  
**Project Type:** Exploratory Data Analysis  
**Data Source:** Skillable Labs – Excel-based assignment  
**Objective:** Understand how lead time, reservation status, and distribution channels relate to booking cancellations using Excel analytics tools (conditional formatting, sparklines, histograms, scatter plots, and charts).

---

## 🔍 Explore Sheet: Conditional Formatting & Sparklines

**Steps:**
1. Applied a color scale to cells **D9:O17** to visually assess reservation volumes by month and lead time category.
2. Created a **sparkline** in cell **P9** for the "Cancelled & Long" row to visualize monthly trends.
3. Dragged the sparkline down through **P17** to represent trends for all reservation statuses and lead time types.


<img width="600" height="404" alt="image" src="https://github.com/user-attachments/assets/81fa9a25-2164-49c2-bdd8-252388878dae" />


**Observations:**
- Cancellations in the "Long" lead time category peaked in certain months.
- "Kept" reservations were more stable across short and medium lead times.
- A clear seasonality is present in reservation behavior.

---

## 📈 Lead Time Sheet: Histogram of Raw Lead Time

**Steps:**
- Created a **histogram** of raw lead time data.

**Observations:**
- Most bookings are made within a short lead time (0–50 days).
- A long tail exists for extended lead times, suggesting some early bookings but less frequently.

---

## 📊 Lead Time by Status Sheet: Histograms by Status

**Steps:**
- Created a **histogram** of the `Cancelled` column.
- Created a **histogram** of the `Kept` column.

**Observations:**
- Cancelled reservations are more likely to have longer lead times.
- Kept reservations cluster toward shorter lead times.
- Suggests longer planning windows correlate with higher cancellation risk.

<img width="600" height="772" alt="image" src="https://github.com/user-attachments/assets/667223db-8c33-4b07-894b-28d0f44b590f" />


---

## 🔗 Lead Time to Cancellations Sheet: Scatter Plot

**Steps:**
- Created a **scatter plot** comparing **average lead time** vs. **number of cancellations** by month.

**Observations:**
- Positive correlation: as average lead time increases, cancellations also tend to rise.
- Indicates early bookings are more likely to be cancelled.

<img width="600" height="788" alt="image" src="https://github.com/user-attachments/assets/a269a3a6-57d3-4b41-aa5b-e38e0945b00a" />

---

## 📉 Over Time Sheet: Line Chart (Normalized Trends)

**Steps:**
- Created a **line graph** comparing normalized average lead time and number of cancellations over time.

**Observations:**
- Both metrics follow a similar seasonal pattern.
- Suggests that seasonality may influence both lead time and cancellations simultaneously.

<img width="600" height="934" alt="image" src="https://github.com/user-attachments/assets/38906d62-9f59-41eb-96dc-0fc9a9fbaa0c" />

---

## 🛎️ By Distribution Channel Sheet

### 1. Bar Chart: Average Lead Time by Distribution Channel
- Direct bookings show the shortest average lead time.
- Travel agent bookings show the longest lead time.

### 2. Stacked Bar Chart: Kept vs. Cancelled by Channel
- Travel agents had the highest cancellation volume relative to their total bookings.
- Direct bookings had the lowest cancellation rate.

## 3. Clustered Column Chart: Cancellation % by Channel & Lead Time
- Long lead time travel agent bookings had the highest cancellation percentage.
- Short lead time bookings across all channels had the lowest cancellation rates.

**Overall Observations:**
- Distribution channels influence both lead time and cancellation behavior.
- Direct bookings are more stable and likely to be kept.
- Longer lead times significantly correlate with cancellation risk, especially in agent-driven bookings.

---

<img width="600" height="948" alt="image" src="https://github.com/user-attachments/assets/bf57ef55-a33f-4b49-ab08-2706124fd9fb" />

## 🧾 Summary

This project allowed me to explore how **lead time**, **reservation status**, **seasonality**, and **sales channels** interact to affect cancellation rates. I used various Excel tools—like conditional formatting, sparklines, histograms, scatter plots, and line/bar charts—to draw insights and identify patterns that can support data-driven hotel operations strategies.
