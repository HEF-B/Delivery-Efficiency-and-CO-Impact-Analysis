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
9. [Executive Conclusion](#9-executive-conclusion)
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

### Operations Performance Report. 
<img width="2636" height="1469" alt="2" src="https://github.com/user-attachments/assets/842e0594-06d4-4dfd-a960-4ba47257ecf5" />

### Root Cause Analysis.
While our logistics network covers a massive 2M km, we are facing a structural Delivery Gap where actual delivery times consistently exceed estimates. The data identifies Oslo as the primary bottleneck and Cargo Planes as the least reliable mode of transport. 
If we want to get above 85% on-time delivery, we need to fix the ups and downs we see in the daily capacity heatmap.

---
### Key Insights.

#### 1.Weather & Traffic Impact
  - ***Pattern:*** The highest route efficiency score—indicating the most friction—occurs during clear weather with high traffic, reaching a peak of 488.
At the same time, during snow and storm conditions, the score increases under low traffic conditions, reaching 223 and 141 respectively.

  - ***Interpretation:*** This suggests that performance challenges are not only driven by extreme weather. Even under clear conditions, high traffic is creating significant delays, which points to limitations in how routes are planned or scheduled.
In harsher weather, the rise in scores—even with low traffic—indicates that environmental conditions alone are enough to disrupt efficiency.

  - ***Impact:*** Delivery performance is being affected by two different pressures: predictable traffic congestion during normal conditions, and reduced operational resilience during severe weather. Addressing both will be important to improve consistency in delivery times.

#### 2. The "Cargo Plane" Reliability.
  - ***Pattern:*** Despite being the most expensive mode, Cargo Planes have one of the lowest On-Time rates at 57%, significantly lower than Vans and Trucks (67-68%).
    
- ***Interpretation:*** We are paying a premium for speed (Air) but receiving the worst reliability. This suggests that ground-level airport handling or air-traffic congestion is negating the speed advantage of flight.
  
- ***Impact:*** Relying on Cargo Planes is currently a high-risk, high-cost strategy. Shifting critical shipments back to road-based Express could actually increase reliability while lowering costs.
  
#### 3. The Weekend Capacity Collapse
  - ***Pattern:*** The Daily Capacity Heatmap shows consistent Red Zones (Peak Loads) on Mondays, Thursdays, and Sundays, while mid-week remains under-utilized (Green).
    
- ***Interpretation:*** Our workload is unevenly distributed. We are likely over-stressing our staff and fleet at the start and end of the week, leading to the 67.1% on-time delivery failure.
  
- ***Impact:*** By Leveling the load, we can reduce overtime costs and minimize the human error factor that contributes to the 1.5-day handling delay.

#### 4. Regional Bottleneck: The "Oslo-Tromsø" Stress Point
  - ***Pattern:*** Oslo is the undisputed bottleneck, originating 543 delay-prone incidents, with the highest individual stress point being the Oslo to Tromsø route (77 score).
    
  - ***Interpretation:*** Oslo is the heart of the network; when it skips a beat, the entire Norwegian supply chain suffers. The Tromsø route is particularly fragile, likely due to distance combined with weather sensitivity.
    
  - ***Impact:*** Investing in a secondary sorting hub outside of Oslo or a dedicated Fast-Track lane for Northern routes like Tromsø would de-risk the entire national network.
  
#### 5. The Expanding Delivery Gap
  - ***Pattern:*** The gap between Estimated Delivery (ED) and Actual Delivery (AD) is widening, peaking in April (9.0 AD vs 8.0 ED).
    
  - ***Interpretation:*** Our predictive algorithms are failing to account for real-world friction. We are consistently over-promising to customers.
    
  - ***Impact:*** This 1-hour "hidden" gap per shipment aggregates into thousands of lost hours across the 2M km traveled, directly causing the dip in on-time delivery and increasing customer service.

---
### Recommendations
#### 1. Improve efficiency at the Oslo hub
  - ***Action:*** Introduce cross-docking in Oslo to reduce the 1.5-day handling time.
  - ***Target:***	 Reduce Oslo’s bottleneck score from 543 to under 400 within the next quarter.
#### 2. "Air-to-Van" Shift for Reliability
  - ***Action:***  Since Vans (68% on-time delivery) outperform Planes (57% on-time delivery), re-route short-haul air freight to high-speed van relays.
  - ***Target:*** Improve on-time delivery by 5% simply by choosing the more reliable.
#### 3. Adaptive Scheduling (Peak Smoothing)
  - ***Action:*** Introduce incentives for customers or partners to ship during "Green Days" (Tuesday/Wednesday) to alleviate the Sunday/Monday red-zone congestion.
  - ***Target:*** Flatten the capacity heatmap to reduce warehouse fatigue and handling errors.
#### 4. Recalibrate Estimated Delivery (ED) Models
  - ***Action:***  Update the April/Spring baseline in the routing software to account for the +1.0 hour variance discovered in the "Actual vs. Estimated" analysis.
  - ***Target:*** Close the "Expectation Gap" to improve customer satisfaction scores even before the physical logistics are fixed.
---
### Financial Performance Report.
<img width="2628" height="1473" alt="3" src="https://github.com/user-attachments/assets/6d2b0d2b-643d-44ba-b37d-1d79b9748e21" />

### Cost Management and Carrier ROI Analysis
With a total delivery spend of 26M NOK and an average cost per kg of 529, our logistics financial health is stable but vulnerable. A staggering 9M NOK is currently identified as Late Delivery Cost Risk, representing nearly 35% of our total spend. Profitability is being threatened by high-cost corridors in Nord-Norge and significant rate variances among our primary carriers.

---
### Strategic Insights.
#### 1. The Geography of Expense: The Northern 
 - ***Pattern:*** Nord-Norge is our most expensive corridor at 7.7M NOK, significantly outpacing southern regions like Sørlandet (2.4M).
   
 - ***Interpretation:*** The higher costs in Northern Norway are largely driven by distance and terrain. This is not only a volume issue, but a structural cost linked to the current routing model.
   
 - ***Impact:*** Any operational improvement in the Nord-Norge route offers the highest financial ROI. Even a 5% efficiency gain in the North saves more than a 15% gain in the South.

#### 2. Carrier Rate Variance: The Efficiency Spread
 - ***Pattern:*** Scandinavian Express and DB Schenker show positive rate variances (0.082 and 0.035), while Posten and DHL Norway are significantly below the benchmark.
   
 - ***Interpretation:*** We have a wide disparity in carrier pricing power. We are currently over-paying for certain specialized carriers while seeing high efficiency from our volume leaders like Posten.

 - ***Impact:*** There is a clear opportunity for Rate Harmonization. By migrating volume from high-variance carriers to those with negative variances (like Posten/DHL), we can lower the total 26M spend without sacrificing service.

#### 3. The "Clear Weather" Spend Trap
 - ***Pattern:*** Over 15.7M NOK (roughly 60% of spend) occurs during Clear Weather, but surprisingly, this is where "Medium" and "High" cost traffic conditions are most concentrated.
   
 - ***Interpretation:*** We are losing money during "good" conditions due to traffic congestion and poor route planning, not just "bad" weather.

 - ***Impact:*** This proves our financial leakage is process-driven, not weather-driven. Improving traffic-aware routing during peak clear-weather windows could recover a significant portion of the 9M NOK risk.

#### 4. Fuel Cost Concentration
- ***Pattern:*** Trucks consume 61% of the fuel cost budget, while Cargo Planes consume 30.4%.

 - ***Interpretation:*** Our financial exposure to fuel price volatility is concentrated in road and air.

 - ***Impact:*** Small fluctuations in global oil prices will hit 91.4% of our logistics spend. Accelerating the transition to EVs for the "Van" segment (only 1.3% of current fuel spend) offers a hedge against this volatility.

---
### Recommendations
#### 1. Risk Mitigation (The 9M NOK Recovery)
   - ***Action:***  Target the 9M NOK Late Delivery Cost Risk by prioritizing shipments on the "Delivery Cost vs. Delay Risk" scatter plot—specifically those high-cost deliveries that are currently falling into the "10+ days late" category.
   - ***Target:*** Convert 20% of "Risk" into "On-Time" to protect ~1.8M NOK in potential penalties or churn costs.
#### 2. Carrier Portfolio Rebalancing
   - ***Action:***  Review contracts for Scandinavian Express. With a variance of 0.082, they are our most expensive partner per km.
   - ***Target:*** Renegotiate or shift volume to Posten or Norsk Transport to capture the negative rate variance and drive down the 529 NOK cost-per-kg.
#### 3. Route-to-Region Optimization
   - ***Action:***  Audit the 7.7M NOK Nord-Norge corridor. Investigate if hub-and-spoke models or rail-intermodal transfers can reduce the reliance on long-haul trucking in this high-cost zone.
#### 4. Traffic-Adaptive Routing
   - ***Action:***  Deploy real-time traffic mitigation strategies during "Clear" weather periods to reduce the 2.6M NOK spent on "High Traffic" clear days.

---
### **Sustainability & Logistics ESG Performance Report**
<img width="2645" height="1491" alt="5" src="https://github.com/user-attachments/assets/07a9ddab-2597-4877-9a11-93799a08ec42" />

### Optimizing Environmental Impact through Operational Analysis.

This project analyses the intersection of logistics operations and environmental sustainability. With a total carbon footprint of 436K kg of CO2, the data highlights a critical reliance on road transport and a significant correlation between shipment priority and emission intensity. While fuel efficiency remains stable, an On-Time Delivery rate of 67.1% suggests a dual opportunity to improve service reliability while simultaneously decarbonizing the supply chain.

---

### Strategic Insights.
#### 1. The "Trucking" Challenge
  - ***Pattern:*** Trucks are the primary driver of emissions, accounting for 0.36M kg of  CO2 vastly outpacing cargo planes, ships, and rail combined.
    
  - ***Interpretation:*** Our environmental impact is heavily weighted on rubber-to-road logistics. Transitioning even a small percentage of long-haul truck routes to rail *the lowest emitter on our chart*could result in exponential carbon savings.
    
#### 2. Priority vs. Planet
  - ***Pattern:*** *Standard* shipping accounts for 302K kg of emissions, while *Express* and *Priority* combined account for 135K kg.
    
  - ***Interpretation:*** While Standard delivery has the highest volume, the Express segment represents a significant portion of our footprint relative to its speed. Reducing *unnecessary urgency* in the supply chain could be our fastest lever for emission reduction.
    
#### 3. External Variables: Weather & Seasonality
  - ***Pattern:*** The majority of emissions occur during Clear weather with 264K kg, likely reflecting peak operational periods.
  - 
  - ***Interpretation:*** Operational volume, rather than weather-related inefficiency, is our primary emission driver. However, the dip in emissions in February (138K) followed by a rebound in March (145K) suggests seasonal volatility that requires agile capacity planning to maintain efficiency.
  - 
#### 4. Carrier Performance Variability
  - ***Pattern:*** There is a wide variance in package weight handled by different carriers (e.g., Posten and Bring handling the highest loads).
    
  - ***Interpretation:*** Not all carriers are equal. By correlating carrier-level emissions with their package weight distribution, we can identify Green Partners and renegotiate contracts with underperformers who have high carbon intensity.

---
### Recommendations.
Based on the dashboard findings, the following actions are proposed:
#### 1.	Modal Shift: 
Incentivize the shift from Road to Rail/Sea for non-urgent shipments to lower the 0.36M kg truck emission peak.
#### 2.	on-time delivery Recovery Plan:
Investigate why 32.9% of deliveries are late. Improving route optimization won't just help the on-time delivery metric, it will reduce wasted fuel and idling emissions.
#### 3.	Carrier Consolidation: 
Shift volume toward carriers demonstrating lower carbon intensity per kg of freight handled.
#### 4.	Priority Optimization: 
Review Express shipping defaults to ensure high-carbon transport is reserved only for truly mission-critical deliveries.

---

## 9. Executive Conclusion

This analysis highlights that delivery performance challenges are not driven by a single issue, but by a combination of routing decisions, transport choices, and regional constraints.

While the network maintains relatively fast delivery times, delays are concentrated in specific regions and conditions, particularly where traffic, weather, and high workload intersect. At the same time, cost and environmental impact are closely linked, with high-speed transport options contributing disproportionately to both.

Overall, the findings suggest that improving delivery outcomes does not require a full redesign of operations, but rather targeted adjustments in how the network is managed day to day.

### Direction

To improve both cost efficiency and sustainability, the business should prioritize consolidating volume within Posten’s trucking network, while gradually shifting suitable express air shipments to rail where geography allows.

### Closing Insight

The key challenge is balancing speed, cost, and environmental impact.
The analysis shows that by improving routing decisions, managing carrier allocation more effectively, and reducing unnecessary use of high-cost transport, the organization can achieve more consistent delivery performance while lowering both cost and emissions.

## 10. Assumptions & Limitations

### Assumptions
- The synthetic dataset was designed to reflect realistic logistics operations, including delivery volumes, routing patterns, and cost structures.
- Delivery time, cost, and emission relationships (e.g., faster transport being more expensive and less sustainable) are assumed to follow typical industry patterns.
- Weather and traffic conditions are simplified representations of real-world disruptions and are assumed to have a consistent impact on delivery performance.
- Carrier performance is treated as comparable across regions, without accounting for differences in service coverage or contractual terms.
- Route efficiency scores are assumed to be a reliable indicator of operational performance and delivery friction.
  
### Limitations
- The dataset is synthetic, so findings should be interpreted as directional insights rather than exact real-world results.
- The analysis does not include time-series depth (e.g., seasonality, long-term trends), which may influence delivery performance and cost over time.
- External factors such as fuel price changes, labor constraints, or regulatory requirements are not included but can significantly impact logistics operations.
- The analysis focuses on aggregated patterns and does not capture shipment-level variability or exceptions.
- CO₂ emissions are estimated based on transport type and volume, and may not reflect precise real-world calculations.


## 11. Author

**Florence Braut**
- 🔗 linkedin.com/in/Florence B
- 💼 Portfolio:https://hef-b.github.io/
- 📧 dainsights@proton.me
