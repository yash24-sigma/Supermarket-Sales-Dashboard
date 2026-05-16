# 🛒 Supermarket Sales Dashboard — Power BI

A sales dashboard built on **5,901 transactions** across **2024–2025**, covering $1.6M in revenue across the United States.

## 🔍 Key Insights

**1.Total Sales generared across United State is $1.6M**

**2.Total Profite generared across United State is $184.1K**

**3. Average days required for delivery is 4 days.**

**4. Revenue grew. Profit margin didn't.**
Sales jumped 77% from 2024 to 2025. But profit margin dropped from 14.5% to 9.3%. Growing fast while earning less per dollar is a risk, not a win.

**5. COD dominates Payment.**
COD leads at $667K (42.6%). Most people preferred COD payment as a safe option.

**6. Chairs vs Phones on Sales .**
Phones top the sub-category chart at $196.6K sales. 

**7.Sales in October 2024 was low but profit was high**
 

---

## 🧹 Data Quality Fix

A full audit was done on the profit column before publishing any numbers.

- **14 rows** had profit greater than sales — mathematically impossible. These were excluded.
- **108 rows** had margins below -100% — flagged for review.
- Fix applied using **Power Query** (flag column) + **DAX** (Adjusted Profit measure).
- Result: profit corrected from $175.3K → **$184.1K**.

---

## 🛠 Tools Used

`Power BI` &nbsp;|&nbsp; `Power Query` &nbsp;|&nbsp; `DAX` &nbsp;|&nbsp; `Excel` &nbsp;|&nbsp; 

---

## 📁 Files

| File | Description |
|---|---|
| `ANALYSIS.pbix` | Power BI dashboard file |
| `SuperStore Sales edited.xlsx` | Cleaned source dataset |
