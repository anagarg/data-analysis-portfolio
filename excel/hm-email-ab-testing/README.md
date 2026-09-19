# H&M Email A/B Testing Analysis

## Overview
This project analyzes an A/B test conducted for H&M to determine whether changing the subject line of promotional emails affected email open rates.

The analysis compares a control subject line, "20% off + free shipping," with a test subject line, "Your last chance to score 20% off + free shipping." The project evaluates the experiment design, analyzes the test results, assesses statistical significance, and considers the broader business implications of using the new subject line.

The project was completed in Excel as part of the Global Career Accelerator Data Analytics program.

## Business Question
Does changing H&M's promotional email subject line increase the email open rate, and does the new subject line meet the company's goal of increasing the open rate to 20%?

## A/B Test Design

### Control Group

**Subject line:**

> 20% off + free shipping

### Test Group

**Subject line:**

> Your last chance to score 20% off + free shipping

### Hypotheses

**Null Hypothesis (H₀):**

Changing the email subject line will not result in a significant difference in the open rate of promotional emails.

**Alternative Hypothesis (H₁):**

Changing the email subject line will result in a higher open rate of promotional emails.

### Target
Historically, H&M's promotional emails had an open rate of **18%**.

The company wanted the new subject line to increase the open rate to **20%**.

The analysis calculated a **minimum detectable effect of 11%** and a required total sample size of approximately **9,300 emails**.

## Data
The A/B test dataset contains individual email records with the following variables:
- Group
- Subject line
- Opened

The `Opened` variable indicates whether the recipient opened the email:
- `0` = Email was not opened
- `1` = Email was opened

The final dataset contained **9,437 emails**.

## Analysis

### 1. A/B Test Design
Before analyzing the results, I identified potential factors that could affect the validity of the experiment.

Two potential confounding factors identified were:
- **Audience differences:** If one group contained more loyal or engaged customers, that group could have a higher open rate regardless of the subject line.
- **Time and day sent:** If the two subject lines were sent at different times, differences in open rates could be caused by sending time rather than the subject line.

A potential mitigation strategy is to randomly assign recipients to each group and distribute both subject lines across the same sending windows.

### 2. PivotTable Analysis
I created an Excel PivotTable to summarize the number of emails sent and the number of emails opened in each experimental group.

| Group | Emails Sent | Emails Opened |
|---|---:|---:|
| Control | 4,764 | 836 |
| Test | 4,673 | 894 |
| **Total** | **9,437** | **1,730** |

The control group contained 91 more emails than the test group, while the test group had 58 more opened emails.

### 3. Conversion Rate Analysis
I calculated the open rate for each group:

**Control:**

`836 / 4,764 ≈ 18%`

**Test:**

`894 / 4,673 ≈ 19%`

The test group therefore produced a higher email open rate than the control group.

The workbook's significance analysis reports that the test group converted approximately **10% better** than the control group.

### 4. Statistical Significance
I used an A/B testing significance calculator to evaluate whether the difference between the control and test groups was statistically significant.

The workbook reports **98% certainty** that the observed improvement was not due to random variation and identifies the result as statistically significant.

### 5. Type I Error
Because the analysis involves a hypothesis test, there is a possibility of incorrectly concluding that the new subject line improves open rates when it does not.

This would be a **Type I error (false positive)**.

## Key Findings
- The control group received **4,764 emails**, while the test group received **4,673 emails**.
- The control group had **836 opens**, compared with **894 opens** for the test group.
- The control group's open rate was approximately **18%**.
- The test group's open rate was approximately **19%**.
- The test group had a higher open rate than the control group.
- According to the workbook's significance analysis, the difference was statistically significant at **98% certainty**.
- Despite the statistically significant improvement, the test group's approximately 19% open rate did **not reach H&M's target of 20%**.

## Recommendation
Based on the results of this test, I would not recommend immediately adopting the new subject line as the standard for H&M's promotional emails.

Although the test subject line produced a statistically significant improvement in open rate, it achieved an open rate of approximately **19%**, which remained below H&M's target of **20%**.

A better approach would be to continue testing alternative subject lines while using the current results as a benchmark for future experiments.

## Business Implications
Email open rate is an important early indicator of customer engagement, but a higher open rate does not necessarily translate into higher sales.

For a more complete evaluation of the subject line, additional metrics should be analyzed, including:
- Click-through rate
- Purchase conversion rate
- Revenue
- Average order value
- Unsubscribe rate
- Spam complaint rate

For example, if the new subject line increased opens but resulted in fewer purchases or lower revenue, the higher open rate alone would not indicate improved business performance.

Future A/B tests should therefore evaluate both email engagement and downstream customer behavior.

## Excel Techniques Used
- PivotTables
- A/B testing
- Hypothesis testing
- Sample-size analysis
- Conversion-rate calculations
- Statistical significance analysis
- Data aggregation
- Business interpretation
- Experimental design
- Confounding-factor analysis

## Excel Workbook
[H&M A/B Testing Email Marketing Campaign Analysis](hm-ab-testing-analysis.xlsx)

## Project Context
This project was completed as part of the Global Career Accelerator Data Analytics program.

The project simulated a real-world marketing analytics scenario in which an analyst evaluates an email A/B test and determines whether a new promotional subject line should be adopted.
