# 🛒 Supermarket Sales Dashboard - Power BI

A sales dashboard built on **5,901 transactions** across **2024–2025**, covering $1.6M in revenue across the United States.

## 🔍 Key Insights

**1.Total Sales generared across United State is $1.6M**

**2.Total Profite generared across United State is $184.1K**

**3. Average days required for delivery is 4 days.**

**4.The Business is Profitable — But Margins Are Shrinking**
The business made $184.1K profit on $1.6M in sales. That means for every $100 sold, only about $11.50 is actual profit. And this number was higher in 2024 — so profit per sale is getting smaller over time even though total sales are growing.

**5.California Carries the Business**
California alone brought $335.2K in sales — more than New York and Texas combined. If California had a bad year, the whole business would feel it. Too much dependence on one state is a risk.

**6.Office Supplies Sells the Most — But is it the Most Profitable?**
Office Supplies leads at $643.7K in sales. But profit has very little difference between Office ($84,628).and Technology ($84,558). Technology ($470.6K sales) makes far more profit per dollar sold. Selling more does not always mean earning more.

**7.Furniture Is Quietly Draining Profit**
Furniture sits at $451.5K in sales — almost equal to Technology. But Furniture's profit is only around $14,939. That means the business is doing a lot of work for very little return on Furniture products.

**8.Phones Sell the Most — But Copiers Make More Profit**
Phones top the sub-category chart at $196.6K. But if you look at actual profit, Binders make more profit than  what Phones make. The product that sells the most is not always the one making the most money.

**9.East Region Is Underperforming**
East region is #2 in sales at 28.75% but runs a lower profit margin than West. West leads in both sales (33.37%) and efficiency. South is the smallest region at 16.1% — a clear growth opportunity.
 
**10.Regular Customers Drive the Business**
Consumer segment brings in $753K — almost half of total revenue. Corporate adds $509.7K and Home Office $303K. The business depends heavily on individual buyers, not companies.

**11. Customers prefers Cash On Delivery for Payment Mode  rather than 

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

Demo Preview :
- Dashboard : https://github.com/yashmonde24/Supermarket-Sales-Dashboard/blob/main/outputs/salesdashboard.png
- Sales Forecast : https://github.com/yashmonde24/Supermarket-Sales-Dashboard/blob/main/outputs/salesforecasting.png
