# Exploratory Data Analysis (EDA) on Sales Data

## Overview

This project aims to analyze a sales dataset to uncover trends, seasonal patterns, and key performance metrics. The goal is to identify factors affecting sales performance, including top-performing products, regions, and sales trends over time.

## Steps Performed

### 1. Importing Necessary Libraries

To begin the analysis, essential Python libraries were imported:

- `pandas` for data manipulation
- `numpy` for numerical operations
- `matplotlib` and `seaborn` for data visualization

### 2. Loading the Dataset

The dataset was loaded into a Pandas DataFrame. The first five (`head()`) and last five (`tail()`) rows were inspected to understand the structure of the data.

### 3. Checking Dataset Information

The following checks were performed:

- Total number of rows and columns using `.shape`
- Data types of each column using `.info()`
- Presence of missing values using `.isnull().sum()`

### 4. Handling Missing Data

It was found that some columns contained missing values:

- **Columns with 89%, 52%, 2%, and 38% missing data** were either dropped or filled based on their importance.
- Missing values were imputed using **mean, median, or mode**, depending on the data type.

### 5. Handling Duplicates and Data Type Conversion

- Duplicate records were checked and removed.
- The `OrderDate` column was converted from **object** type to **datetime** format.
- The `Year` column did not reflect actual years, so it was corrected.

### 6. Identifying and Handling Outliers

- Outliers were detected in the `Sales` column using statistical methods.
- These were handled appropriately to ensure meaningful analysis.

### 7. Statistical Analysis

- Descriptive statistics were computed for both continuous and categorical data.
- Correlation analysis was performed between `Sales` and other numerical variables.

## Exploratory Data Analysis (EDA)

### **i) Univariate Analysis**

- **Histogram Analysis:** The `DealSize` column contained three categories: **Small, Medium, and Large**. It was observed that **Medium DealSize was the most preferred.**
- **Pie Chart Analysis:** The `Status` column analysis showed that the **Shipped mode had the highest performance.**

### **ii) Bivariate Analysis**

- **Bar Chart Analysis:**
  - Large DealSize had the **highest number of sales.**
  - Most sales were in **On Hold status mode.**
  - **2005 had the highest sales** compared to other years.
  - The highest quantity of orders was placed in **Shipped mode.**

### **iii) Multivariate Analysis**

- **Sales vs Status vs DealSize:** It was observed that in **Shipped mode, Medium DealSize performed the best.**
- **Status vs DealSize vs Quantity Ordered:** Again, in **Shipped mode, Medium DealSize showed the highest performance.**

## **Key Insights & Findings**

### **1. Sales Trends & Seasonal Patterns**

- **Sales have decreased over the years.**
- **Quantity ordered has also decreased over time.**
- **California (CA) had the highest sales among all states.**
- **The USA had the highest number of quantities ordered.**
- **88% of total sales belonged to the EMEA (Europe, Middle East, and Africa) territory region.**

## **Conclusion**

This exploratory data analysis provided valuable insights into sales trends, regional performance, and product demand. The analysis helps in understanding key areas where businesses can focus on improving sales and inventory management.

---

### 📌 **Next Steps**

- Perform **predictive modeling** to forecast future sales trends.
- Implement **customer segmentation** to improve marketing strategies.
- Optimize **inventory management** based on sales trends and demand fluctuations.

**📊 Tools Used:** Python, Pandas, Matplotlib, Seaborn, Jupyter Notebook.

---

### **🔗 References & Credits**

This project was developed for educational purposes in data analysis and visualization.

---

### **📬 Connect with Me**

If you have any questions or suggestions, feel free to reach out!
