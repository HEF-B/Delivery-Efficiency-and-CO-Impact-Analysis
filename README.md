# Delivery-Efficiency-and-CO-Impact-Analysis
# Employee Satisfaction & Workplace Analysis.
Analyzed HR survey data to identify key drivers of employee satisfaction, burnout risk and workplace fairness across Nordic countries, and built an interactive Power BI dashboard to support data-driven HR decision-making.

## Table of Contents
1. [Project Overview](#1-project-overview)
2. [Objectives](#2-objectives)
3. [Executive Summary](#3-executive-Summary)
4. [Tools & Technologies](#4-tools--technologies)
5. [Repository Structure](#5-repository-structure)
6. [Data Workflow](#6-data-workflow)
7. [Key Metrics](#7-key-metrics)
8. [Key Insights](#8-key-insights)
9. [Recommendations](#9-recommendations)
10. [Assumptions & Limitations](#10-assumptions--limitations)
11. [Author](#11-author)

## 1. Project Overview
Organizations often struggle to understand what truly drives employee satisfaction and where risks like burnout or disengagement are emerging. This project explores HR survey data to uncover patterns in employee wellbeing, performance, and career progression across departments and regions.

The dataset was sourced from Kaggle and extended with Nordic country data to create a more realistic and regionally relevant analysis. The focus was on identifying key drivers such as work-life balance, overtime, compensation, and promotion patterns, and understanding how these factors vary across roles and locations.

The final output is a 4-page interactive Power BI dashboard that enables HR teams to monitor employee experience, detect risk areas early, and make more informed workforce decisions.

## 2. Objectives
- Identify the key drivers of employee satisfaction and burnout risk.
- Analyze the impact of overtime on work-life and employee wellbeing.
- Evaluate promotion patterns and fairness across departments and genders.
- Compare workforce trends across Nordic countries.

## 3. Executive Summary

<img width="2250" height="1255" alt="1" src="https://github.com/user-attachments/assets/292a16c7-88b5-4963-8376-e008a9422c9f" />

- The data provides a high-level view of employee satisfaction, engagement, and burnout risk across departments and Nordic countries. Overall engagement is stable (3.1), with a relatively low but meaningful burnout rate of 19.2%, indicating that while most employees are doing well, there is a notable at-risk group that requires attention.
  
- Burnout risk is not evenly distributed. While 80.8% of employees fall into the low-risk category, a smaller segment (approximately 4%) is classified as high-risk, which can have a disproportionate impact on productivity and retention if not addressed early.
  
- Department-level analysis shows that engagement scores are relatively consistent across teams, but headcount differences highlight where HR efforts may have the greatest impact.
  
- On Country level comparisons reveal slight variations in burnout risk, suggesting that local workplace conditions may influence employee wellbeing.

Overall, the dashboard enables HR teams to quickly identify risk areas, compare regions, and take proactive action to improve employee experience.



## 4. Tools & Technologies

| Category        | Tools Used                       |
| --------------- | ---------------------------------- |
| Data Storage    | CSV files (Kaggle dataset)         |
| Data Processing | Power BI (Power Query)             |
| Analysis        | Power BI (DAX) |
| Visualization   | Power BI                           |
| Version Control | Git / GitHub                       |
| Documentation   | Markdown                           |


## 5. Repository Structure

```
Employee Satisfaction & Workplace Analysis/
│
├── data/
│   ├── raw/
│   ├── processed/
│
├── visuals/
│   └── dashboard screenshots/
│
├── pbix/
│   └── Industry Financials Dashboard.pbix
│   
└── README.md

```

## 6. Data Workflow

```
Source
- HR employee dataset from Kaggle, extended with Nordic country data.
        ↓
Ingestion
- Imported into Power BI using Power Query.
        ↓
Cleaning
- Handled missing values
- Standardized categorical variables
- Ensured consistency across added country data
        ↓
Transformation
- Created calculated metrics (burnout categories, engagement index)
- Grouped variables (training hours, salary ranges)
- Structured data for multi-dimensional analysis 
        ↓
Analysis 
- Trend and segmentation analysis
- Department, role, and country comparisons
- Behavioral analysis (overtime vs burnout)  
        ↓
Output
- Interactive Power BI dashboard (Multi-pages)  

```

## 7. Key Metrics

| Metric                  | Definition                           | Why It Matters                             |
| ----------------------- | ------------------------------------ | ------------------------------------------ |
| Engagement Index        | Average employee engagement score    | Measures overall workforce sentiment       |
| Burnout Rate            | % of employees in high-risk category | Identifies retention and performance risks |
| Overtime Hours          | Average extra working hours          | Key driver of burnout                      |
| Promotion Rate          | % of employees promoted              | Indicates career growth and fairness       |
| Work-Life Balance Score | Employee rating of balance           | Strong predictor of satisfaction           |


## 8. Key Insights

### Dashboard 2: Wellbeing & Work Patterns.
<img width="2247" height="1270" alt="2" src="https://github.com/user-attachments/assets/d9086657-cada-48b7-acb5-3b0f444c3097" />

- #### Overtime is the clearest early warning signal for burnout

  - ***Pattern:***
Employees working higher overtime hours consistently show lower work-life balance scores, and a higher proportion of burnout risk (more high-risk cases appear as overtime increases).

  - ***Interpretation:***
This suggests burnout is not random, it is strongly linked to workload pressure. Employees are not necessarily disengaged; they are overextended.

  - ***Impact:***
Overtime becomes a leading indicator HR can monitor proactively. Managing workload and overtime is likely the fastest way to reduce burnout risk before it escalates into turnover.

---
- #### Burnout risk is concentrated in specific roles, not evenly distributed

   - ***Pattern:***
The heatmap shows higher burnout values clustered in roles like Software Engineers, Sales Executives, and certain IT-related positions, while others remain consistently low.

   - ***Interpretation:***
Burnout is role-driven rather than organization-wide. Some roles naturally carry higher pressure, expectations, or workload intensity.

   - ***Impact:***
A one-size-fits-all wellbeing strategy will not work. HR should focus targeted interventions on high-risk roles, rather than applying broad policies across all employees.

---
- #### Moderate overtime is common, extreme cases are the real risk

   - ***Pattern:***
Most employees fall within a moderate overtime range (around 2–4 hours), with relatively fewer employees at extreme levels.

  - ***Interpretation:***
The organization’s overall workload looks manageable at a high level, but outliers (employees with very high overtime) are driving burnout risk.

   - ***Impact:***
Instead of reducing overtime across the board, HR should identify and act on extreme cases, where intervention will have the highest impact.

---
- #### Work-life balance is the strongest differentiator between low and high burnout groups

   - ***Pattern:***
Employees with high work-life balance scores are mostly in the low burnout category, while those with lower scores appear more frequently in medium and high-risk groups.

   - ***Interpretation:***
Work-life balance is not just a “nice-to-have” metric, it directly reflects employee wellbeing and risk exposure.

   - ***Impact:***
Improving work-life balance (through flexibility, workload management, or policy changes) is likely to have a direct and measurable effect on reducing burnout.

---
### **Dashboard 3: Growth, Rewards & Fairness**
<img width="2220" height="1260" alt="3" src="https://github.com/user-attachments/assets/6a523833-8ed5-4c00-8288-a819bad089be" />

- #### Promotion outcomes are uneven across departments and genders
  - ***Pattern:***
Promotion rates vary significantly by department, with noticeable differences between male and female employees in several areas (e.g., IT, Engineering, Operations).

  - ***Interpretation:***
Career progression is not consistent across the organization. These differences may reflect structural imbalances, role pipelines, or potential bias in promotion practices.

  - ***Impact:***
This introduces a fairness risk. If left unaddressed, it can reduce trust, lower motivation, and impact retention especially among underrepresented groups.
________________________________________
- #### Training does not consistently turn into promotions
  - ***Pattern:***
Employees with zero training hours show relatively high promotion percentages, while increased training hours do not clearly lead to higher promotion rates.

  - ***Interpretation:***
Training programs may not be aligned with promotion criteria, or promotions may depend more on experience, visibility, or role demand than formal development.

  - ***Impact:***
This creates a disconnect between effort and reward. HR should reassess whether training is effectively supporting career progression or simply acting as a formality.
________________________________________
- #### Compensation increases with level but variability suggests inconsistencies
  - ***Pattern:***
Salary ranges generally rise with job level, but there is noticeable spread (min–max range) within each level.

  - ***Interpretation:***
While the pay structure appears tiered, the wide variation within levels may indicate inconsistent compensation practices or negotiation-based differences.

  - ***Impact:***
This can lead to perceived inequity, even if the overall structure is sound. Transparency and clearer salary bands may help reduce this risk.
________________________________________
- #### Some departments combine high workload risk with unclear reward signals
  - ***Pattern:***
When combined with earlier findings (burnout + promotions), certain departments show both higher workload pressure and inconsistent promotion outcomes.

  - ***Interpretation:***
Employees in these areas may feel they are working more without proportional recognition or advancement.

  - ***Impact:***
This is a high-risk retention zone. Employees in these roles are more likely to disengage or leave if effort is not matched with growth opportunities.
---
### **Dashboard 4: Detailed Overview**
<img width="2255" height="1262" alt="4" src="https://github.com/user-attachments/assets/1de72872-1cc3-4ac9-a98b-d3de1244427e" />

- #### Employee satisfaction is stable across countries, with only minor variation
  - ***Pattern:***
Average rating scores across Norway, Sweden, Denmark, and Finland are very close (~3.05–3.12), with similar distribution patterns.

  - ***Interpretation:***
Employee experience is relatively consistent across regions, suggesting that company-wide policies and culture are broadly aligned.

  - ***Impact:***
Major interventions do not need to be country specific. HR can focus on role  and workload-based improvements rather than geographic differences.
________________________________________
- #### Work-life balance and job satisfaction are strong, but not exceptional
  - ***Pattern:***
Most responses fall into “Neutral” and “Good” categories, with fewer “Very Good” ratings.

  - ***Interpretation:***
Employees are generally satisfied, but not highly engaged or delighted. There is room to improve from “acceptable” to “excellent.”

  - ***Impact:***
This represents an opportunity zone, not a crisis. Small improvements could significantly boost overall engagement.
________________________________________
- #### Performance ratings are high, but may lack differentiation
  - ***Pattern:***
A large majority of employees are rated positively in performance (strong skew toward high ratings).

  - ***Interpretation:***
Performance evaluations may be inflated or not sufficiently differentiated between employees.

  - ***Impact:***
This reduces the effectiveness of performance as a tool for:
       - Promotions 
       - ompensation decisions 
       - Talent identification 
________________________________________
- #### Workforce distribution is concentrated in key departments and countries
  - ***Pattern:***
Norway has the largest workforce and payroll, with Engineering and IT having the highest headcounts.

  - ***Interpretation:***
Business operations are heavily dependent on a few core regions and technical departments.

  - ***Impact:***
This creates concentration risk  any issues in these areas (burnout, turnover) will have a disproportionate business impact.
________________________________________
- #### Workforce demographics show a mid-career heavy population
  - ***Pattern:***
Age distribution is centred around mid-30s to early 40s.
  - ***Interpretation:***
The workforce is experienced but may soon face:
       - Career plateau risks 
       - Increased demand for growth opportunities 
  - ***Impact:***
HR should focus on:
      - Career progression pathways 
      - Leadership development 
      - Retention strategies for experienced talent 

---

## 9. Recommendations

| Priority | Recommendation                                                      | Based On                                                           | Suggested Owner      |
| -------- | ------------------------------------------------------------------- | ------------------------------------------------------------------ | -------------------- |
| High     | Reduce excessive overtime across teams to prevent burnout           | *“Overtime Impact on Work-Life Balance & Burnout Risk”*            | HR / Team Leads      |
| High     | Identify and support employees in high burnout risk category (~4%)  | *“Burnout Risk Distribution”*                                      | HR                   |
| High     | Focus burnout prevention efforts on IT and Engineering roles        | *“Burnout Hotspots by Department and Role”*                        | HR / Tech Leadership |
| Medium   | Review promotion fairness across departments and genders            | *“Promotions & Promoted Last Year (%) by Department and Gender”*   | HR                   |
| Medium   | Align training programs with promotion outcomes                     | *“Promoted Last Year (%) by Training Hours”*                       | HR                   |
| Medium   | Monitor salary ranges to ensure fair compensation across job levels | *“Monthly Income Distribution by Job Level”*                       | HR / Finance         |
| Low      | Track regional differences in burnout and satisfaction trends       | *“Burnout Risk by Country”* & *“Rating Distribution by Countries”* | HR                   |


## 10. Assumptions & Limitations

### Assumptions
- Survey responses accurately reflect employee sentiment.
- Added Nordic data represents realistic distributions.
- Engagement and burnout scores are consistently measured.
  
### Limitations
- Synthetic/modified dataset may not reflect real company behavior.
- No time-series data .
- Cannot establish causation, only correlation.
- External factors (policy changes, global markets) not fully included

## 11. Author

**Florence Braut**
- 🔗 linkedin.com/in/Florence B
- 💼 Portfolio:https://hef-b.github.io/
- 📧 dainsights@proton.me
