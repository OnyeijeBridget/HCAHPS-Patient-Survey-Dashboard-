# HCAHPS-Patient-Survey-Dashboard-


This project analyzes 9 years of Hospital Consumer Assessment of Healthcare Providers and Systems (HCAHPS) survey data to uncover trends in patient experience across U.S. hospitals. Using Power BI and DAX, I created a two-page interactive dashboard that highlights both national and state-level insights.

---
**📊 Project Overview**

The HCAHPS survey is the first national, standardized survey of patients’ perspectives of hospital care. It measures domains such as:

Nurse Communication

Doctor Communication

Discharge Information

Quietness of the Hospital Environment

Care Transitions and more

---
**Features of the Datasets**

For this project, I worked with multiple tables from the HCAHPS dataset, covering patient experience survey results at the national, state, and facility level.

1. Reports Table

      Release Period (PK): The reporting period (e.g., 07_2019).

      Start Date / End Date: The time range for each survey period.

2. States Table

      State (PK): Two-letter state code.
      
      State Name: Full name of the state.
      
      Region: Census region grouping for states.

3. Measures Table
      
      Measure ID (PK): Unique identifier for each measure.
      
      Measure: The type of patient experience being measured (e.g., Nurse Communication, Cleanliness).
      
      Type: Category of the measure.

4. Questions Table

      Question Num: Identifier for each survey question.
      
      Measure ID (FK): Links the question to its measure.
      
      Question: The actual survey question asked.

      Bottom-box / Middle-box / Top-box Answer: The response categories used in HCAHPS reporting.

5. National Results Table
      
      Release Period (FK): Links to the reporting period.
      
      Measure ID (FK): Links to the measure being evaluated.
      
      Bottom-box %, Middle-box %, Top-box %: National percentages of patient responses.

6. State Results Table

      Release Period (FK): Links to the reporting period.
      
      State (FK): Links to the state.
      
      Measure ID (FK): Links to the measure.

      Bottom-box %, Middle-box %, Top-box %: Percentages of responses at the state level.

7. Responses Table

      Release Period (FK): Reporting period.

      State (FK): State code.
      
      Facility ID: Unique identifier for each hospital/facility.
      
      Completed Surveys: Number of completed patient surveys.
      
      Response Rate (%): Percentage of patients who responded.

---
**Questions:**
This project answers four guiding questions:

1. Have hospitals improved in their quality of care over the past 9 years?
2. Which areas of care have made the most progress?
3. How have scores changed over time?
4. What recommendations can help hospitals further improve patient experience?

---
**🛠 Tools & Skills Used**

Power BI → Dashboard design & storytelling

Power Query → Data cleaning and transformation

DAX → Custom calculations (NPS, YoY change, progress rankings)

Data Modeling → Star schema with fact and dimension tables

---
**📈 Key Insights**

1. Patient experience improved nationally from 2013–2020, peaked in 2021, then dipped post-pandemic.
2. Nurse & Doctor Communication are strong points across the decade.
3. Communication about Medicines, Care Transition, and Quietness of Hospital consistently underperform.
4. State-level analysis revealed wide variation across regions, with some outperforming national averages while others lagged.
