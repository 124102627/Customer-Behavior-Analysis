
# Customer Trends Analysis

## Project Overview
This project analyses customer shopping behaviour using Python, PostgreSQL, and Power BI. It explores 3,900 customer records to understand purchasing patterns, customer segments, subscription behaviour, and product performance.

The workflow covers data cleaning, feature engineering, SQL analysis, and an interactive dashboard to communicate customer insights.

## Tools and Technologies
- Python and Pandas — data inspection, cleaning, and transformation.
- PostgreSQL and SQL — data storage and business analysis.
- Power BI — interactive dashboard development and data visualisation.
- Jupyter Notebook — developing and documenting the Python workflow.
- SQLAlchemy — connecting Python to PostgreSQL and loading the prepared dataset.

## Dataset
The dataset contains customer demographics, purchase details, and shopping preferences, including:

- Age, gender, and location.
- Product category and item purchased.
- Purchase amount and previous purchases.
- Review ratings and subscription status.
- Shipping type and payment method.
- Discount usage and purchase frequency.

## Data Preparation
The Python notebook prepares the dataset for analysis by:

- Inspecting data types, summary statistics, and missing values.
- Filling missing review ratings using category-level median values.
- Standardising column names for SQL compatibility.
- Creating age-group and purchase-frequency features.
- Removing a redundant promotional field.
- Loading the cleaned dataset into PostgreSQL.

## SQL Analysis
The SQL script explores business questions such as:

- How does revenue vary across customer demographics?
- Do subscribers and non-subscribers have different spending patterns?
- Which products receive the highest average review ratings?
- Which products have the highest proportion of discounted purchases?
- What are the most-purchased products within each category?
- How do purchase amounts compare across shipping options?
- How much revenue does each age group contribute?

The queries use aggregations, subqueries, common table expressions (CTEs), CASE statements, and window functions.

## Customer Segmentation
Customers are classified using their previous purchase history:

- New — 1 previous purchase.
- Returning — 2 to 10 previous purchases.
- Loyal — more than 10 previous purchases.

These project-defined segments support comparisons between customers with different purchasing histories.

## Power BI Dashboard
The Customer Behaviour Dashboard provides an overview of:

- Total number of customers.
- Average purchase amount.
- Average review rating.
- Subscriber and non-subscriber distribution.
- Revenue by product category.
- Revenue comparisons across age groups.

Interactive filters allow users to explore the data by subscription status, gender, product category, and shipping type.

## Repository Contents
- Jupyter Notebook (.ipynb) — data inspection, cleaning, feature engineering, and database export.
- SQL script (.sql) — queries exploring customer behaviour and product performance.
- Customer dataset (.csv) — source data used for the analysis.
- Dashboard screenshot — preview of the Power BI dashboard.

## How to Run
1. Download or clone the repository.
2. Install the required Python packages:
   `pip install pandas sqlalchemy psycopg2-binary jupyter`
3. Open the notebook in Jupyter and update the CSV file path.
4. Configure your local PostgreSQL connection. Keep database credentials out of version control.
5. Run the notebook to prepare and load the data.
6. Execute the SQL script against the prepared `customer` table.

The dashboard screenshot provides a visual preview. Editing or refreshing the report requires the Power BI report file.

## Skills Demonstrated
- Data cleaning and preparation.
- Exploratory data analysis.
- Feature engineering.
- SQL querying and database integration.
- Customer segmentation.
- Power BI dashboard development.
- Data visualisation and storytelling.

