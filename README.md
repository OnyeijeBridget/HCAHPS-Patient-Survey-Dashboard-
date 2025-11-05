# 🏥 **HCAHPS Patient Survey Analysis | Power BI**

<p align="center">
  <img src="https://img.shields.io/badge/Tool-Power%20BI-yellow?style=flat-square&logo=powerbi" alt="Power BI Badge"/>
  <img src="https://img.shields.io/badge/Skill-DAX-blue?style=flat-square" alt="DAX Badge"/>
  <img src="https://img.shields.io/badge/Focus-Healthcare%20Analytics-green?style=flat-square&logo=data:image/svg+xml;base64," alt="Healthcare Analytics Badge"/>
  <img src="https://img.shields.io/badge/Platform-Maven%20Analytics-orange?style=flat-square" alt="Maven Analytics Badge"/>
</p>

---

## 📘 **Overview**
This project analyzes **9 years of Hospital Consumer Assessment of Healthcare Providers and Systems (HCAHPS)** survey data to uncover trends in patient experience across U.S. hospitals.  

Using **Power BI and DAX**, I created a **two-page interactive dashboard** that tracks both national and state-level performance, providing clear visibility into areas of excellence and opportunities for improvement.

---

## 🎯 **Project Objective**
The **HCAHPS survey** is the first national, standardized measure of patients’ perspectives on hospital care in the United States.  

This project set out to:
1. 📈 Assess how hospital quality of care evolved from **2013–2022**  
2. 🔍 Identify areas of care showing the most improvement  
3. ⏳ Examine changes in patient experience over time  
4. 💡 Recommend actions to improve overall satisfaction  

📊 **Data Source:** [Maven Analytics](https://mavenanalytics.io/data-playground)

---

<details>
<summary><b>🧾 Dataset Structure (Click to Expand)</b></summary>

### 🧩 **Reports Table**
- `Release Period (PK)` – Reporting period (e.g., 07_2019)  
- `Start Date / End Date` – Time range for each survey  

### 🗺️ **States Table**
- `State (PK)` – Two-letter state code  
- `State Name` – Full name of state  
- `Region` – Census region grouping  

### 📏 **Measures Table**
- `Measure ID (PK)` – Unique identifier for each measure  
- `Measure` – Patient experience metric (e.g., Nurse Communication)  
- `Type` – Measure category  

### 💬 **Questions Table**
- `Question Num` – Identifier  
- `Measure ID (FK)` – Linked measure  
- `Question` – Survey question text  
- `Bottom-box / Middle-box / Top-box %` – Response categories  

### 🌍 **National Results Table**
- `Release Period (FK)` – Reporting period reference  
- `Measure ID (FK)` – Measure reference  
- Response % fields for bottom, middle, and top-box categories  

### 🏛️ **State Results Table**
- `Release Period (FK)` – Reporting period reference  
- `State (FK)` – State reference  
- `Measure ID (FK)` – Measure reference  
- Response % by state  

### 🧮 **Responses Table**
- `Facility ID` – Hospital identifier  
- `Completed Surveys` – Count of valid responses  
- `Response Rate (%)` – Participation percentage  

</details>

---

## ⚙️ **Methodology**
To answer the research questions, I developed a **two-page Power BI dashboard** structured as follows:

| Page | Focus | Description |
|------|--------|-------------|
| **Page 1** | National Overview | Long-term trends, top & bottom measures |
| **Page 2** | State Insights | Regional comparisons and performance deviations |

### 🧠 Workflow Steps
1. **Data Modeling:** Built a **star schema** linking fact tables (National, State, Responses) with dimensions (Measures, Questions, States, Dates).  
2. **Power Query Transformation:** Cleaned data and standardized naming conventions.  
3. **DAX Calculations:** Created metrics like:  
   - `NPS Score = Top-box % – Bottom-box %`  
   - Year-over-Year (%)  
   - Measure Ranking by Improvement  
4. **Dashboard Design:** Used card visuals, KPIs, slicers, and dynamic filtering for interactivity.  

---

## 🧰 **Tools & Skills Demonstrated**

| 🧩 Skill | 💼 Description |
|-----------|----------------|
| **Power BI** | Data modeling, visualization, dashboard creation |
| **Power Query** | Data cleaning, merging, and transformation |
| **DAX** | Custom metrics (NPS, YoY change, ranking) |
| **Data Modeling** | Star schema relationships for optimized performance |
| **Storytelling** | Presenting insights through clean, contextual visuals |

---

## 💡 **Key Insights**
- 🟢 **Patient experience improved** nationally from 2013–2020, peaked in 2021, then slightly declined post-pandemic.  
- 💬 **Nurse and Doctor Communication** consistently ranked highest in satisfaction.  
- 🔴 **Communication About Medicines** and **Quietness of Environment** scored lowest.  
- 🧭 **Regional variation** revealed that hospitals in certain states outperformed national averages, suggesting localized best practices.  

---

## 🩺 **Recommendations**
✅ Invest in **communication training** for clinical staff  
✅ Improve **pain management protocols** and patient comfort measures  
✅ Reinforce **cleanliness and noise control policies**  
✅ Continue tracking HCAHPS data for continuous quality improvement  

---

## 📊 **Dashboard Preview**

### 🗺️ National Insights (Page 1)
![National Dashboard](https://github.com/OnyeijeBridget/HCAHPS-Patient-Survey-Dashboard-/blob/main/National%20Results.png)

### 🧭 State Insights (Page 2)
![State Dashboard](https://github.com/OnyeijeBridget/HCAHPS-Patient-Survey-Dashboard-/blob/main/State%20Results.png)

---

<details>
<summary><b>📂 Repository Files</b></summary>

| File | Description |
|------|--------------|
| `HCAHPS_Patient_Experience_Dashboard.pbix` | Power BI project file |
| `HCAHPS_Dataset.xlsx` | Maven Analytics dataset |
| `Project_Summary.pdf` | PDF summary of visuals and insights |
| `National Results.png` / `State Results.png` | Dashboard snapshots |

</details>

---

## 🏁 **Conclusion**
This project demonstrates how **data analytics can drive hospital quality improvements** by visualizing patient feedback across time and geography.  
The interactive dashboard supports **evidence-based decision-making** to enhance patient satisfaction and healthcare delivery outcomes.

---

## 🧠 **Skills Highlight**
`Power BI` • `DAX` • `Data Modeling` • `Healthcare Analytics` • `Data Storytelling` • `Power Query`

---

## 📬 **Contact**
**Bridget Onyeije**  
📍 Nigeria  
💼 [LinkedIn](https://www.linkedin.com/in/bridget-onyeije)  
📊 [GitHub Portfolio](https://github.com/OnyeijeBridget)  

---

<p align="center">
  ✨ <i>Turning healthcare data into meaningful insights that improve patient experience.</i> ✨
</p>
