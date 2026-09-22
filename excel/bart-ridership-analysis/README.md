# BART Ridership Analysis

## Overview
This project analyzes 2021 BART ridership data to understand passenger volume across weekdays and weekends, evaluate the role of the Yellow Line, and examine ridership at downtown San Francisco stations.

The analysis uses Excel feature engineering, conditional aggregation, and descriptive metrics to identify patterns in passenger volume and translate those findings into recommendations for service scheduling and station prioritization.

The project was completed as part of the Global Career Accelerator Data Analytics program.

## Business Questions
This analysis addresses several questions:
- How many passengers used BART in 2021?
- How does ridership differ between weekdays and weekends?
- What proportion of passengers traveled on the Yellow Line?
- What does the weekday/weekend ridership difference suggest about commuter behavior?
- What additional data would help evaluate the Yellow Line's impact on system efficiency and rider experience?
- How does ridership at downtown San Francisco stations compare with non-downtown stations?

## Data
The dataset contains BART station exit data collected throughout **2021**.

Each record includes:
- Date
- Station Code
- Lines
- Total Passengers

The dataset also includes a station-code reference that maps station codes to station names.

Additional variables were created in Excel to support the analysis:
- Month
- Day of Week
- First Letter of Line Code
- Yellow Line classification
- Downtown station classification

## Analysis

### 1. Feature Engineering
I created several calculated columns to prepare the dataset for analysis.

**Month**

Used the `MONTH()` function to extract the month from each date.

**Day of Week**

Used the `WEEKDAY()` function with Monday represented as 1 and Sunday as 7.

**First Letter**

Used the `LEFT()` function to extract the first character from the BART line code.

This was used to identify whether a station was associated with the Yellow Line.

**Yellow Line**

Created a classification using an `IF()` statement:
- `Yes` = Station is on the Yellow Line
- `No` = Station is not on the Yellow Line

### 2. Overall Ridership
I used the `SUM()` function to calculate total BART ridership across the dataset.

Total passenger volume in 2021 was:

**24,583,309 passengers**

This serves as the baseline ridership metric for the analysis.

### 3. Weekday vs. Weekend Ridership
I used `SUMIF()` to calculate total passenger volume for weekdays and weekends.

| Ridership Period | Passengers | Share of Total |
|---|---:|---:|
| Weekdays | 20,281,852 | 82.5% |
| Weekends | 4,301,457 | 17.5% |
| **Total** | **24,583,309** | **100%** |

The large difference between weekday and weekend ridership indicates that BART usage was substantially concentrated on weekdays during the analyzed period.

### 4. Yellow Line Ridership
I used the engineered `FirstLetter` field with `SUMIF()` to calculate passenger volume associated with the Yellow Line.

Yellow Line passenger volume was:

**19,425,399 passengers**

This represented approximately:

**79.0% of total passenger volume**

The analysis therefore identifies the Yellow Line as a major component of the passenger volume represented in the dataset.

### 5. Data-Driven Service Considerations
The weekday/weekend difference suggests that BART could consider adjusting service levels according to demand.

For weekdays, the analysis recommends considering:
- Higher train frequency during peak commuting periods
- Additional capacity in high-demand areas
- Reliable service and reduced delays
- Coordination with major businesses and connecting transit systems

For weekends, potential considerations include:
- Adjusting service during consistently lower-demand periods
- Increasing service around major events
- Scheduling maintenance during lower-demand periods
- Promoting BART for leisure and recreational travel

These recommendations are based on the ridership patterns identified in the dataset and would require additional operational data before specific scheduling changes could be evaluated.

## Yellow Line Analysis
Because the Yellow Line accounts for a large proportion of passenger volume in the dataset, additional information would be useful for evaluating its impact on the overall BART system.

Useful additional data would include:
- Ridership by station
- Ridership by time of day
- Train occupancy
- Crowding levels
- On-time performance
- Delays
- Customer satisfaction
- Station-level capacity
- Train frequency

This information could help determine whether high passenger volume is concentrated at particular stations or times and whether additional service capacity is needed.

For example, consistently high demand could support increasing train frequency or capacity, while lower demand during certain periods could support reallocating service to higher-demand areas.

## Downtown Ridership Analysis
As an optional LevelUp analysis, I classified four San Francisco stations as downtown stations:
- Embarcadero (EM)
- Montgomery Street (MT)
- Powell Street (PL)
- Civic Center (CC)

I then used `SUMIF()` to calculate passenger volume through these stations.

Downtown stations accounted for:

**6,932,181 passengers**

This represented approximately:

**28.2% of total passenger volume**

Therefore, non-downtown stations accounted for approximately **71.8%** of total passenger volume.

| Station Group | Share of Total Ridership |
|---|---:|
| Downtown stations | 28.2% |
| Non-downtown stations | 71.8% |

Although non-downtown stations account for a larger share of total passenger volume, the downtown stations represent only four stations. This makes the downtown stations important locations to evaluate in terms of passenger concentration, capacity, and service reliability.

## Key Findings
- BART recorded **24,583,309 passengers** across the analyzed 2021 data.
- **82.5%** of passenger volume occurred on weekdays.
- **17.5%** of passenger volume occurred on weekends.
- The Yellow Line accounted for approximately **79.0%** of total passenger volume in the dataset.
- Downtown San Francisco stations accounted for approximately **28.2%** of total passenger volume.
- Non-downtown stations accounted for approximately **71.8%** of total passenger volume.
- The large difference between weekday and weekend ridership indicates substantially higher weekday demand.
- The high share of passenger volume associated with the Yellow Line makes additional operational and rider-experience data important for evaluating service decisions.

## Recommendations

### Adjust Service Based on Weekday and Weekend Demand
The substantial difference between weekday and weekend ridership suggests that service planning should account for different demand patterns throughout the week.

Weekday service could prioritize capacity and reliability during periods of high demand, while weekend service could be adjusted based on lower baseline demand and increased around major events.

### Evaluate Yellow Line Performance With Additional Data
Because the Yellow Line represents approximately 79.0% of passenger volume in the dataset, BART could combine ridership data with train occupancy, station-level demand, delays, and customer satisfaction data.

This would provide a more complete picture of whether Yellow Line service is appropriately matched to demand.

### Prioritize High-Volume Stations
The downtown stations represent approximately 28.2% of total passenger volume despite consisting of only four stations.

BART could use station-level ridership and crowding data to identify where additional capacity, staffing, maintenance, or passenger-information resources would have the greatest operational value.

## Excel Techniques Used
- Excel Tables
- Feature engineering
- `MONTH()`
- `WEEKDAY()`
- `LEFT()`
- `IF()`
- `SUM()`
- `SUMIF()`
- Percentage calculations
- Conditional classification
- Data aggregation
- Descriptive analysis
- Data-driven recommendations

# Excel Workbook
[Bart Ridership Analysis](bart-ridership-analysis.xlsx)

## Project Context
This project was completed as part of the Global Career Accelerator Data Analytics program.

The project focused on using Excel to transform raw transit data, calculate key ridership metrics, identify patterns in passenger behavior, and translate those findings into operational considerations for BART.
