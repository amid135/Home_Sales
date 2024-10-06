# Home_Sales
Home_Sales Project
Overview
The Home_Sales project uses PySpark to analyze home sales data, allowing for the extraction of key metrics and insights from the dataset. This project demonstrates the use of Spark SQL to perform various queries and operations on home sales data, including caching, partitioning, and performance measurement.

Files
- Home_Sales.ipynb: Jupyter Notebook containing the code for reading, processing, and analyzing the home sales data.
- home_sales_revised.csv: CSV file containing the home sales dataset.

Steps
The following steps outline the analysis performed in the project:
- Load Data: Read the home_sales_revised.csv file into a Spark DataFrame.
- Create Temporary Table: Create a temporary SQL table named home_sales from the DataFrame.
- SQL Queries:
  - Calculate the average price for four-bedroom houses sold each year.
  - Calculate the average price of three-bedroom, three-bathroom homes for each year built.
  - Calculate the average price of three-bedroom, three-bathroom, two-floor homes that are at least 2,000 square feet for each year built.
  - Calculate the average price of homes per "view" rating for homes with an average price greater than or equal to $350,000 and measure runtime.
- Caching: Cache the home_sales temporary table and verify the cache status.
- Run Cached Query: Run the previous query using the cached table and compare runtimes.
- Partitioning: Partition the home sales dataset by the "date_built" field and create a parquet table.
- Query on Parquet Table: Run the last query on the parquet table and measure runtime.
- Uncache Table: Uncache the home_sales temporary table and verify that it has been uncached.

Key Metrics
- Average price for four-bedroom homes sold each year.
- Average price of homes with specific features and conditions.
- Performance improvements from caching and partitioning.
