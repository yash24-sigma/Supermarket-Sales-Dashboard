## Supermarket Sales Dashboard — Power BI

Two years of US supermarket sales data, cleaned, analyzed, and turned into a dashboard that shows where the business is actually making money — and where it isn't.

## 1. Background and Overview

A US-based supermarket chain needed a clear picture of its sales and profit performance across states, product categories, and customer types.

This project builds a full sales dashboard in Power BI covering 2024 and 2025 — with a data audit done before any analysis, to make sure the numbers are trustworthy.

Detail	Info
Tool	Power BI
Dataset Size	5,901 rows
Period	Jan 2024 – Dec 2025
Total Revenue	$1.6M
Adjusted Profit	$184.1K

## 2. Data Structure Overview

The dataset is a single flat table with the following columns:

Order Info — Order ID, Order Date, Ship Date, Ship Mode

Customer Info — Customer ID, Segment (Consumer / Corporate / Home Office)

Location — City, State, Region

Product Info — Category, Sub-Category, Product Name

Financials — Sales, Quantity, Profit, Returns, Payment Mode

Note: No cost or discount column exists in the raw data. Profit is pre-calculated in the source file.

## 3.  Executive Summary

The business generated $1.6M in sales and $184.1K in adjusted profit across two years. On the surface that looks healthy. But two things stand out when you dig in:

Sales grew 77% from 2024 to 2025. Profit margin fell from 14.5% to 9.3% in the same period. The business is scaling but earning less per sale.
Some of the strongest states by revenue are quietly losing money. High sales numbers alone do not tell the full story.

The dashboard makes both of these visible — along with product, region, and customer breakdowns.

## 4.  Insights Deep Dive
- Revenue vs Profit — Not the Same Thing
 Sales jumped 77% year over year. But profit margin dropped from 14.5% in 2024 to 9.3% in 2025.
 For every $100 sold, the business kept only $11.50 as profit. And that number is shrinking. Growing revenue with falling margins is a warning sign worth           investigating.

- California Carries Too Much Weight
  California brought in $335.2K in sales — more than New York ($186.7K) and Texas ($116.3K) combined. That level of dependence on one state is a business risk.      One bad quarter in California and the overall numbers take a serious hit.

- Office Supplies vs Technology — Sales Lie, Margins Tell the Truth
  Category	Sales	Profit
  Office Supplies	$643.7K	$84,628
  Technology	$470.6K	$84,558
  Furniture	$451.5K	$14,939
  
  Office Supplies sells the most. But Technology makes nearly the same profit on $173K less in sales. Furniture does $451.5K in sales for only $14,939 in profit —   a 3.3% margin. The business is spending effort on Furniture for very little return.

- Texas Is Losing Money
  Texas ranks 3rd by sales at $116.3K. Its actual profit is negative. The business is spending resources to sell in Texas and coming out behind. This needs a root   cause investigation — shipping costs, discounts, or product mix could all be factors.

- The Best-Selling Sub-Category Is Not the Most Profitable
  Phones lead sub-category sales at $196.6K. But Binders generate more profit than Phones despite lower sales. Volume and profitability are two different metrics    and they often point in opposite directions.

- East Region Is Second-Largest but Least Efficient
  Region	Sales Share	Margin
  West	33.37%	12.99%
  East	28.75%	11.86%
  Central	21.78%	8.05%
  South	16.10%	10.53%

  West leads in both volume and efficiency. Central has the lowest margin at 8.05% — almost half of West. South is the smallest region and likely has the most       room to grow.

- Consumers Drive the Revenue
  The Consumer segment accounts for $753K — nearly half of total revenue. Corporate adds $509.7K and Home Office $303K. The business leans heavily on individual     buyers rather than business clients.

- Cash on Delivery Is the Top Payment Method
  By actual revenue, COD leads at 42.6%, followed by Online at 35.4% and Cards at 22%. The original dashboard chart showed the wrong order because it was counting   number of orders instead of revenue value — this was corrected.

## 5.  Recommendations

- Investigate Texas immediately High sales, negative profit — something is off. Check if heavy discounts or high shipping costs are behind this.

- Reassess the Furniture category $451.5K in sales for a 3.3% margin is not worth the logistics cost. Either reprice or reduce focus.

- Reduce California dependence One state driving this much revenue is a concentration risk. South at 16.1% looks underdeveloped and could be a growth target.

- Push Technology over Office Supplies Same profit on lower sales means better efficiency. Technology is the smarter category to focus on.

- Review Central region operations 8.05% margin is the lowest across all regions. Pricing, product mix, or logistics costs could be pulling it down.

## 6.  Assumptions and Limitations
- Profit values are taken as-is from the source file. No cost or discount data was available to verify them independently.
- 14 rows where profit exceeded sales were excluded from calculations and treated as data entry errors.
- 108 rows with margins below -100% were flagged for review but kept in the raw data.
- The dataset covers the US only. No international sales data is included.
- Payment mode percentages in the original dashboard were based on order count. All payment analysis here uses revenue value instead.

## 7.  Future Enhancements
- Profitability drill-down — let users click a state or category and see exactly which products are behind the losses.
- Discount column — would make it possible to properly explain why some rows have negative profit.
- Return rate page — returns data exists in the dataset but is not currently visualized.
- Forecasting — project 2026 trends using Power BI's built-in forecast feature.
- Live data refresh — connect to a live source so the dashboard updates without manual file uploads.
  
## 8. Deliverables
File	What It Contains
ANALYSIS.pbix	Full Power BI dashboard with all visuals, DAX measures and Power Query steps
SuperStore_Sales_edited.xlsx	Source dataset — 5,901 rows
README.md	Full project documentation

## 9. Outcomes Preview :
- Dashboard : https://github.com/yashmonde24/Supermarket-Sales-Dashboard/blob/main/outputs/salesdashboard.png
- Sales Forecast : https://github.com/yashmonde24/Supermarket-Sales-Dashboard/blob/main/outputs/salesforecasting.png
