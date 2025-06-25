# Online Retail Data Analysis

## Introduction
This notebook performs an exploratory data analysis on an online retail dataset. It aims to uncover insights related to sales patterns, item returns, and categorization based on transaction amounts.

## Dataset
The dataset comprises transactional data from an online retail store, detailing customer purchases, dates, and item details.

## Analysis Performed

### 1. Data Loading and Initial Inspection
- **Load Data**: Imported the dataset into the environment.
- **Initial Checks**: Performed descriptive statistics analysis, identified null values, and detected duplicates.

### 2. Data Cleaning
- Removed duplicate rows to maintain data integrity.
- Discarded rows containing missing `CustomerID`.

### 3. Feature Engineering
- **TotalAmount Calculation**: Computed as `Quantity * UnitPrice`.
- **Date Handling**: Converted `InvoiceDate` into datetime objects.
- **Extracted Date Features**: Derived `Year`, `Month`, `Day`, `Quarter`, and `Semester` from `InvoiceDate`.

### 4. Sales Analysis
- **Total Sales Calculation**:
  - Analyzed sales totals by year, quarter, semester, and month.
- **Return Analysis**: Identified and categorized returned items where `Quantity` is negative.

### 5. Sales Category Analysis
- Divided sales into categories: 'Low', 'Medium', and 'High', based on `TotalAmount`.

### 6. Visualization
- **Item Sale vs. Returns**: Pie chart illustrating proportions.
- **Sales by Amount Category**: Pie chart depicting distribution across categories.
- **Monthly Sales Trends**: Bar chart visualizing sales by month.
- **Top-Selling Items**: Horizontal bar chart showcasing the top 10 items by `Quantity` sold.

## Key Findings
- Significant missing values existed in the `CustomerID` and `Description` columns.
- Returned items were flagged by negative quantities.
- **Seasonality in Sales**: Marked peak in November.
- Predominance in 'Low' amount category for transactions.
- Top-selling items by quantity were effectively highlighted.

## Code Structure
The notebook execution follows a structured approach in distinct segments:

1. **Data Loading and Initial Checks**: Setting the groundwork and quality assessment.
2. **Data Cleaning**: Ensuring data reliability and consistency.
3. **Feature Creation**: Enhancing dataset with new, insightful metrics.
4. **Sales Analysis**: Dissecting sales over various time frames.
5. **Return Analysis**: Examining item return dynamics.
6. **Sales Categorization**: Classifying transactions by value.
7. **Visual Representation**: Translating findings into visual insights.

## How to Use
1. Ensure you have the `online_retail.csv` file accessible in your directory.
2. Update the `file_path` in the first code cell as needed.
3. Execute the cells sequentially to reproduce and explore the analysis.

---

Please feel free to contribute, provide feedback, or collaborate to further enhance this project. For inquiries, connect through the project's issues section or contact me directly at [your email].
