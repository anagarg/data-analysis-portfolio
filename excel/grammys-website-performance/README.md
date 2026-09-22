# Grammys Website Performance Analysis

## Overview
This project analyzes website performance data for GRAMMY.com and The Recording Academy to evaluate how separating the two websites affected user engagement.

The analysis uses website traffic, engagement, device, and A/B testing data to compare website performance before and after the February 2022 website split. The project was completed in Excel as part of the Global Career Accelerator Data Analytics program.

## Business Question
Did separating GRAMMY.com and The Recording Academy's website improve user engagement, and should the organization continue using a split website structure?

## Data
The workbook contains several datasets related to website activity.

### GRAMMY.com Website Data
The GRAMMY.com dataset contains daily website activity, including:
- Date
- Visitors
- Pageviews
- Sessions
- Bounced sessions
- Average session duration
- Event type
- Website content
- Mobile visitors

The data covers website activity before and after the February 1, 2022 transition, when GRAMMY.com began focusing on GRAMMY content rather than combining GRAMMY and Recording Academy content.

### Recording Academy Website Data
The Recording Academy dataset contains daily website analytics after the websites were separated, including:
- Date
- Year
- Visitors
- Pageviews
- Sessions
- Bounced sessions
- Average session duration

### A/B Test Data
The workbook also contains an A/B test comparing visitors who experienced the original combined website with visitors who experienced the split website structure.

The test measured engagement with a homepage call-to-action (CTA) encouraging visitors to watch highlights from the 64th GRAMMY Awards.

## Analysis

### 1. Website Traffic Analysis
I created a [line chart](images/number_of_daily_visitors.png) to examine daily visitors to GRAMMY.com and identify periods of increased website traffic.

The analysis showed that the largest traffic spikes occurred around GRAMMY Awards ceremonies. Smaller recurring spikes appeared around the announcement of GRAMMY nominations, while additional increases occurred during the months following the awards.

I also created a PivotTable comparing average daily visitors on GRAMMY Awards days with regular days:
| Grammy Awards Days | Regular Days | Total |
| -------- | -------- | -------- |
| 1389590 | 32388 | 39922 |

### 2. Website Engagement Metrics
I calculated three key engagement metrics to compare website performance before and after the split:

**Pages per Session**

Calculated as:

`Total Pageviews / Total Sessions`

**Bounce Rate**

Calculated as:

`Total Bounced Sessions / Total Sessions`

**Average Time on Site**

Calculated as the average of the `avg_session_duration_secs` field.

These metrics were used to evaluate how visitor behavior changed after the websites were separated.

### 3. Mobile Visitor Analysis
I used the XLOOKUP function to match mobile visitor data to the corresponding dates in the main GRAMMY.com dataset.

I then calculated the percentage of visitors using mobile devices by dividing total mobile visitors by total visitors.

### 4. A/B Testing
I analyzed a controlled A/B test comparing:
- **Control group:** Visitors who experienced the original combined website
- **Test group:** Visitors who experienced the split website structure

I created a PivotTable to compare the number of visitors and CTA clicks in each group and evaluated the results using the workbook's A/B testing significance calculator.

The test included:
- 3,797 control-group visitors
- 4,099 test-group visitors
- 119 CTA clicks in the control group
- 158 CTA clicks in the test group

The test group had 39 more CTA clicks despite having 302 more visitors.

## Key Findings

### Website Traffic
- GRAMMY.com experienced its largest traffic spikes around GRAMMY Awards ceremonies.
- Smaller recurring spikes occurred around GRAMMY nomination announcements.
- Traffic also remained elevated during portions of the months following major award events.

### Engagement Before and After the Website Split

| Metric | Combined GRAMMY + Recording Academy | GRAMMY.com After Split | Recording Academy After Split |
|---|---:|---:|---:|
| Pages per Session | 1.86 | 2.25 | 2.78 |
| Bounce Rate | 41.6% | 40.2% | 33.7% |
| Average Time on Site | 102.85 sec | 82.99 sec | 128.50 sec |

The Recording Academy website showed higher pages per session, a lower bounce rate, and a higher average time on site compared with the combined website.

GRAMMY.com also had higher pages per session and a slightly lower bounce rate after the split, although its average time on site decreased.

The largest change among the three engagement metrics was pages per session, particularly for the Recording Academy website, where it increased from 1.86 to 2.78 pages.

### Mobile Usage
Approximately **73.7% of visitors** in the analyzed GRAMMY.com data accessed the website using a mobile device.

This highlights the importance of considering mobile usability when evaluating website engagement.

### A/B Test
The test group had a higher CTA conversion rate than the control group.

According to the workbook's A/B testing analysis:
- The test group converted **23% better** than the control group.
- The results reached **96% certainty** according to the workbook's significance calculator.
- The workbook identifies the result as **statistically significant**.

## Business Recommendation
Based on the engagement analysis and A/B test results, the analysis supports continuing with the split website structure while continuing to improve how the two websites work together.

The Recording Academy website showed improvements across the measured engagement metrics after the split. The GRAMMY.com website also showed an increase in pages per session and a small decrease in bounce rate, although average time on site decreased.

The A/B test additionally showed a higher CTA conversion rate for visitors who experienced the split website structure.

The analysis also suggests opportunities for continued optimization, particularly for mobile users, who represented approximately 73.7% of visitors in the analyzed data.

However, these engagement metrics do not measure broader business outcomes such as membership growth, donations, ticket sales, newsletter sign-ups, or other conversions. Incorporating these metrics into future analysis would provide a more complete assessment of the long-term impact of the website structure.

## Excel Techniques Used
- PivotTables
- XLOOKUP
- SUMIFS
- AVERAGEIFS
- IF statements
- Calculated metrics
- Line charts
- Data comparison
- A/B testing
- Statistical significance analysis
- Data interpretation
- Business recommendations

## Visualizations
[Number of daily visitors to the website on a given day](images/number_of_daily_visitors.png)

## Excel Workbook
[Analyzing Website Performance for The Grammys](grammys-website-performance-analysis.xlsx)

## Project Context
This project was completed as part of the Global Career Accelerator Data Analytics program.

The project simulated a real-world website analytics scenario for The Recording Academy, requiring analysis of website traffic and engagement data, Excel-based data manipulation, A/B testing, and a final business recommendation.
