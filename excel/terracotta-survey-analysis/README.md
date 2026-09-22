# Terracotta Survey Analysis

## Overview
This project analyzes customer survey data for Terracotta, a plant retailer, to understand customer purchasing preferences and identify opportunities to improve marketing and online plant sales.

The analysis combines survey responses with plant-care information and categorized free-response data to identify the types of plants customers purchase most frequently, the factors they consider when choosing plants, and the information Terracotta should emphasize in its marketing.

The project was completed in Excel as part of the Global Career Accelerator Data Analytics program.

## Business Questions
This analysis addresses three primary questions:
1. Which types of plants are most frequently purchased by customers?
2. Are there factors in choosing a plant that are consistently important to customers?
3. What information should Terracotta advertise to boost sales?

A LevelUp analysis also examines whether purchasing frequency is associated with differences in what customers value when choosing plants.

## Data
The workbook contains **217 customer survey responses**.

The analysis combines three primary sources of information:

### Customer Survey Responses
Survey responses include:
- Survey ID
- Plant type typically purchased
- Reason for purchasing a plant
- Plant purchase frequency
- Desired plant-care information
- Preferred planter/container type

### Plant Information
The `plant-info` sheet provides information about different plants, including:
- Plant type
- Light requirements
- Water requirements
- Maintenance requirements
- Pet and child safety

### Free-Response Analysis
The `free-response-analysis` sheet contains customer responses to the question:
> "What factor is most important to you when choosing a plant to buy?"

Each free-response answer was assigned to a broader category by a senior analyst.

The categories include:
- Care requirements
- Pet-friendly or safe for children
- Benefits
- Rare or unique species
- Size
- Price

## Analysis

### 1. Plant Purchase Preferences
I used XLOOKUP to connect customer survey responses with the plant information table.

The analysis added:
- Maintenance requirements
- Pet and child safety
to each survey response based on the plant type selected by the customer.

I then used PivotTables to examine the distribution of plant maintenance levels among customer purchases.

The results showed that **low-maintenance plants were the most frequently purchased maintenance category**.

### 2. Maintenance Preferences
The maintenance-level analysis showed:

| Maintenance Level | Responses | Share |
|---|---:|---:|
| Low-maintenance | 172 | 79.26% |
| Medium-maintenance | 34 | 15.67% |
| High-maintenance | 11 | 5.07% |
| **Total** | **217** | **100%** |

Low-maintenance plants accounted for approximately **79.26% of survey responses**.

### 3. Pet and Child Safety
I used XLOOKUP to identify whether each customer's selected plant was classified as safe for pets and children.

The results showed:

| Plant Safety Classification | Share |
|---|---:|
| Safe for pets & children | 99.54% |
| Toxic | 0.46% |

Approximately **99.54% of survey responses** listed plants classified as safe for pets and children.

### 4. Reasons for Purchase
I used XLOOKUP to match each survey response with its categorized reason for purchasing a plant.

A PivotTable was then used to count and rank the categories.

| Purchase Factor | Responses | Share |
|---|---:|---:|
| Care requirements | 58 | 26.73% |
| Pet-friendly or safe for children | 56 | 25.81% |
| Benefits | 41 | 18.89% |
| Rare or unique species | 27 | 12.44% |
| Size | 24 | 11.06% |
| Price | 11 | 5.07% |
| **Total** | **217** | **100%** |

The two most frequently selected factors were **care requirements (26.73%)** and **pet-friendly or child-safe characteristics (25.81%)**.

### 5. Desired Plant-Care Information
The survey also asked customers what plant-care information they would like to see provided in-store or online.

The responses included:
- Pet-safe information
- Light requirements
- Watering frequency & amount
- Propagation techniques
- Soil type & fertilization

The most requested information was **pet-safe information**, followed by **light requirements** and **watering frequency & amount**.

### 6. Customer Segmentation by Purchase Frequency
As a LevelUp analysis, I used a PivotTable to examine whether customers who purchase plants more frequently value different characteristics than occasional buyers.

Purchase-frequency groups included:
- Weekly
- Monthly
- Every few months
- Once a year
- Rarely, only for special occasions

I then displayed purchase-factor results as a percentage of each frequency group's total responses.

The analysis found differences in the relative importance of purchase factors across customer-frequency groups.

For example:
- Among weekly buyers, **care requirements** represented 27.27% of responses.
- Among monthly buyers, **pet-friendly or safe for children** represented 27.12%.
- Among customers who purchase once a year, **pet-friendly or safe for children** represented 50%.
- Among customers who purchase every few months, **care requirements** represented 31.11%.

These differences suggest that customer needs may vary depending on how frequently they purchase plants.

## Key Findings
- The survey contains **217 customer responses**.
- **Low-maintenance plants** were the most frequently purchased maintenance category, representing **79.26%** of responses.
- **Chinese Evergreen** was the most frequently selected individual plant type, with **27 responses**.
- **Peperomia** and **Cast-Iron Plant** were the next most frequently selected plant types, with **23 responses each**.
- Approximately **99.54%** of selected plants were classified as safe for pets and children.
- **Care requirements** were the most frequently cited factor when choosing a plant, representing **26.73%** of responses.
- **Pet-friendly or child-safe characteristics** were the second most common factor at **25.81%**.
- **Benefits** represented **18.89%** of responses.
- **Price** was the least frequently selected purchase factor at **5.07%**.
- Pet-safe information was the most frequently requested type of plant-care information.
- The relative importance of purchase factors varied across customer purchase-frequency groups.

## Recommendation
Based on the survey results, Terracotta should make it easy for customers to find plants that fit their lifestyle and care preferences.

### 1. Highlight Low-Maintenance Plants
Since **79.26%** of responses identified low-maintenance plants as the most frequently purchased maintenance category, Terracotta could prominently feature low-maintenance plants in its online store and marketing materials.

### 2. Make Care Requirements Easy to Find
Because **26.73%** of customers identified care requirements as the most important factor when choosing a plant, Terracotta could provide clear filters and product information for:
- Maintenance level
- Light requirements
- Watering requirements
- Other care needs

### 3. Highlight Pet and Child Safety
Pet-friendly and child-safe characteristics represented **25.81%** of the most important purchase factors.

Terracotta could create a dedicated "Pet-Friendly & Child-Safe" collection and make safety information highly visible on individual product pages.

### 4. Provide Educational Content
The survey indicates demand for practical plant-care information, particularly information about pet safety, lighting, and watering.

Terracotta could incorporate this information into product descriptions, buying guides, FAQs, and educational content.

### 5. Consider Customer Segments
The LevelUp analysis suggests that purchase factors vary across customers with different purchasing frequencies.

Terracotta could consider tailoring recommendations and marketing content to different customer groups rather than presenting every customer with the same information.

## Business Implications
The survey suggests that customers place greater emphasis on plant care and safety than on price when choosing plants.

This creates opportunities for Terracotta to differentiate its online shopping experience through:
- Care-based product filters
- Pet- and child-safety labels
- Detailed care guides
- Personalized plant recommendations
- Low-maintenance plant collections
- Educational content

These findings are based on survey responses and describe the preferences represented in this dataset. They should not necessarily be generalized to all Terracotta customers without additional survey data or a larger representative sample.

## Excel Techniques Used
- XLOOKUP
- PivotTables
- Data categorization
- Percentage calculations
- Sorting
- Survey analysis
- Categorical data analysis
- Customer segmentation
- Data enrichment
- Data-driven recommendations

## Excel Workbook
[Terracotta Survey Analysis](terracotta-survey-analysis.xlsx)

## Project Context
This project was completed as part of the Global Career Accelerator Data Analytics program.

The project simulated a customer survey analysis scenario for Terracotta, requiring the use of Excel to combine survey responses with plant information, categorize qualitative responses, identify customer preferences, segment customers by purchase frequency, and develop a data-driven marketing recommendation.
