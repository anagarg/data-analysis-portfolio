# DoorDash Delivery Analysis

## Overview
This project analyzes DoorDash delivery data to understand delivery-time variability, differences between markets, and customer ordering preferences across cuisine types.

The analysis uses Excel formulas, PivotTables, descriptive statistics, and data visualization to examine delivery performance across six U.S. markets and identify opportunities for DoorDash to tailor its operations and offerings to local customer demand.

The project was completed as part of the Global Career Accelerator Data Analytics program.

## Business Questions
This analysis addresses several questions:
- How long does a typical DoorDash order take to be delivered?
- How consistent are delivery times?
- How do order volume, delivery time, and order value vary across markets?
- Which cuisine types are most popular overall and within individual markets?
- How can DoorDash use these patterns to tailor its service offerings?

## Data
The dataset contains **50,036 DoorDash orders** across six U.S. markets:
- Boston
- Chicago
- Los Angeles
- New York City
- San Francisco
- Seattle

Key variables include:
- Market
- Order creation time
- Delivery time
- Restaurant
- Restaurant cuisine category
- Order protocol
- Total items
- Order subtotal
- Number of distinct items
- Minimum item price
- Maximum item price
- Number of Dashers on shift
- Number of busy Dashers
- Number of outstanding orders

The dataset also includes timestamps for when orders were created and delivered, which were used to calculate delivery time in minutes.

## Analysis

### 1. Delivery Time Analysis
I calculated the elapsed delivery time for each order by measuring the difference between the order creation timestamp and delivery timestamp.

I then calculated the:
- Average delivery time
- Standard deviation of delivery time

The average delivery time was approximately **49.9 minutes**, while the standard deviation was approximately **21.6 minutes**.

The relatively large standard deviation indicates substantial variation in delivery times. While the average provides a general expectation of approximately 50 minutes, individual orders can take considerably more or less time.

Potential operational factors that could contribute to this variation include restaurant preparation time, traffic, driver availability, weather, and delivery distance.

### 2. Market Analysis
I created a PivotTable comparing the six markets by:
- Total number of orders
- Average order price
- Average delivery time

| Market | Orders | Average Order Price | Average Delivery Time |
|---|---:|---:|---:|
| New York City | 14,343 | $26.38 | 47.53 min |
| Chicago | 11,785 | $28.87 | 48.98 min |
| San Francisco | 9,310 | $27.23 | 55.04 min |
| Los Angeles | 5,924 | $25.52 | 50.83 min |
| Boston | 4,729 | $24.45 | 48.10 min |
| Seattle | 3,945 | $24.70 | 49.66 min |
| **Total** | **50,036** | **$26.71** | **49.88 min** |

New York City had the highest number of orders and the lowest average delivery time among the six markets.

Chicago had the highest average order price, while San Francisco had the highest average delivery time.

### 3. Cuisine Analysis
I created a PivotTable to examine the number of orders by restaurant cuisine category.

The most popular cuisine category overall was **American**, accounting for approximately **9.91% of orders**.

Other highly represented categories included:
- Mexican — approximately 8.78%
- Pizza — approximately 8.70%
- Sandwich — approximately 5.04%
- Burger — approximately 5.38%

I then added market-level grouping to examine the percentage distribution of cuisine types within each city.

### 4. Regional Cuisine Preferences
The market-level analysis showed that cuisine preferences differed across cities.

For example:
- American cuisine was the most popular overall and was the most popular cuisine within **three markets**.
- Chinese cuisine represented approximately **7.25% of Boston's orders**.
- Seattle had the highest percentage of orders from sandwich restaurants at approximately **7.35%**.

These differences demonstrate that customer ordering patterns vary across markets and can be used to inform localized strategies.

### 5. Delivery Time by Cuisine
As an optional LevelUp analysis, I created a PivotTable comparing [average delivery time across cuisine categories]((images/avg_delivery_time.png)) and sorted the results from longest to shortest delivery time.

The cuisine with the highest average delivery time was **Spanish**, at approximately **66.3 minutes**.

Other cuisines with relatively high average delivery times included:
- Tapas — 61.8 minutes
- Moroccan — 60.2 minutes
- Comfort-food — 59.8 minutes
- Kosher — 57.6 minutes

This analysis can help identify cuisine categories where operational improvements may have the greatest potential impact on delivery times.

## Key Findings

### Delivery Performance
- The average DoorDash delivery time was approximately **49.9 minutes**.
- The standard deviation was approximately **21.6 minutes**, indicating considerable variation in delivery times.
- San Francisco had the highest average delivery time at approximately **55.0 minutes**.
- New York City had the lowest average delivery time at approximately **47.5 minutes**.

### Market Performance
- New York City had the highest order volume with **14,343 orders**.
- Chicago had the highest average order price at approximately **$28.87**.
- San Francisco had the highest average delivery time.
- Seattle had the lowest order volume among the six markets.

### Cuisine Preferences
- American cuisine was the most popular category overall, representing approximately **9.91% of orders**.
- American cuisine was the most popular category in three of the six markets.
- Chinese cuisine represented approximately **7.25% of Boston's orders**.
- Seattle had the highest percentage of orders from sandwich restaurants at approximately **7.35%**.

### Cuisine and Delivery Time
- Spanish cuisine had the highest average delivery time in the optional cuisine-level analysis at approximately **66.3 minutes**.
- Delivery times varied considerably across cuisine categories.

## Recommendations
Based on the market and cuisine analysis, DoorDash could consider tailoring its operations and marketing strategies to individual markets rather than applying the same strategy across all cities.

### 1. Strengthen American Restaurant Partnerships
American cuisine was the most popular category overall and was particularly prominent in Boston, San Francisco, and Los Angeles.

DoorDash could consider expanding restaurant partnerships and promotional placement for American restaurants in markets where demand is strongest.

### 2. Expand Chinese Cuisine Options in Boston
Chinese restaurants represented approximately **7.25% of Boston's orders**.

DoorDash could consider strengthening its Chinese restaurant selection in Boston and using targeted promotions to increase visibility among customers.

### 3. Tailor Seattle Offerings to Sandwich Demand
Seattle had the highest percentage of orders from sandwich restaurants at approximately **7.35%**.

DoorDash could consider recruiting additional sandwich restaurants, promoting lunch specials, and highlighting sandwich options during peak lunch hours.

### 4. Investigate Long Delivery Times by Cuisine
The LevelUp analysis identified Spanish cuisine as having the highest average delivery time at approximately **66.3 minutes**.

DoorDash could investigate whether restaurant preparation time, delivery distance, Dasher availability, or other operational factors contribute to longer delivery times for this category before implementing targeted operational changes.

## Business Implications
The analysis demonstrates that DoorDash's markets have different combinations of order volume, customer preferences, order values, and delivery performance.

Using market-level data could allow DoorDash to:
- Allocate Dashers according to local demand
- Identify markets with longer delivery times
- Tailor restaurant recruitment
- Develop localized promotions
- Highlight cuisine categories that are particularly popular in each market
- Investigate operational bottlenecks affecting specific cuisine categories

The analysis identifies patterns in the data, but the available dataset does not establish that individual factors such as traffic, weather, or driver availability caused differences in delivery time.

## Excel Techniques Used
- Excel formulas
- Date/time calculations
- Descriptive statistics
- Average calculations
- Standard deviation
- PivotTables
- Percentage-of-total analysis
- Sorting
- Grouping
- Horizontal bar charts
- Market-level analysis
- Category analysis
- Data-driven recommendations

## Visualizations
[Average Delivery Time by Cuisine Type](images/avg_delivery_time.png)

## Excel Workbook
[DoorDash Delivery & Customer Analysis](doordash-delivery-analysis.xlsx)

## Project Context
This project was completed as part of the Global Career Accelerator Data Analytics program.

The project simulated a real-world operations analytics scenario for DoorDash. The analysis focused on delivery performance, market-level differences, and customer cuisine preferences to identify opportunities for improving service efficiency and tailoring offerings to local demand.
