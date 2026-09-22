# Warby Parker Website A/B Testing Analysis

## Overview
This project analyzes an A/B test for Warby Parker's website to determine whether a redesigned landing page affected user satisfaction.

The analysis compares satisfaction ratings from users who viewed the original landing page with ratings from users who viewed the new landing page. A two-sample t-test assuming unequal variances was used to determine whether the difference between the two groups was statistically significant.

The project also examines regional and demographic patterns in user ratings and provides recommendations for designing future A/B tests.

The project was completed in Excel as part of the Global Career Accelerator Data Analytics program.

## Business Question
Does changing Warby Parker's landing page result in a statistically significant difference in user satisfaction?

The analysis also explores whether user ratings vary by region, age, and income.

## A/B Test Design

### Control Group
Users in the control group viewed the **original version** of the website.

### Test Group
Users in the test group viewed the **new version** of the website.

Users rated their satisfaction with the website on a scale from **1 to 5**:
- 1 = Least satisfied
- 5 = Most satisfied

### Hypotheses

**Null Hypothesis (H₀):**

The change to the landing page will not result in a difference in user satisfaction and opinion.

**Alternative Hypothesis (H₁):**

The change to the landing page will result in a difference in user satisfaction and opinion.

Because the analysis tests for a difference in either direction, a **two-tailed test** was used.

## Data
The main A/B testing dataset contains **3,365 user responses**.

Each record includes:
- Cookie ID
- Device type
- Operating system
- Date
- Hour
- Test condition
- User rating

The `condition` variable identifies which version of the website the user saw:
- `0` = Original website / control group
- `1` = New website / test group

All users in the dataset accessed the website using a mobile device.

The workbook also contains additional regional and demographic information for the test users, including:
- Region
- Age
- Income

Regions are coded as:
- Region 1 = Northeast
- Region 2 = South
- Region 3 = Midwest
- Region 4 = West

## Analysis

### 1. A/B Test Results
I separated the user ratings into test and control groups and used Excel's Data Analysis ToolPak to conduct a **two-sample t-test assuming unequal variances**.

The results were:

| Metric | Test Group | Control Group |
|---|---:|---:|
| Observations | 1,699 | 1,666 |
| Average Rating | 3.34 | 3.28 |
| Variance | 1.51 | 1.46 |

The test group had a slightly higher average satisfaction rating than the control group.

### 2. Statistical Significance
The two-tailed t-test produced a **p-value of 0.1494**.

Using a 95% confidence level:
- Significance level: **α = 0.05**
- p-value: **0.1494**
- Since p > α, the null hypothesis was not rejected.

The results therefore do not provide sufficient statistical evidence to conclude that the new landing page produced a difference in user satisfaction.

The observed difference in average ratings could reasonably be due to random variation.

### 3. Potential Statistical Error
Because the analysis did not find a statistically significant difference, there is a possibility of making a **Type II error**.

A Type II error would occur if the new landing page actually affected user satisfaction but the test failed to detect the difference.

The business consequence could be missing an opportunity to implement a landing page that genuinely improves user engagement or conversions.

### 4. Recommendations for Future A/B Tests
The analysis identified several ways to improve future experiments:
- Define the hypothesis before collecting data.
- Establish the primary success metric in advance.
- Calculate the required sample size before launching the experiment.
- Randomly assign users to the control and test groups.
- Track additional business metrics beyond satisfaction ratings.
- Control for external factors such as marketing campaigns, holidays, and seasonal trends.
- Consider metrics such as conversion rate, purchases, revenue, and time on site.

This would help ensure that future experiments are designed to measure meaningful business outcomes rather than relying on a single satisfaction metric.

## Regional and Demographic Analysis
The workbook includes additional data for test users that allows user ratings to be examined by region, age, and income.

### 5. User Ratings by Region
I created a PivotTable comparing the average user rating across the four regions.

| Region | Average Rating |
|---|---:|
| Northeast | 3.00 |
| South | 3.74 |
| Midwest | 3.64 |
| West | 2.26 |
| **Overall** | **3.34** |

The average rating varies across regions in the dataset.

The South had the highest average rating at approximately **3.74**, while the West had the lowest at approximately **2.26**.

These differences identify regional patterns worth exploring further, but the analysis does not establish that region itself causes differences in satisfaction.

### 6. User Age by Region
I created a PivotTable comparing average age across regions.

| Region | Average Age |
|---|---:|
| Northeast | 34.61 |
| South | 33.77 |
| Midwest | 36.95 |
| West | 41.44 |
| **Overall** | **36.62** |

The West had the highest average age, while the South had the lowest.

### 7. User Income by Region
I also compared average income across regions.

| Region | Average Income |
|---|---:|
| Northeast | $65,327 |
| South | $67,371 |
| West | $74,157 |
| Midwest | $74,786 |
| **Overall** | **$71,592** |

The Midwest had the highest average income in the dataset, while the Northeast had the lowest.

### 8. Age and User Ratings
The workbook also compares average user ratings between customers younger than 25 and customers aged 25 or older.

| Age Group | Average Rating |
|---|---:|
| Under 25 | 4.84 |
| 25 or older | 3.14 |
| **Overall** | **3.34** |

The under-25 group had a substantially higher average rating than the 25-or-older group in this dataset.

This is an observed association within the sample and should not be interpreted as evidence that age itself causes differences in satisfaction.

## Key Findings
- The A/B test contained **3,365 user responses**.
- The test group contained **1,699 users**, while the control group contained **1,666 users**.
- The new landing page had an average rating of approximately **3.34**.
- The original landing page had an average rating of approximately **3.28**.
- The difference in average ratings was relatively small.
- The two-tailed t-test produced a **p-value of 0.1494**.
- At the 95% confidence level, the result was **not statistically significant**.
- The analysis therefore did not provide sufficient statistical evidence that the new landing page changed user satisfaction.
- Average ratings varied across the four regions.
- The South had the highest average regional rating, while the West had the lowest.
- Users under 25 had a higher average rating than users aged 25 or older in the analyzed sample.
- Regional differences in age and income were also observed.

## Business Recommendation
Based on the A/B test results, the analysis does not provide sufficient statistical evidence to conclude that the new landing page improves or worsens user satisfaction.

Rather than making a decision based solely on the observed difference in average ratings, Warby Parker should consider conducting a follow-up experiment with a clearly defined success metric and sufficient sample size.

Future testing should also incorporate business outcomes such as:
- Conversion rate
- Purchases
- Revenue
- Time on site
- Customer engagement

These metrics would help determine whether a landing-page change produces meaningful business results even when differences in satisfaction ratings are small.

## Business Implications of Statistical Errors
A **Type I error** would occur if Warby Parker concluded that the new landing page affected user satisfaction when it actually did not. This could lead the company to adopt an ineffective design and potentially spend resources implementing a change that does not improve performance.

A **Type II error** would occur if the new landing page actually improved satisfaction but the experiment failed to detect the difference. This could cause Warby Parker to reject a potentially beneficial design and miss opportunities to improve user experience or business performance.

## Excel Techniques Used
- Data Analysis ToolPak
- Two-sample t-test assuming unequal variances
- Hypothesis testing
- p-value interpretation
- Statistical significance
- PivotTables
- Average calculations
- Regional segmentation
- Demographic analysis
- Data interpretation
- Experimental design
- Business recommendations

## Excel Workbook
[]()

## Project Context
This project was completed as part of the Global Career Accelerator Data Analytics program.

The project simulated a real-world A/B testing scenario for Warby Parker. The analysis required testing hypotheses, conducting a two-sample t-test, interpreting statistical significance, considering Type I and Type II errors, and examining regional and demographic patterns in user satisfaction.
