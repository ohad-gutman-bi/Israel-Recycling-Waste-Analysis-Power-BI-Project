<img width="1983" height="793" alt="ChatGPT Image Oct 1, 2026, 07_52_18 PM" src="https://github.com/user-attachments/assets/cf9e2fcc-f1f2-48d9-9a25-eb193de1358c" />
<p align="center">
  <img src="./Docs/dashboard_main.png" alt="Israel-Recycling-Waste-Analysis-Power-BI-Project" width="100%" style="border-radius: 8px;">
</p>

# Israel-Recycling-Waste-Analysis-Power-BI-Project
This repository features an end-to-end BI project analyzing municipal recycling trends in Israel. It transforms raw multi-year data using Power Query ETL, structures it into a dimensional star schema model, and delivers interactive Power BI dashboards driven by advanced DAX metrics for strategic decision-making.
---
#  Israel Recycling & Waste Analysis — Power BI Project

##  Overview
This repository contains an end-to-end Business Intelligence project analyzing recycling and waste management trends across Israeli municipalities and local authorities. 

The project was developed as a **Final Capstone Project for the BI Developer Course at abra**. 

The main objective was to take raw, unorganized Excel datasets containing multi-year recycling records, perform comprehensive data cleaning and transformations using **Power Query**, design a robust dimensional data model, and craft interactive **Power BI Dashboards** powered by **DAX metrics** for strategic decision-making.

---

##  Tech Stack & Tools Used
* **Business Intelligence Tool:** Microsoft Power BI Desktop
* **ETL & Data Transformation:** Power Query (M Language)
* **Data Modeling & Calculations:** DAX (Data Analysis Expressions)
* **Data Source:** Raw Excel reports covering waste types, municipal demographics, and annual recycling tonnages.

---

## 🏗️ Data Architecture & Modeling
The project follows a **Star Schema** architectural pattern to ensure optimal DAX performance and streamlined report filtering.

### Data Model Components:
* **Fact Table (`RecycleFactTable`):** Contains granular transactional records of collected recycled materials (in Tons) across various years and areas[cite: 1].
* **Dimension Tables:**
  * `CityData`: Demographic data per municipality (Population, District, City Type, Average Salary, Council Members)[cite: 1].
  * `TypeData`: Waste classification details (Separation methods, Decomposition time, Processing effort hours per ton)[cite: 1].
  * `DimDate`: Standard date dimension for time-intelligence analysis[cite: 1].

---

##  ETL Process (Power Query)
1. **Extraction:** Imported raw multi-file Excel workbooks spanning multiple years (2014–2019)[cite: 1].
2. **Transformation:**
   * Filtered system files and unpivoted columns to convert wide-format yearly data into a normalized long-format fact table[cite: 1].
   * Handled missing values, standardized header promotions, and fixed data type inconsistencies (Int64, Decimals, Strings)[cite: 1].
   * Cleaned geographic names and waste type IDs to enable proper primary/foreign key relationships[cite: 1].
3. **Loading:** Loaded sanitized data streams into the Power BI Tabular Engine[cite: 1].

---

##  Key Insights & DAX Calculations
The project incorporates custom DAX measures and calculated columns for advanced analytical views[cite: 1]:
* **Time Intelligence:** Year-over-Year (YoY) growth calculations for total recycled volume using custom date hierarchies[cite: 1].
* **Per Capita Analysis:** Measuring recycling volume per resident by combining municipal population data with total tonnage[cite: 1].
* **Effort & Efficiency:** Calculating operational hours required per ton recycled based on waste type characteristics[cite: 1].

---

##  Dashboard Features
* **Executive Overview:** High-level KPIs displaying total recycling volume, active municipalities, and top-performing districts[cite: 1].
* **Geographic & Municipal Insights:** Regional breakdowns highlighting performance differences across local councils, districts, and population clusters[cite: 1].
* **Material & Environmental Impact:** Deep dive into specific waste streams (e.g., paper, plastic, glass) and their corresponding decomposition footprints and processing requirements[cite: 1].

---

1. Clone this repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/Israel-Recycling-BI-Analysis.git](https://github.com/YOUR_USERNAME/Israel-Recycling-BI-Analysis.git)
