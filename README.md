WAVE-X Project (Watercfaft)

Project-Specific Requirements:
1. Exclude data from the year 2018
2. Exclude sales data from discontinued product WR3
3. Create a sales forecast for the next two years
   
The project has completed through the following multiple stages of the Power BI process, which are:

Data Discovery

Import Data

Data Transformation

Data Modeling and DAX

Creating Visualizations & Reports

# How to do a project with Power BI
Creating a project with Power BI involves several steps, including data collection, data cleaning, data analysis, and visualization. Below is a step-by-step guide to help you create a simple Power BI project, for instance, a sales dashboard.

### Step-by-Step Guide to Create a Power BI Project

#### Step 1: Data Collection

For this example, let's assume you have a CSV file containing sales data. The CSV file might have columns like `Date`, `Product`, `Category`, `Sales`, `Quantity`, and `Region`.

#### Step 2: Load Data into Power BI

1. **Open Power BI Desktop.**
2. **Get Data:**
   - Click on `Home` -> `Get Data` -> `Text/CSV`.
   - Browse and select your CSV file.
   - Click `Load` to import the data.

#### Step 3: Data Cleaning and Transformation

1. **Open Power Query Editor:**
   - Click on `Transform Data` to open Power Query Editor.

2. **Basic Data Cleaning:**
   - **Remove unnecessary columns**: Right-click on the column header and select `Remove`.
   - **Rename columns**: Double-click the column header to rename it.
   - **Change data types**: Click on the column header and choose the appropriate data type from the `Data Type` dropdown.
   - **Handle missing values**: Use the `Replace Values` option to handle missing data or remove rows/columns with missing data.

3. **Add Calculated Columns:**
   - You can add new columns for more detailed analysis. For example, you might want a `Revenue` column calculated as `Quantity * Sales`.
   - Click `Add Column` -> `Custom Column`, and define the formula.

4. **Close and Apply:**
   - Once the data is clean, click `Close & Apply` to apply the changes and load the data into Power BI.

#### Step 4: Creating Visualizations

1. **Select Visualization Type:**
   - Click on a blank area on the report canvas.
   - Choose a visualization type from the `Visualizations` pane (e.g., Bar Chart, Line Chart, Pie Chart, etc.).

2. **Add Data to Visualizations:**
   - Drag and drop fields from the `Fields` pane to the appropriate area in the `Visualizations` pane (e.g., Axis, Values, Legend).

3. **Create Multiple Visuals:**
   - Add multiple visuals to your report by repeating the steps above. Each visual can represent different aspects of your data.

4. **Example Visualizations:**
   - **Bar Chart**: To show total sales by product.
   - **Line Chart**: To show sales trends over time.
   - **Pie Chart**: To show the sales distribution by category.
   - **Map**: To show sales by region.

#### Step 5: Create Interactive Dashboards

1. **Add Slicers:**
   - Slicers allow users to filter the data on the dashboard. For example, you can add slicers for `Date`, `Product`, `Category`, or `Region`.
   - Click on `Slicer` from the `Visualizations` pane and drag the desired field into it.

2. **Interactivity:**
   - Power BI visuals are interactive by default. Clicking on a part of one visual will filter the other visuals on the report page.

3. **Format Visuals:**
   - Customize the appearance of your visuals using the `Format` pane. You can change colors, add data labels, adjust titles, and more.

#### Step 6: Publish and Share

1. **Sign in to Power BI Service:**
   - Click `File` -> `Publish` -> `Publish to Power BI`.
   - Sign in with your Power BI account.

2. **Publish the Report:**
   - Select a workspace to publish your report to.
   - Once published, go to `https://app.powerbi.com` to view and share your report.

3. **Share the Dashboard:**
   - In Power BI Service, you can share the dashboard with others by clicking on `Share` and entering their email addresses.

### Example Project: Sales Dashboard

Here’s a brief example project outline for a Sales Dashboard:

1. **Data Source:**
   - Sales data CSV file with columns: `Date`, `Product`, `Category`, `Sales`, `Quantity`, `Region`.

2. **Visualizations:**
   - **Total Sales by Product**: Bar Chart
   - **Monthly Sales Trends**: Line Chart
   - **Sales Distribution by Category**: Pie Chart
   - **Sales by Region**: Map
   - **Top Products**: Table

3. **Interactivity:**
   - Add slicers for `Date`, `Product`, `Category`, and `Region`.

4. **Customization:**
   - Customize visuals for clarity and aesthetics. Add titles, data labels, and adjust colors.

5. **Publish and Share:**
   - Publish the dashboard to Power BI Service and share it with stakeholders.

### Summary

Power BI is a powerful tool for data visualization and analysis. By following the steps above, you can create insightful and interactive dashboards that help in making data-driven decisions. This example provides a basic framework, but Power BI offers much more functionality, including DAX (Data Analysis Expressions) for

more advanced calculations, custom visuals, and integration with various data sources.

### Advanced Features to Explore

1. **DAX (Data Analysis Expressions):**
   - Learn to write DAX formulas for more complex calculations and measures.
   - Example: Create a calculated measure for year-over-year growth:
     ```DAX
     YoY Growth = 
     CALCULATE(
         SUM(Sales[Amount]),
         DATEADD(Date[Date], -1, YEAR)
     ) / SUM(Sales[Amount]) - 1
     ```

2. **Custom Visuals:**
   - Explore the Power BI Marketplace to find and integrate custom visuals that suit your specific needs.
   - Example: Use a custom Gantt chart for project management data.

3. **Power Query Advanced Transformations:**
   - Dive deeper into Power Query for more complex data transformations like pivoting, unpivoting, and merging queries.
   - Example: Combine multiple CSV files from a folder into a single dataset.

4. **Row-Level Security (RLS):**
   - Implement RLS to restrict data access for different users based on roles.
   - Example: Sales managers can only see data for their respective regions.

5. **Integration with Other Data Sources:**
   - Connect Power BI to various data sources like SQL Server, Azure, SharePoint, and APIs.
   - Example: Pull live data from a SQL Server database for real-time reporting.

### Example: Advanced Sales Dashboard

**Data Source:**
   - SQL Server database with tables for `Sales`, `Products`, `Regions`, and `Dates`.

**Visualizations:**
   - **Sales Overview**: KPI cards showing total sales, total orders, and average order value.
   - **Sales Trends**: Line chart showing monthly sales trends.
   - **Product Performance**: Bar chart showing sales by product category.
   - **Regional Sales**: Map visualization showing sales by region.
   - **Sales Funnel**: Funnel chart showing the sales pipeline stages.
   - **Customer Segmentation**: Pie chart showing sales distribution by customer segment.

**Advanced Features:**
   - **DAX Measures**: Custom measures for YOY growth, average sales per customer, etc.
   - **Dynamic Date Filtering**: Slicers for selecting specific date ranges.
   - **Custom Visuals**: Use of Gantt charts and heatmaps for more insightful data representation.
   - **Drill-Throughs and Tooltips**: Enable drill-through functionality to navigate from summary views to detailed reports.

**Interactivity:**
   - Use bookmarks and buttons to create interactive navigation experiences.
   - Configure slicers and filters for dynamic data exploration.

**Publishing and Sharing:**
   - Publish the report to Power BI Service and embed it in a SharePoint page or an intranet site.
   - Schedule data refreshes to ensure the dashboard displays the latest data.

### Summary

Creating a project with Power BI involves collecting and cleaning data, creating interactive visualizations, and sharing insights. Power BI offers a range of advanced features that allow for complex data analysis and interactive reporting. By leveraging these tools, you can build comprehensive dashboards that provide valuable insights and aid in data-driven decision-making.
