# Coffee-Sales-EXcel-Dashboard
An interactive Excel dashboard for analyzing coffee sales trends, customer insights, and product performance.

## **Overview**
The **Coffee Sales Dashboard** is an interactive Excel-based dashboard designed to analyze and visualize coffee sales data. It provides insights into sales trends, customer behavior, and product performance using pivot tables, slicers, and charts. This project demonstrates data cleaning, transformation, and visualization techniques in Excel.

## **Data Sources**
The dashboard is built using the following datasets:

1. **Orders Dataset:** Contains transactional data related to coffee sales, including order details, customer information, and product details.
2. **Customers Dataset:** Includes customer information such as names, emails, phone numbers, addresses, and loyalty program status.
3. **Products Dataset:** Lists coffee products with details like type, roast level, size, price, and profit margins.

## **Data Processing Steps**
### **1. Data Cleaning & Formatting:**
   - Retrieved missing values using **XLOOKUP** and other Excel formulas.
   - Formatted dates correctly and displayed sales values in currency format.
   - Removed duplicate entries.

### **2. Data Transformation:**
   - Computed sales revenue using formulas:  
     **`=L2 * E2`** (Unit Price × Quantity)
   - Ensured relevant data types were used for accuracy in calculations.

### **3. Data Analysis & Visualization:**
   - Created pivot tables to analyze sales trends.
   - Developed an interactive dashboard with slicers and charts.

## **Excel Formulas Used**
- **XLOOKUP:** To retrieve customer and product details:
  ```excel
  =XLOOKUP(C2, customers!$A$2:$A$1001, customers!$B$2:$B$1001, "", 0)
  ```
  ```excel
  =XLOOKUP(D2, products!$A$2:$A$49, products!$B$2:$B$49, "", 0)
  ```

- **Sales Calculation:**
  ```excel
  =L2 * E2
  ```

- **Removing Errors:**
  ```excel
  =IFERROR(XLOOKUP(C2, customers!$A$2:$A$1001, customers!$B$2:$B$1001, "", 0), "Not Found")
  ```

## **Dashboard Features**
The dashboard includes the following visual elements:

1. **Month and Year Slicer:** Enables users to filter data by specific time periods.
2. **Coffee Type Slicer:** Allows filtering sales by coffee type.
3. **Roast Type Slicer:** Filters data based on roast type (Light, Medium, Dark).
4. **Total Sales by Coffee Type (Stacked Bar Chart):** Displays yearly sales distribution across different coffee types.
5. **Total Sales by Country (Bar Chart):** Provides insights into geographic sales distribution.
6. **Top 5 Customers (Bar Chart):** Highlights the highest-spending customers.

## **Tools & Techniques Used**
- **Excel Formulas:** XLOOKUP, SUM, COUNT, IFERROR, etc.
- **Pivot Tables & Pivot Charts**
- **Data Cleaning & Formatting**
- **Interactive Slicers & Filters**
- **Currency & Date Formatting**

## **Conclusion**
The Coffee Sales Dashboard effectively visualizes sales performance, helping businesses track trends, identify top-performing products, and analyze customer purchases. This project demonstrates the power of Excel in business intelligence and sales analysis.

---
**Author:** [Your Name]  
**Date:** [Project Completion Date]

