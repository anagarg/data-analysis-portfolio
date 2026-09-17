# Investigating UFO Sightings

## Overview
This project analyzes reported UFO sightings to identify patterns in sighting locations, encounter duration, time of day, reported shapes, and geographic distribution. The analysis uses Tableau to transform and visualize UFO reporting data and uncover trends across countries and U.S. states.

The project was completed in Tableau as part of the Global Career Accelerator Data Analytics program.

## Business Question
What patterns can be identified in reported UFO sightings based on location, time, encounter duration, and reported UFO shape?

## Data
The analysis uses UFO sighting records containing information about:
- Location
- Date and time of sighting
- Reported UFO shape
- Encounter duration
- Description of the sighting
- Date documented
- Latitude and longitude

The dataset contains both geographic and descriptive information, allowing sightings to be analyzed across multiple dimensions.

## Data Preparation
Before creating the visualizations, I used Tableau calculated fields to clean and standardize several variables.

Key transformations included:
- Extracting country and state information from the location field
- Converting UFO shape values to a consistent uppercase format
- Converting descriptions to lowercase for text-based analysis
- Converting encounter duration from seconds to minutes
- Standardizing location and categorical values for analysis
- Extracting information from free-text descriptions to identify reported colors

These transformations made the dataset more consistent and easier to analyze.

## Analysis
I created Tableau visualizations to examine UFO sightings across geographic, temporal, and categorical dimensions.

Key analysis included:
- Comparing the number of reported sightings across countries
- Examining the distribution of sightings across U.S. states
- Analyzing sightings by hour of the day
- Identifying the most frequently reported UFO shapes
- Examining how encounter duration varies by month
- Using calculated fields to transform and categorize raw data
- Exploring geographic patterns in reported sightings

## Key Findings

### Geographic Distribution
The United States accounts for a substantial portion of the reported sightings in the dataset. Among U.S. states, California, Florida, and Texas had the highest numbers of reported sightings.

The concentration of reports in these states provides a useful starting point for exploring geographic differences in reporting frequency.

### UFO Shapes
The dataset contains a wide variety of reported UFO shapes. Some shapes occur considerably more frequently than others, allowing the most commonly reported forms to be identified through the visualization.

### Time of Day
Reported sightings vary throughout the day. Analyzing sightings by hour provides insight into when reports are most frequently made and helps identify periods with particularly high reporting activity.

### Encounter Duration
Encounter duration varies substantially between reports. Converting the original duration measurements from seconds to minutes made it easier to compare the length of reported encounters across months.

## Visualizations
[UFO Sightings By State](images/ufo-sightings-by-state.png)

[Number of Sightings Per Country](images/number-of-sightings-per-country.png)

[UFO Sightings Length By Month](images/ufo-sightings-length-by-month.png)

[UFO Sightings By Shape](images/ufo-sightings-by-shape.png)

[UFO Sightings By Hour](images/ufo-sightings-by-hour.png)

[UFO Sightings By Color](images/ufo-sightings-by-color.png)

## Interactive Dashboard
[View the interactive visualization on Tableau Public](https://public.tableau.com/views/Milestone-InvestigatingUFOSightings--AnanyaGarg/WriteAnswersHere?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Tools & Skills
- Tableau
- Data visualization
- Calculated fields
- Data cleaning and transformation
- Geographic analysis
- Time-series analysis
- Text manipulation
- Categorical analysis
- Data aggregation
- Interactive visualizations
- Pattern analysis

## Project Context
This project was completed as part of the Global Career Accelerator Data Analytics program. The analysis focused on transforming and visualizing UFO reporting data to identify geographic, temporal, and categorical patterns in reported sightings.
