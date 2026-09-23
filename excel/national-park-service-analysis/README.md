# National Park Service Analysis

## Overview
This project analyzes 2024 National Park Service visitation data to support a promotional campaign focused on National Park Service sites in Washington state.

The analysis begins with nationwide visitation patterns before narrowing the focus to Washington. It examines the most visited sites, overnight camping activity, and how Washington's National Parks compare with National Parks across the United States.

The project was completed in Excel as part of the Global Career Accelerator Data Analytics program.

## Business Questions
The analysis addresses four main questions:
1. How popular are National Park Service sites across the country?
2. Which sites in Washington state attract the most visitors?
3. How do visitors experience Washington's sites?
4. Are Washington's National Parks more popular compared to National Parks across the country?

## Data
The dataset contains **398 National Park Service sites** and includes 2024 visitation and camping information.

Key variables include:
- Site Name
- Site Type
- Region
- State
- Recreation Visits
- Tent Campers
- RV Campers
- Backcountry Campers

### Site Types
The dataset includes multiple types of National Park Service sites, including:
- National Parks
- National Recreation Areas
- National Historical Parks
- National Historic Sites
- National Monuments
- Other National Park Service designations

### Data Definitions
**Recreation Visits** represents total recreational visits in 2024.

**Tent Campers**, **RV Campers**, and **Backcountry Campers** represent overnight stays in each camping category.

## Analysis
### 1. National Park Service Sites Across the Country
I first analyzed the complete dataset to establish a nationwide baseline.

The dataset contains:
- **398 National Park Service sites**
- **331,863,358 total recreation visits**
- **833,828 average recreation visits per site**

The nationwide analysis provides context for evaluating Washington's sites.

### 2. Most Visited Sites in Washington
I filtered the dataset to Washington state and sorted sites by Recreation Visits.

Washington contains **10 National Park Service sites** in the dataset, receiving a combined:

**9,003,899 recreation visits in 2024.**

The three most visited sites were:

| Rank | Site | Recreation Visits |
|---|---|---:|
| 1 | Olympic NP | 3,717,267 |
| 2 | Mount Rainier NP | 1,620,006 |
| 3 | Lake Roosevelt NRA | 1,091,489 |

These three sites accounted for a substantial share of Washington's total recreation visits.

### 3. Washington Site Visitation
Washington's 10 sites vary considerably in visitation.

The most visited site was **Olympic NP**, with more than 3.7 million recreation visits.

Other highly visited sites included:
- Mount Rainier NP
- Lake Roosevelt NRA
- Fort Vancouver NHS
- Ross Lake NRA

North Cascades NP had substantially fewer recreation visits than the other National Parks in Washington in this dataset.

This variation suggests that promotional materials could highlight both Washington's highly visited destinations and lesser-visited sites.

### 4. Overnight Camping
I analyzed three categories of overnight camping in Washington:
- Tent camping
- RV camping
- Backcountry camping

Washington sites recorded:

| Camping Type | Overnight Stays |
|---|---:|
| Tent Campers | 285,893 |
| RV Campers | 202,503 |
| Backcountry Campers | 212,996 |

Together, these categories accounted for **701,392 overnight camping stays**.

Compared with Washington's 9,003,899 recreation visits, camping stays represented approximately **7.8%** of the recreation-visit total.

Because recreation visits and overnight stays are different measures, this percentage should be interpreted as a comparison of the dataset's reported counts rather than the percentage of individual visitors who camped.

## National Parks: Washington vs. the United States
The final analysis focuses specifically on sites classified as **National Parks**, rather than all National Park Service site types.

### Nationwide National Parks
The dataset contains:
- **63 National Parks**
- Average 2024 recreation visits: **1,496,628 per National Park**

### Washington National Parks
Washington contains:
- **3 National Parks**
- Average 2024 recreation visits: **1,784,586 per National Park**

The Washington National Parks in the dataset are:
- Olympic NP
- Mount Rainier NP
- North Cascades NP

### Comparison
The average Washington National Park received approximately **1.78 million recreation visits**, compared with approximately **1.50 million** for National Parks nationwide.

The workbook therefore concludes that:
> National Parks in Washington state receive more visitors than the average National Park in the United States.

## Key Findings
- The dataset contains **398 National Park Service sites**.
- These sites received approximately **331.9 million recreation visits in 2024**.
- The average site received approximately **833,828 recreation visits**.
- Washington contains **10 National Park Service sites** in the dataset.
- Washington's sites received approximately **9.0 million recreation visits** in 2024.
- **Olympic NP** was the most visited Washington site with **3,717,267 visits**.
- **Mount Rainier NP** was the second-most visited Washington site with **1,620,006 visits**.
- **Lake Roosevelt NRA** was the third-most visited Washington site with **1,091,489 visits**.
- Washington recorded **285,893 tent-camping stays**, **202,503 RV stays**, and **212,996 backcountry stays**.
- The three camping categories totaled **701,392 overnight stays**.
- There are **63 National Parks** in the dataset.
- Washington has **3 National Parks**.
- Washington's National Parks averaged approximately **1.78 million visits**, compared with approximately **1.50 million** nationwide.

## Business Implications
The analysis provides several useful insights for a Washington-focused promotional campaign.

### Highlight High-Visitation Destinations
Olympic NP and Mount Rainier NP attract substantial visitation and could serve as prominent destinations in promotional materials.

### Showcase Different Types of Experiences
Washington's sites include National Parks, National Recreation Areas, and National Historical Sites. Promotional materials can therefore highlight different types of outdoor and historical experiences rather than focusing exclusively on National Parks.

### Promote Overnight Experiences
The camping analysis shows substantial activity across tent, RV, and backcountry camping. These categories could be incorporated into promotional materials aimed at visitors interested in overnight experiences.

### Consider Lesser-Visited Sites
The large differences in visitation between Washington sites also identify opportunities to promote sites that receive fewer visitors.

## Excel Techniques Used
- Excel Tables
- Filtering
- Sorting
- COUNTIF
- COUNTIFS
- SUM
- SUMIF
- AVERAGE
- AVERAGEIF
- AVERAGEIFS
- Conditional analysis
- Data aggregation
- Comparative analysis
- Regional analysis
- Data-driven business recommendations

## Excel Workbook
[National Park Service Analysis](national-park-service-analysis.xlsx)

## Project Context
This project was completed as part of the Global Career Accelerator Data Analytics program.

The project simulated a data analyst assignment for the National Park Service, with the goal of analyzing visitation patterns and creating insights for a promotional campaign focused on Washington state.
