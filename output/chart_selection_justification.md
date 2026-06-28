# Chart Selection Justification

This document explains the purpose, design decisions, and visualisation choices behind each major chart included in the Tableau Executive Dashboard.

---

# 1. Sales Trend & Growth Analysis

### Business Question
How are sales changing over time?

### Chart Type
Line Chart

### Why This Chart?
A line chart is the most effective format for displaying trends across months and identifying seasonal shifts or growth patterns.

### Fields Used

* **X-Axis:** Order Date (Month)
* **Y-Axis:** Sales
* **Color:** Region
* **Filter:** Region, Customer Segment, Category

### Design Principle Applied

* Continuous timeline used to support trend analysis
* Consistent colour coding applied per region
* Visual clutter kept to a minimum

### Mistake Avoided
Pie charts and column charts were not used, as they are poorly suited to communicating time-based trends.

---

# 2. Regional Performance Dashboard

### Business Question
Which region produces the highest sales?

### Chart Type
Bar Chart

### Why This Chart?
Bar charts make cross-regional comparison straightforward and allow the highest and lowest performers to be identified at a glance.

### Fields Used

* **Category:** Region
* **Measure:** Sales
* **Color:** Sales Value
* **Filter:** Customer Segment, Category

### Design Principle Applied

* Bars sorted to facilitate quick comparison
* Consistent colour intensity applied throughout
* Clear and descriptive axis labels included

### Mistake Avoided
3D charts and decorative visual effects were avoided as they reduce overall readability.

---

# 3. Product Category Profitability

### Business Question
Which product categories and sub-categories generate the highest profit?

### Chart Type
Horizontal Bar Chart

### Why This Chart?
Horizontal bars improve readability when multiple category names need to be displayed and allow for easy ranking across sub-categories.

### Fields Used

* **Category:** Sub-Category
* **Measure:** Profit
* **Color:** Category
* **Label:** Profit

### Design Principle Applied

* Bars sorted in descending order for instant prioritisation
* Consistent category colours used throughout
* Data labels added to aid direct comparison

### Mistake Avoided
Stacked bars were avoided because they would make it harder to compare individual sub-category profitability.

---

# 4. Customer Segment Analysis

### Business Question
How does sales performance differ across customer segments?

### Chart Type
Bar Chart

### Why This Chart?
A bar chart clearly communicates sales differences across customer segments and makes performance comparisons easy to read.

### Fields Used

* **Category:** Customer Segment
* **Measure:** Sales
* **Color:** Profit
* **Label:** Sales

### Design Principle Applied

* Equal-width bars for fair visual comparison
* Simple and uncluttered layout
* Readable labels throughout

### Mistake Avoided
Pie charts were avoided as comparing values across segments is far more intuitive with bars.

---

# 5. Shipping & Delivery Performance

### Business Question
Which shipping mode carries the longest average delivery time?

### Chart Type
Stacked Bar Chart

### Why This Chart?
The stacked bar chart displays average delivery days per shipping mode while also showing how different delivery delay categories contribute to the total.

### Fields Used

* **Category:** Ship Mode
* **Measure:** Average Delivery Days
* **Color:** Shipping Delay Bucket

### Design Principle Applied

* Consistent colours used for each delay bucket
* Clear cross-mode comparison maintained

### Mistake Avoided
Complex heat maps were avoided as they would make delivery time comparisons harder to interpret.

---

# 6. Impact of Discount on Profitability

### Business Question
How do discount levels affect profit?

### Chart Type
Scatter Plot

### Why This Chart?
A scatter plot is the most appropriate format for revealing relationships between two continuous variables.

### Fields Used

* **X-Axis:** Discount
* **Y-Axis:** Profit
* **Color:** Category
* **Detail:** Order ID

### Design Principle Applied

* Individual order-level data points plotted for granular visibility
* Trends and outliers easy to identify visually

### Mistake Avoided
Line charts were not used because discount values do not follow a sequential time-based progression.

---

# 7. Return Pattern Analysis

### Business Question
Which product categories and customer segments record the highest return volumes?

### Chart Type
Stacked Bar Chart

### Why This Chart?
The stacked bar chart allows total returned orders to be compared across product categories while simultaneously showing each customer segment's contribution to that total.

### Fields Used

* **Category:** Category
* **Measure:** Return Flag
* **Color:** Customer Segment
* **Label:** Returned Orders

### Design Principle Applied

* Clear category-level comparison maintained
* Consistent segment colours applied throughout
* Return distribution easy to interpret at a glance

### Mistake Avoided
Pie charts were avoided as comparing multiple categories simultaneously is far more difficult using a circular format.

---

# Overall Dashboard Design Principles
The dashboard was developed in line with established business intelligence and data visualisation best practices:

* Chart types selected to match the specific business question being addressed
* Consistent colour palette applied across all visualisations
* Clear titles and descriptive labels on every chart
* Interactive filters available for Region, Category, Customer Segment, and Ship Mode
* Dashboard action filters included to enable dynamic exploration
* Minimal clutter with emphasis on readability throughout
* Proper sorting and formatting applied to aid interpretation
* Focus placed on supporting executive decision-making rather than decorative visual design
