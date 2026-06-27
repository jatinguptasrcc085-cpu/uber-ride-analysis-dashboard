# 🚖 Uber Ride Analytics Dashboard | Power BI

## 📊 Overview

The Uber Ride Analytics Dashboard is an end-to-end Business Intelligence solution developed in Power BI to monitor ride performance, revenue generation, customer satisfaction, and operational efficiency across multiple vehicle categories.

The dashboard transforms raw ride-booking data into actionable insights through interactive visualizations, KPI tracking, and dynamic filtering capabilities, enabling stakeholders to make informed business decisions regarding fleet utilization, customer experience, and revenue optimization.

---

## Dashboard Preview

<img width="1126" height="645" alt="image" src="https://github.com/user-attachments/assets/394de0c9-8cde-4642-8ba0-86981bd800ab" />


---

## 🎯Business Objective

Ride-sharing platforms generate massive volumes of operational data daily. The primary objective of this project was to design a centralized analytics solution capable of answering critical business questions:

* Which vehicle categories contribute the most to overall revenue?
* What proportion of bookings are successfully completed versus lost?
* Which locations generate the highest ride demand?
* How do booking patterns fluctuate throughout the year?
* How satisfied are customers and drivers across different service categories?
* What operational inefficiencies impact revenue generation?

By addressing these questions, the dashboard helps management identify growth opportunities, optimize resource allocation, and improve service quality.

---

## 🏗️ Dashboard Architecture

* Tracks completed bookings, lost bookings, revenue, and ride-distance KPIs.
* Monitors monthly trends in bookings and revenue generation.
* Analyzes revenue contribution across different vehicle categories.
* Evaluates vehicle-wise booking volume and operational performance.
* Identifies top pickup and drop-off locations by ride demand.
* Measures customer and driver satisfaction through ratings analysis.
* Quantifies revenue loss from cancellations and incomplete rides.
* Enables dynamic filtering through interactive vehicle slicers.
* Supports data-driven decisions for fleet and revenue optimization.
* Provides a unified view of operational, customer, and financial metrics.

---

## 🔍 Key Insights Generated

* Auto rides emerged as the highest revenue-contributing vehicle category.
* More than fifty thousand bookings were lost due to cancellations and incomplete transactions, indicating significant revenue leakage.
* Customer satisfaction remained consistently high with an average rating above 4.4.
* Khandsa recorded the highest ride pick-up volume.
* Ashram recorded the highest ride drop-off volume.
* Revenue remained relatively stable throughout the year, indicating consistent demand.

---

## ⚙️ Technical Implementation

### Data Preparation

* Data Cleaning using Power Query
* Missing Value Handling
* Data Type Standardization
* Creation of Supporting Dimension Tables

### Data Modeling

* Star Schema Design
* Fact and Dimension Table Relationships
* Optimized Filtering Structure
* Vehicle Image Mapping Integration

### 🧮 DAX Measures

Key metrics were created using advanced DAX functions such as:

```DAX
Completed_Bookings =
CALCULATE([Booking_Count],Uber[Booking Status] = "Completed")
```

```DAX
Bookings_Remove_Status_Filter =
CALCULATE([Booking_Count],ALL(Uber[Booking Status]))
```

Additional Measures:

```DAX
Booking_Value = SUM(Uber[Booking Value])

Lost_Bookings =CALCULATE([Booking_Count],Uber[Booking Status] <> "Completed")

Average_Distance =
AVERAGE(Uber[Ride Distance])
```

### Visualization Techniques

* Interactive KPI Cards
* Dynamic Vehicle Image Slicers
* Trend Analysis Charts
* Revenue Comparison Visuals
* Conditional Formatting
* Custom Dashboard Layout Design

---

## 🛠️ Tools & Technologies

| Tool             | Purpose                          |
| ---------------- | -------------------------------- |
| Power BI Desktop | Dashboard Development            |
| Power Query      | Data Cleaning & Transformation   |
| DAX              | KPI & Business Logic Development |
| Microsoft Excel  | Data Source Management           |
| Data Modeling    | Relationship Management          |

---

## 🎓Skills Demonstrated

* Business Intelligence
* Data Analytics
* Dashboard Design
* Data Visualization
* KPI Development
* DAX Programming
* Power Query
* Data Modeling
* Analytical Storytelling
* Problem Solving

---

## 📂 Project Files

This repository contains:

* Power BI Dashboard (.pbix) - [UBER_ANALYSIS_DASHBOARD.pbix](https://github.com/jatinguptasrcc085-cpu/uber-ride-analysis-dashboard/blob/ac1a26eb5b7d5816569e3b10a14a5e54f40aed44/UBER_ANALYSIS_DASHBOARD.pbix)
* Dataset (.xlsx/.csv)
* Dashboard Screenshots
* Project Documentation

To explore the dashboard interactively, download the PBIX file and open it in Power BI Desktop.

---

## 👤 Author

### Jatin Gupta

**M.A. Economics | Jamia Millia Islamia**

**B.A. (Hons.) Economics | Shri Ram College of Commerce (SRCC)**

📧 [jatinguptasrcc085@gmail.com](mailto:jatinguptasrcc085@gmail.com)

Open to opportunities in Data Analytics, Business Intelligence, Economic Research, and Consulting.
