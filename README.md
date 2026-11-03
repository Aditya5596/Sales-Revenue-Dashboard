# AdventureWorks Sales & Performance Dashboard | Power BI

An interactive, multi-page Power BI report that tracks revenue, profit, orders, returns, and customer behaviour for AdventureWorks, a fictional bicycle and accessories retailer. It gives executives a one-page view of performance and lets analysts drill into products, customers, and regions.

![Executive Dashboard](images/Dashboard-Overview.png)

## Business Problem

Leadership needs to answer questions like:

- How are revenue, profit, and orders trending month over month?
- Which product categories and products drive orders, and which have the highest return rates?
- Where (by continent and country) are orders coming from?
- Who are the top customers, and what do high-value customers have in common?
- Are we on track against revenue, profit, and order targets?

## Data

- **Source:** AdventureWorks sample dataset
- **Model:** Star schema with a central measure table and lookup (dimension) tables for Calendar, Product, Product Categories, Product Subcategories, Customer, and Territory

## Tools Used

- **Power BI Desktop:** data modelling, DAX measures, interactive report design
- **Excel / SQL:** used for cleaning and preparing data in this project

## Report Pages

| Page | What it shows |
|---|---|
| **Exec Dashboard** | KPI cards for Revenue, Profit, Orders, and Return Rate; month-over-month KPI trends; revenue trend line; orders by category; top ordered and top returned product types; product table with orders, revenue, and return rate |
| **Map** | Orders by country on an interactive map, filterable by continent |
| **Product Detail** | Profit trend (actual vs adjusted), gauges for Revenue, Profit, and Orders against targets, and a returns trend by selected metric |
| **Customer Detail** | Total customers, average revenue per customer, orders by occupation and income level, customer trends, and a Top 100 Customers table |
| **Decomposition Tree** | Break down total orders by category, subcategory, and product to find what drives volume |
| **Key Influencers** | AI visuals showing which product and customer attributes (price, cost, income, education, occupation, home ownership, and others) influence outcomes |
| **Category Tooltip** | Custom hover tooltip showing orders, revenue, profit, returns, and return rate for a category |

## Key Features

- **Custom navigation:** left-hand nav buttons and icons to move between pages
- **Bookmarks:** show/hide slicer panel and one-click "clear filters" buttons on the Exec and Customer pages
- **What-if analysis:** a Price Adjustment (%) slicer to see how price changes affect profit
- **Dynamic metric switching:** slicers that let users switch the metric shown in the product and customer trend charts
- **Targets:** gauges comparing actual revenue, profit, and orders to target
- **Custom tooltips and mobile layouts** for the main page
## Key Insights

1. **Strong margins and a growth trend.** The business generated ₹17.5M in revenue and ₹7.4M in profit (about a 42% margin) across 19.1K orders. Monthly revenue accelerated from mid-2021 onward and reached ₹1.38M in the latest month, up 1.14% on the previous month.

2. **Order volume and revenue come from different products.** Accessories lead on orders (13.5K) ahead of Bikes (9.9K) and Clothing (5.5K), and Tires and Tubes is the top-ordered product type. But the best-selling items are low-ticket: Water Bottle (30 oz) has the most orders (3,231) yet only ₹32K in revenue, while Fender Set - Mountain earns ₹73K from about half as many orders (1,668).

3. **Helmets have a return problem.** The overall return rate is 2.2%, but the Sport-100 helmets run well above it: Blue at 3.52%, Red at 3.12%, and Black at 2.98%, compared with roughly 1-2% for the other top sellers. Shorts is the top returned product type. Monthly returns did fall from 131 to 123 (about 6%).

4. **The customer base is broad, not concentrated.** There are 17.4K unique customers, and the Top 100 together contribute only about ₹615K, roughly 3.5% of revenue. The top customer (Maurice Shan) spent ₹12.4K across 6 orders, so there is little dependence on a few big accounts.

5. **Customer profile.** Average-income customers place 47.0% of orders, low-income 41.6%, and high-income 11.4%. By occupation, Professionals account for 43.4% of orders, Skilled Manual 32.6%, and Management 24.0%.

6. **Revenue per customer is falling even as revenue grows.** Average revenue per customer dropped from about ₹3K in early 2020 to about ₹1K by 2022. This suggests growth has come from acquiring more customers rather than from each customer spending more, which makes upselling and retention an opportunity.

7. **The US is the dominant market.** On the map it has the largest order volume, with Australia, Canada, the UK, France, and Germany smaller.

8. **Product targets:** For Water Bottle (30 oz) in the latest month, orders were 404 against a target of 438 (about 92%), revenue was ₹4,067 against ₹4,292 (about 95%), and profit was ₹2.55K against ₹2.69K (about 95%). All three are slightly below target.

## Recommendations

- Investigate quality, sizing, or description issues behind the Sport-100 helmet returns, since they are also strong revenue earners.
- Bundle high-volume, low-price accessories (water bottles, tubes, patch kits) with bikes and helmets to raise revenue per order.
- Focus on retention and cross-selling to reverse the decline in revenue per customer.
- Keep investing in the US market, and test growth campaigns in the smaller markets.
## Explore the Report

Download `AdventureWorks_Report.pbix` and open it in Power BI Desktop (free, Windows only). A walkthrough video is linked above for anyone who can't open the file.
