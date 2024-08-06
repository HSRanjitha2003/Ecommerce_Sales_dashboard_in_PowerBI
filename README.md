# Ecommerce_Sales_dashboard_in_PowerBI
Goal : Main goal is to create a power bi dashboard to help Madhav to understand and analyse trends in their online sales.

Creating an E-Commerce Sales Dashboard in Power BI: 
Step 1: Importing the Data

1. Load Data from CSV:
   - Open Power BI Desktop.
   - Go to the "Home" tab and select "Get Data."
   - Choose "CSV" from the list of data sources.
   - Navigate to the location of your CSV file, select it, and click "Open."
   - Power BI will preview the data. Click "Load" to import the data into Power BI.

Step 2: Data Cleaning and Transformation

1. Change Data Types:
   - Click on "Transform Data" to open Power Query Editor.
   - Review each column and adjust the data types as necessary. For example, change columns that should contain dates from "Text" to "Date" format.

2. Group Data:
   - Select the column or columns by which you want to group data.
   - Use the "Group By" function to aggregate data. For instance, you can group sales data by month and region to get monthly sales totals.

3. Remove Duplicates:
   - In the Power Query Editor, select the columns where duplicates might exist.
   - Click "Remove Rows" and then select "Remove Duplicates" to ensure each row is unique based on the selected columns.

4. Handle Missing Values:
   - Identify missing or null values in your dataset.
   - Use "Replace Values" to substitute missing values with appropriate data or "Remove Rows" to eliminate rows with missing values if they are not crucial.

Step 3: Data Modeling

1. Define Relationships:
   - Switch to the "Model" view by clicking on the "Model" icon on the left sidebar.
   - If you have multiple tables, drag and drop to create relationships between tables based on common fields (e.g., Order ID, Customer ID).
   - Set the relationship types (e.g., one-to-many) and configure any additional settings such as cardinality.

Step 4: Data Cleaning Enhancements

1. Apply Conditional Formatting:
   - Select a visual or table where you want to apply conditional formatting.
   - Use the "Format" pane to set rules that highlight key metrics or outliers, such as highlighting sales values that exceed a certain threshold.

2. Use Format Painter:
   - To ensure visual consistency, select a well-formatted visual.
   - Use the "Format Painter" tool to copy the formatting and apply it to other visuals.

3. Verify Data in Data View:
   - Switch to "Data View" to see a table-like representation of your data.
   - Verify that data is clean and accurately transformed by reviewing the values and types.

Step 5: Creating Measures

1. Write DAX Formulas:
   - Go to the "Model" view or "Data" view and select the table where you want to add measures.
   - Click on "New Measure" and write DAX (Data Analysis Expressions) formulas to create metrics such as:
     - Total Sales: Total Sales = SUM(Sales[Amount])`
     - Total Orders: Total Orders = COUNT(Sales[OrderID])`
     -  Order Value:`Average Order Value = AVERAGE(Sales[OrderValue])`

Step 6: Designing the Dashboard

1. Add and Configure Visuals:
   - Drag and drop visuals such as bar charts, line charts, pie charts, and tables onto the report canvas.
   - Use the "Visualizations" pane to select different chart types and drag relevant fields into the "Values," "Axis," and "Legend" areas.

2. Customize Visuals:
   - Use the "Format" pane to adjust the appearance of your visuals. Customize colors, labels, titles, and other visual elements to improve clarity and aesthetics.

Step 7: Adding Filters and Slicers**

1. Add Slicers:
   - Drag and drop the "Slicer" visual onto the report canvas.
   - Add fields such as "Quarter" and "Region" to the slicer to allow users to filter data dynamically.

2. Configure Filters:
   - Open the "Filters" pane to add filters at different levels: visual, page, or report.
   - Set up filter criteria to enable users to view specific subsets of data based on their selection.

Conclusion

This dashboard will help visualize key sales metrics, track performance, and provide insights into your e-commerce business. Ensure that your data is clean, relationships are well-defined, and visuals are tailored to your reporting needs for the most effective dashboard.
