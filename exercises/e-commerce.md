# E-commerce Orders & Sales
## Subject / story
“Build a pipeline to track orders, revenue, and delivery performance for an e-commerce company.”
## Data source options
NYC / global style e-commerce datasets on GitHub/Kaggle (various order-level datasets). Example: a GitHub repo containing multiple e-commerce sample datasets (products, prices, etc.). 
Source: https://github.com/luminati-io/eCommerce-dataset-samples?utm_source=chatgpt.com
## Suggested Activities
    •	Create a medallion architecture:
      o	Bronze: read from source and store the raw files.
      o	Silver: read from raw files stored in bronze and split into dimensions and fact tables.
      o	Golden: read from silver tables and create some tables ready for dashboards.
    •	The pipeline should allow incremental load.
    •	The bronze layer should store all files from previous extractions.
    •	Identify all possible dimensions on data (orders, order_items, customers, payments, reviews).
    •	Normalize and clean data.
    •	On gold create the following marts:
      o	Sales by month / product / category.
      o	Delivery performance (promised vs actual delivery date).
      o	Customer cohort retention.
