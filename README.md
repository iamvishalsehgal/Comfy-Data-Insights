# Comfy Data Analysis Project

## Overview
This project analyzes data from Comfy.ua, a Ukrainian electronics retailer, to assess data quality and tackle two key business challenges: transitioning to a marketplace model and launching an electronics rental service.

## Data Description
The analysis is based on two datasets (Data - Anonymised):
- **Client Dataset (411K records):** Includes client IDs, registration dates, gender, age, number of receipts, and total revenue.
- **Transaction Dataset (2.6M records):** Covers receipts, sale vs. return, channels, platforms, credit transactions, revenue, quantity, businesses, categories, brands, cities, and regions.

## Data Quality Assessment
Key findings from the data quality assessment:
- **Client Dataset:**
  - Gender: 94% missing
  - Age: 66% blank or invalid
  - Outliers in number of receipts (3%) and total revenue (1.1%)
- **Transaction Dataset:**
  - 621,261 duplicate receipts
  - Revenue: 0.9% missing, 1.9% negative, 15.4% outliers
  - Quantity: 1.9% negative values
  - Platforms: 67.5% blank, inconsistent data

### Recommended Actions
- Clean gender, age, and platform fields
- Investigate and resolve duplicate receipts
- Validate revenue and quantity data
- Enrich demographics via surveys or third-party data
- Improve data collection for consistency

## Business Challenges
### 1. Transition to a Marketplace Model
**Approach:**
- Segment customers using RFM analysis and K-means clustering
- Identify underserved categories with demand gap analysis
- Find complementary products via market basket analysis
- Analyze regional sales for localized partnerships
- Develop pricing strategies based on elasticity and competitors

**Goal:** Create a marketplace targeting tech-savvy urban consumers and third-party sellers.

### 2. Launching an Electronics Rental Service
**Approach:**
- Select durable, high-revenue products with Pareto analysis
- Estimate device lifespans using survival analysis
- Target urban millennials with logistic regression
- Integrate with the loyalty program
- Use tiered pricing based on depreciation rates

**Goal:** Launch a flexible rental program for high-end electronics to boost engagement.

## Integration of External Data
Recommended external sources:
- Competitor pricing (e.g., Rozetka)
- Industry depreciation rates (e.g., Gartner, IDC)
- Social media sentiment (e.g., Google/Apple Maps APIs)
- Macroeconomic indicators (e.g., Ukraine’s State Statistics Service)

These enhance insights into market gaps, pricing, preferences, and regional priorities.

## Methodology
Techniques used:
- **Data Quality:** Statistical profiling for missing values, duplicates, and outliers
- **Segmentation:** RFM and K-means clustering
- **Demand Analysis:** Gaps identified via market trends
- **Association:** Market basket analysis for product links
- **Lifespan:** Survival analysis for rental devices
- **Targeting:** Logistic regression for customer predictions

## Tools Used
- Python for analysis and visualization
- Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

## Code
The Python code and detailed descriptions are in the `notebooks` directory of this repository.

## Conclusion
This project highlights Comfy’s data quality issues and offers data-driven strategies for a marketplace transition and rental service launch. Implementing these recommendations and leveraging external data will improve data reliability and support scalable business growth.