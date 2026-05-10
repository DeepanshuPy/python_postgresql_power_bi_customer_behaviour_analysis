# Customer Shopping Behaviour Analysis

## Project Overview
This end-to-end data analytics project analyzes customer shopping behavior using transactional data from 3,900 purchases across various product categories. The primary goal is to uncover insights into spending patterns, customer segments, product preferences, and subscription behavior to guide strategic business decisions.

## Tech Stack
* **Language:** Python (Pandas for EDA and Data Cleaning)
* **Database:** PostgreSQL (Structured Data Analysis)
* **Visualization:** Power BI (Interactive Dashboarding)

## Dataset Summary
* **Transactions:** 3,900 rows
* **Features:** 18 columns including Customer ID, Age, Gender, Item Purchased, Category, Purchase Amount, Location, Subscription Status, and Review Rating.
* **Data Health:** Handled 37 missing values in the `Review Rating` column via category-based median imputation.

## Project Workflow

### 1. Data Cleaning & Preparation (Python)
* **Initial Exploration:** Performed summary statistics and structure checks.
* **Standardization:** Renamed columns to `snake_case` for consistency.
* **Feature Engineering:** * Created `age_group` bins.
    * Derived `purchase_frequency_days`.
* **Database Integration:** Connected the cleaned data to a PostgreSQL instance for advanced querying.

### 2. Business Analysis (PostgreSQL)
Key insights extracted through SQL queries include:
* **Revenue by Gender:** Male customers contributed significantly higher revenue ($157,890) compared to Female customers ($75,191).
* **Customer Segmentation:** Classified the user base into **Loyal** (3,116), **Returning** (701), and **New** (83) segments.
* **Subscription Metrics:** While non-subscribers drive the bulk of total revenue ($170,436), subscribers show consistent average spending (~$59.49).
* **Product Performance:** Identified 'Gloves' as the top-rated product (3.86 avg rating) and 'Jewelry' as the top-selling item in the Accessories category.

### 3. Data Visualization (Power BI)
Developed an interactive **Customer Behaviour Dashboard** featuring:
* KPI cards for Total Customers (3.9K), Avg Purchase Amount ($59.76), and Avg Review Rating (3.75).
* Revenue and Sales distribution by Category and Age Group.
* Slicers for Gender, Subscription Status, and Shipping Type for deep-dive analysis.

## Key Business Recommendations
1.  **Boost Subscriptions:** Implement exclusive benefit programs to increase the current 27% subscription rate.
2.  **Loyalty Programs:** Focus on the "Returning" segment to transition them into "Loyal" customers.
3.  **Targeted Marketing:** Prioritize high-revenue age groups (Young Adults) and users preferring Express Shipping.
4.  **Product Positioning:** Leverage high-rated items like Gloves and Sandals in promotional campaigns.

## Author
**Deepanshupy**
