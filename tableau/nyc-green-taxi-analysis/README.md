# NYC Green Taxi Fares Analysis

## Overview
This project analyzes NYC Green Taxi trip data from 2015 to identify patterns in fares, trip distances, rate types, and tipping behavior. The analysis uses Tableau to explore how trip characteristics and payment behavior vary across different types of taxi trips.

The project was completed in Tableau as part of the Global Career Accelerator Data Analytics program.

## Business Question
How do fare amounts, trip distances, rate types, and tipping behavior vary across NYC Green Taxi trips, and what insights can be used to inform pricing and service strategies?

## Data
The analysis uses 2015 NYC Green Taxi trip data.

Key variables include:
- Rate type
- Rate code
- Fare amount
- Trip distance
- Tip amount
- Payment type
- Extra charges
- MTA tax
- Improvement surcharge
- Toll amount

The dataset provides information about individual taxi trips, allowing pricing and customer payment behavior to be analyzed.

## Analysis
I created Tableau visualizations to examine fare distributions, rate types, trip distances, and tipping behavior.

Key analysis included:
- Creating a histogram of fare amounts to examine the distribution of taxi fares
- Comparing the number of trips across different rate types
- Examining trip distances across rate types
- Creating calculated fields to translate numerical rate codes into meaningful rate categories
- Categorizing payment types using calculated fields
- Calculating the total fare subtotal from fare and additional charges
- Calculating tip per distance to compare tipping behavior across trips
- Creating calculated fields and bins to identify patterns in fare and tip amounts
- Comparing tipping behavior across different rate types

## Key Findings
### Fare Distribution
The fare distribution shows that most NYC Green Taxi trips fall within the lower fare ranges, while a smaller number of trips have substantially higher fares.

A noticeable concentration of trips occurs around the $52–$54 range, which may reflect particular common trip types or standardized/high-distance routes within the dataset.

### Rate Types
The analysis shows that Standard Rate trips account for a large portion of the trips in the dataset, while other rate categories represent more specialized trip types.

Examining trip counts alongside trip distances helps distinguish the characteristics of different rate categories.

### Trip Distance
Trip distance varies across rate types. Comparing distance distributions provides insight into how different types of trips contribute to overall taxi usage and fare generation.

### Tipping Behavior
The analysis uses tip per distance to compare tipping behavior while accounting for differences in trip length. This provides a more meaningful comparison than looking only at total tip amounts.

## Visualizations
- [Fare Histogram](images/fare-histogram.png)
- [Trip Count By Rate Type](images/trip-count-by-rate-type.png)
- [Trip Distance By Rate Type](images/trip-distance-by-rate-type.png)
- [Tip By Rate Type](images/tip-by-rate-type.png)
- [Tip-Subtotal Ratio Histogram](images/tip-subtotal-ratio-histogram.png)

## Interactive Dashboard
[View the interactive visualization on Tableau Public](https://public.tableau.com/views/Milestone-NYCGreenTaxiFaresAnalysis--AnanyaGarg/WriteAnswersHere?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Tools & Skills
- Tableau
- Data visualization
- Calculated fields
- Histograms
- Data aggregation
- Data categorization
- Binning
- Comparative analysis
- Pricing analysis
- Customer behavior analysis
- Interactive visualizations

## Project Context
This project was completed as part of the Global Career Accelerator Data Analytics program. The analysis was developed from the perspective of a data analyst working with NYC Green Taxi data to understand pricing, trip patterns, and customer tipping behavior.
