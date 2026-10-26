# HR Analytics Dashboard using Power BI

## 📌 Project Overview

The **HR Analytics Dashboard** is an interactive Business Intelligence project developed using Microsoft Power BI to analyze employee data and generate actionable insights into workforce composition, employee attrition, salary distribution, job roles, tenure, and performance ratings.

The dashboard transforms raw HR data into meaningful visual insights, helping users understand workforce patterns and supporting data-driven Human Resource Management (HRM) decisions.

## 🎯 Project Objectives

- Analyze the overall workforce and active employee population.
- Measure employee attrition count and attrition rate.
- Evaluate employee distribution across departments, job roles, and genders.
- Analyze monthly income across departments and age groups.
- Explore employee tenure and performance rating patterns.
- Develop interactive KPI cards and visualizations for HR reporting.

## 🛠️ Tools & Technologies

- **Microsoft Power BI** — Dashboard development and data visualization
- **DAX (Data Analysis Expressions)** — KPI calculations and analytical measures
- **Microsoft Excel** — HR dataset and source data
- **Data Analytics** — Workforce analysis and insight generation
- **Business Intelligence** — Interactive reporting and decision support

## 📊 Dashboard Features

### 1. Key Performance Indicators (KPIs)

The dashboard includes KPI cards for:

- Total Employees
- Active Employees
- Attrition Count
- Attrition Rate (%)
- Average Monthly Salary
- Total Monthly Income

An additional Active Employee Rate (%) measure can be used to monitor the proportion of employees currently active.

### 2. Employee Distribution Analysis

- Employee Count by Job Role
- Employee Count by Gender
- Department-wise workforce distribution

### 3. Salary Analysis

- Department-wise Monthly Income
- Age-wise Monthly Income

### 4. Workforce Analysis

- Employee Tenure by Gender
- Performance Rating by Age

### 5. Interactive Filtering

The dashboard uses slicers for:

- Gender
- Job Role
- Department

An Attrition Status slicer can also be added to support more detailed analysis.

## 📈 Key Insights

Based on the dataset used in this project:

- **Total Employees:** 250
- **Active Employees:** 204
- **Employees Who Left:** 46
- **Overall Attrition Rate:** 18.4%

The dashboard provides a consolidated view of workforce composition, employee exits, salary distribution, and employee performance patterns.

These findings describe the supplied dataset and should not be interpreted as industry-wide HR benchmarks.

## 🧮 DAX Measures

Example: Total Employees

```dax
Total Employees =
DISTINCTCOUNT('HR_Analytics'[Employee_ID])
```

Example: Active Employees

```dax
Active Employees =
CALCULATE(
    DISTINCTCOUNT('HR_Analytics'[Employee_ID]),
    'HR_Analytics'[Attrition] = "Active"
)
```

Example: Attrition Rate

```dax
Attrition Rate % =
DIVIDE(
    [Attrition Count],
    [Total Employees],
    0
)
```

*Note: Replace `HR_Analytics` with the actual table name in your Power BI model if it differs.*

## 💡 Skills Demonstrated

- Power BI Dashboard Development
- DAX Measures and KPI Calculation
- Data Visualization
- Workforce and Attrition Analysis
- Salary and Employee Distribution Analysis
- Interactive Report Design
- Business Intelligence and Analytical Thinking

## 📂 Project Files

Suggested repository structure:

```text
HR-Analytics-Dashboard-PowerBI/
│
├── README.md
├── hr_analytics_dataset.xlsx
├── HR_Analytics_Dashboard.pbix
└── images/
    └── dashboard_screenshot.png
```

Add the actual project files and dashboard screenshot to the repository using these filenames or update the structure to match your files.

## 🚀 How to Explore the Project

1. Download or clone this repository.
2. Open `HR_Analytics_Dashboard.pbix` using Microsoft Power BI Desktop.
3. Ensure the Excel dataset is accessible and update the data source path if required.
4. Refresh the dataset if necessary.
5. Explore KPI cards, charts, and slicers to analyze the HR data.

## 🔮 Future Enhancements

- Add attrition analysis by department and job role.
- Develop a dedicated employee attrition analysis page.
- Improve age-group and performance-rating comparisons.
- Add further workforce KPIs and advanced DAX measures.
- Enhance the dashboard with additional analytical insights.

## 👩‍💻 Author

**Prajna Mondal**

Aspiring Data Analyst | Power BI | SQL | Python | Data Visualization

🎥 **Project Walkthrough:** Watch the video demonstration of my HR Analytics Dashboard on LinkedIn: https://lnkd.in/p/dbPZMnRw

## ⭐ Conclusion

This project demonstrates the application of Power BI and DAX in developing an interactive HR Analytics Dashboard. It highlights how workforce data can be transformed into structured visual reports to improve HR reporting, identify employee attrition patterns, and support data-driven decision-making.

If you find this project useful, feel free to explore the repository and share your feedback.
