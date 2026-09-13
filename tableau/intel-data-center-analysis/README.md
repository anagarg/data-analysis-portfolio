# Intel Data Center Analysis

## Overview
This project analyzes regional electricity generation, energy demand, and renewable energy availability to identify a suitable location for a new Intel data center. The analysis was completed in Tableau as part of the Global Career Accelerator Data Analytics program.

## Business Question
Which U.S. region would be the strongest location for a new Intel data center based on energy production, demand, and renewable energy availability?

## Data
The analysis uses energy generation and demand data organized by region, time period, and energy source.

Key variables include:
- Region
- Energy demand
- Net generation
- Coal generation
- Natural gas generation
- Nuclear generation
- Wind generation
- Solar generation
- Hydropower and pumped storage
- Other fuel sources
- Local time

## Analysis
I created interactive Tableau visualizations to compare energy production and renewable energy availability across regions.

Key analysis included:
- Calculating Net Production as net generation minus demand
- Calculating total Renewable Energy from wind, solar, and hydropower
- Calculating the percentage of overall generation from renewable sources
- Comparing energy production by region and energy source
- Examining supply and demand patterns over time
- Analyzing hourly changes in energy generation
- Using a Tableau parameter to switch between day, week, and month periods
- Creating an interactive dashboard with regional and energy-source filters

## Key Findings
* The Mid-Atlantic, Northwest, Southwest, Central, and Southeast regions were identified as net producers.
* The Northwest had the highest percentage of renewable energy generation at 52.25%.
* The Northwest was the second-largest region in net energy production at approximately 21.7 MW.
* The Northwest and Central regions were both net producers and among the top three regions by renewable energy percentage.
* The Northwest's energy demand closely matched, and sometimes exceeded, its net generation during parts of the year.
* California's wind generation showed substantial hourly variation, with the analysis identifying hours 12–22 as a period of increasing wind generation.

## Recommendation
Based on the visualizations, I would recommend the Northwest as the location for the next Intel data center. The Northwest combines relatively high net energy production with the highest percentage of renewable energy generation among the regions analyzed. This combination makes it a strong candidate for supporting Intel's energy needs while also aligning with sustainability goals. A potential concern is that the Northwest's demand closely matches or sometimes exceeds its net generation during certain periods. This should be considered in any further site-selection analysis.

## Dashboard
Main Dashboard

Net Production

Renewable Energy

Supply and Demand

## Tools & Skills
* Tableau
* Data visualization
* Interactive dashboards
* Calculated fields
* Parameters
* Filters
* Time-series analysis
* Comparative analysis
* Business-focused data analysis
* Data-driven recommendations

## Project Context
This project was completed as part of the Global Career Accelerator Data Analytics program. The project was developed around a data center planning scenario involving Intel's sustainability considerations.
