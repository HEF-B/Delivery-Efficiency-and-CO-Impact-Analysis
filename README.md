# Delivery-Efficiency-and-CO-Impact-Analysis
Analyzed logistics operations to identify opportunities to improve delivery reliability, reduce CO₂ emissions, and optimize cost efficiency through Power BI dashboard.

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
Logistics operations often face a trade-off between cost, delivery speed, and environmental impact. This project explores delivery performance data to understand where inefficiencies exist and how they affect both operational reliability and CO₂ emissions.

The dataset was synthetically generated to simulate real-world logistics scenarios, including shipment volumes, delivery times, vehicle types, weather conditions, and carrier performance. The analysis focuses on identifying key drivers of delays, cost variability, and environmental impact.

The final output is a multi-page Power BI dashboard designed to help operations teams monitor performance, detect inefficiencies, and make data-driven decisions to improve both service quality and sustainability.

## 2. Objectives
- Identify the key operational drivers affecting on-time delivery performance and overall delivery efficiency. 
- Determine how different vehicle types impact delivery cost, reliability, and CO₂ emissions. 
- Quantify the impact of external factors (weather and traffic conditions) on delivery delays and route efficiency. 
- Identify high-risk regions and routes contributing most to delays and poor operational performance. 
- Evaluate whether higher delivery costs lead to improved delivery performance or indicate inefficiencies. 
- Analyse carrier performance to identify cost and efficiency differences across logistics providers. 

## 3. Executive Summary
<img width="2621" height="1482" alt="1" src="https://github.com/user-attachments/assets/9da64933-0ffd-4509-85d2-e2c72d8b0019" />

### Optimizing Operational Cost, Speed, and Regional Reliability

This analysis evaluates the operational performance of a logistics network handling 5,000 shipments. While delivery speed is relatively fast, with an average of 2 days, the organization faces a significant On-Time Delivery challenge at 67.1%. 
The data reveals that delivery costs are relatively high, averaging 5.2K NOK per shipment. Largely this driven using Cargo Planes, which is significantly more expensive than other options. In addition, performance issues are not evenly distributed the Østlandet region stands out as a key area where delays and inefficiencies are concentrated.

---
### Strategic Insights 

 #### 1. The Cost of Speed: Air vs. Ground
- ***Insight:*** Cargo Planes represent a massive cost at 48K NOK average delivery cost, compared to just 6K NOK for Trucks.
- ***Interpretation:***  We are paying an 8x premium for air freight. While this supports our 2-day delivery average, the correlation with emissions is nearly linear.
  
If we can identify which deliveries truly need air transport and shift the rest to ground options, we can reduce costs significantly without affecting service where it matters most.

#### 2. Regional Risk: The Østlandet Bottleneck
- ***Insight:*** Østlandet handles the highest volume of activity in the region (over 1M km travelled) but carries a Poor Efficiency Score of 57, more than 3x any other region with 755 late deliveries.
- ***Interpretation:*** The region is critical to overall operations, but it is also where most of the problems are happening. Any disruption here affects the whole network.

#### 3. Carrier Efficiency (Funnel)
- ***Insight:*** Posten and Bring are handling the largest share of volumes (109K and 96K respectively), while smaller specialized carriers like Scandinavian Express remain underutilized.
- ***Interpretation:*** We are heavily reliant on two major carriers. While this offers scale, it also creates a dependency risk. Exploring the "Efficiency Performance" of our other carriers (DSV, DB Schenker) could provide more cost-effective alternatives for specific regional routes.

#### 4. Volume Stability
- ***Insight:*** Shipment volume remained steady over time, with no major spikes or drops from January (1,748) through March (1,652).
- ***Interpretation:*** The consistency in volume suggests that the delivery issues are not caused by peak periods or temporary pressure. They are more likely due to ongoing operational inefficiencies.
________________________________________
 ### Recommendations
#### 1.	Focus on improving performance in Østlandet
Start by understanding where delays are happening. whether in processing, routing, or last-mile delivery and address those specific issues. 
#### 2.	Reduce unnecessary use of air transport
Review which shipments require fast delivery and shift the rest to more cost-effective ground options where possible. Hence improving the 5.2K NOK average cost and lower our carbon footprint.
#### 3.	Test and expand the use of other carriers
Gradually allocate some shipments to underused carriers to evaluate whether they can improve delivery performance in certain regions. like Nord-Norge or Trøndelag.
#### 4.	Align delivery expectations with actual performance
If deliveries are consistently missing expected timelines, it may be necessary to either improve execution or adjust delivery promises to customers.

---
## 4. Tools & Technologies

| Category        | Tools Used                       |
| --------------- | ---------------------------------- |
| Data Storage    | CSV files (synthetic dataset)      |
| Data Processing | Power BI (Power Query)             |
| Analysis        | Power BI (DAX) |
| Visualization   | Power BI                           |
| Version Control | Git / GitHub                       |
| Documentation   | README                           |


## 5. Repository Structure

```
Delivery Efficiency and CO2 Impact Analysis/
│
├├── data/
│   └── logistics dataset.csv 
│
├── visuals/
│   └── dashboard screenshots/
│           └── executive summary.png
│           └──operations dashboard.png
│           └── financial dashboard.png
│          └── Sustainability & ESG dashboard.png
│
├── pbix/
│   └── logistics performance Dashboard.pbix
│   
└── README.md

```

## 6. Data Workflow

```
Data Generation
- Generated synthetic data representing shipments, routes, vehicle types, delivery times, costs, and external conditions.
        ↓
Ingestion
- Imported into Power BI using Power Query.
        ↓
Cleaning
- Standardized standardized fields
- Ensured consistency across dimensions
        ↓
Transformation
- Created calculated metrics (On-time delivery rate, CO₂ emissions per shipment)
- Structured data for multi-dimensional analysis 
        ↓
Analysis 
- Built relationships between key entities
- Trend and segmentation analysis
- Actual vs Estimated Delivery Gap
- On-Time Delivery by Vehicle Type (%)  
        ↓
Output
- Interactive Power BI dashboard (Multi-pages)  

```

## 7. Key Metrics

| Metric                  | Definition                           | Why It Matters                             |
| ----------------------- | ------------------------------------ | ------------------------------------------ |
| On-Time Delivery Rate (%)       | Percentage of shipments delivered within the expected timeframe    | Measures overall service reliability   |
| CO₂ Emissions (kg)          | Emissions generated per shipment and by vehicle type | Measures environmental impact |
| Delivery Cost (NOK)         | Total and average cost per shipment.          | Tracks operational efficiency and cost control                     |
| Average Handling Time (Days)       | Time spent in processing before shipment.            | Used to distinguish internal vs transit delays       |
| Average Delivery Time (Days) | Average number of days from shipment to delivery.          | Helps identify delays in transit.        |


## 8. Key Insights

### Dashboard 2: Wellbeing & Work Patterns.
<img width="2636" height="1469" alt="2" src="https://github.com/user-attachments/assets/842e0594-06d4-4dfd-a960-4ba47257ecf5" />

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
<img width="2628" height="1473" alt="3" src="https://github.com/user-attachments/assets/6d2b0d2b-643d-44ba-b37d-1d79b9748e21" />

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
<img width="2645" height="1491" alt="5" src="https://github.com/user-attachments/assets/07a9ddab-2597-4877-9a11-93799a08ec42" />

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

| Priority | Recommendation                                                                            | Based On                                                                      | Owner                       |
| -------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | --------------------------- |
| High     | Improve transit efficiency by addressing delays during delivery, not handling             | *Actual vs Estimated Delivery Gap*                                          | Operations                  |
| High     | Reduce reliance on high-cost, high-emission transport (e.g., cargo planes) where feasible | *Average Delivery Cost and CO₂ Emissions by Vehicle Type*                   | Operations / Sustainability |
| High     | Focus operational improvements on high-risk regions (e.g., Østlandet)                     | *Operational Risk Areas*                                                    | Operations                  |
| Medium   | Optimize routing and scheduling around peak workload periods                              | *Daily Capacity & Peak Load Analysis*                                       | Operations                  |
| Medium   | Incorporate weather and traffic conditions into planning and forecasting                  | *Impact of Weather & Traffic on Delivery Timelines*                         | Operations                  |
| Medium   | Reassess carrier performance and reallocate volume to more efficient providers            | *Carriers by Efficiency Performance* & *High-Cost Carriers per Kilometer* | Procurement                 |
| Low      | Monitor cost vs performance to eliminate unnecessary spending                             | *Delivery Cost vs Delay Risk*                                               | Finance / Operations        |


## 10. Assumptions & Limitations

### Assumptions
- The dataset was synthetically generated but designed to reflect realistic logistics operations, including delivery volumes, routing patterns, and performance variability. 
- Cost, vehicle type, and CO₂ emission relationships are modeled to mirror typical industry trade-offs. 
- Weather and traffic conditions are simplified but structured to represent how external disruptions can impact delivery timelines and efficiency. 
  
### Limitations
- Since the data is synthetic, the findings should be interpreted as directional insights rather than exact real world measurements. 
- The analysis covers a limited time period, so it does not capture long term trends, seasonality, or operational changes over time. 
- Some real-world factors such as fuel price fluctuations, regulatory constraints, and unexpected disruptions are not included, which may affect cost and performance.


## 11. Author

**Florence Braut**
- 🔗 linkedin.com/in/Florence B
- 💼 Portfolio:https://hef-b.github.io/
- 📧 dainsights@proton.me
