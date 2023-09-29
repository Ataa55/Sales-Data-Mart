# Sales-Data-Mart
designing a sales data mart based on AdventureWorks data base 
Overview
This GitHub repository contains the documentation for a Sales Data Mart project. The project's goal is to create a data mart from the Adventure Works database, including fact tables for sales data and dimension tables for products, customers, time, and territories. This project is based on the dimensional modeling approach, and it includes data extraction, transformation, and loading (ETL) processes.

Data Model:
The data mart is designed with the following dimensional model:

Fact Sales: Contains sales-related measures and foreign keys to dimensions.

Dim Product: Stores product information with attributes like product name, category, and subcategory.

Dim Customer: Contains customer details and supports slowly changing dimension (SCD) processing for customer changes.

Dim Time: Represents time-related information such as date, month, quarter, and year.

Dim Territory: Stores territory information with attributes like region, country, and state.

![SalesMart_StarSchema](https://github.com/Ataa55/Sales-Data-Mart/assets/115408306/8bf6f1f1-aad6-4f96-8c20-f9e36c21321a)

ETL Process:
1. Dim Product Design
Extract product data from the source database.
Transform and cleanse product attributes (e.g., name, category, subcategory).
Load the Dim Product table.

![Dim_Product](https://github.com/Ataa55/Sales-Data-Mart/assets/115408306/d71578d3-f6d1-419a-a92f-2c39d60bc118)

2. Dim Customer Design
Extract customer data from the source database.
Apply Slowly Changing Dimension (SCD) processing to handle customer changes.
Transform and cleanse customer attributes (e.g., name, address).
Load the Dim Customer table.

![Dim_Customer](https://github.com/Ataa55/Sales-Data-Mart/assets/115408306/f8811e05-d965-4132-9843-223bf0f53ee7)

3. Dim Territory Design
Extract territory data from the source database.
Transform and cleanse territory attributes (e.g., region, country, state).
Load the Dim Territory table.

![Dim_Terittory](https://github.com/Ataa55/Sales-Data-Mart/assets/115408306/a8a58304-2af0-4276-9267-8d04ba21f030)

Finally: populate the fact table 
Fact Sales Design
Extract sales-related data from the source database.
Perform necessary transformations on the data (e.g., calculate measures, apply business rules).
Ensure that foreign keys to dimension tables are appropriately mapped.
Load the Fact Sales table with sales measures and dimension keys.

![Fact_Sales](https://github.com/Ataa55/Sales-Data-Mart/assets/115408306/5c907209-c486-4f8c-8dff-bcc9966da769)

Here is the the overall control flow:

![Control_Flow](https://github.com/Ataa55/Sales-Data-Mart/assets/115408306/6e574464-9d68-46ff-a762-030c19cea66a)















