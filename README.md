# Airline Data Snapshot Analysis (Excel)

## Introduction

This project explores a three-week snapshot of a simulated airline database (documented [here](https://github.com/data-analysis-colab/database_creation_airline_python/blob/master/README.md)), 
using Microsoft Excel as the primary tool for analysis and visualization. The objective is to demonstrate Excel’s
ability to handle interactive data exploration, scenario testing, and KPI-driven insights using slicers, pivot tables,
Power Query, and DAX-based measures.

The analysis focuses on key business metrics such as booking performance, revenue, profitability, and delay causes, 
complemented by a dynamic what-if analysis to model the impact of cost and pricing changes.

Associated File: [Excel Workbook](analysis_excel.xlsx)  
Data Model Diagram: [View Diagram](screenshots/(0a)_tables_diagram.png)

## Problem Statement

Airline profitability depends on the interplay of multiple operational and commercial factors, including passenger 
demand, route performance, pricing, and cost structures. Understanding how these factors interact–especially under 
changing economic conditions such as fluctuating fuel costs–is critical for effective decision-making.
This analysis seeks to answer:

- How do booking rates vary by passenger class and day of the week?
- Which airports and routes generate the highest revenues and profits?
- What are the primary causes of delays, and how significant are weather effects?
- How would changes in ticket prices or fuel costs affect overall profitability?

## Skills Demonstrated

- Data transformation and modeling using Power Query and Excel Data Model.
- KPI dashboard design with slicers and dynamic visual navigation. ![Dashboard](screenshots/(1)_home.png)
- Scenario and sensitivity analysis using [DAX-measures](screenshots/(0b)_dax_measures.png) and parameter-driven what-if tools.
- Interactive visual storytelling through pivot-based dashboards.
- Quantitative reasoning applied to operational and commercial airline metrics.
- Collaborative design, verification, and refinement of Power Query transformations, DAX/measure logic, and interactive 
  dashboard elements for clarity and consistency.

## Data Sourcing

All data used in this analysis originates from a synthetic dataset designed to mirror the structure and dynamics of
a real-world airline operation. The snapshot represents three weeks of simulated flight, booking, and operations
data, capturing metrics such as:

- Passenger bookings and class distributions
- Flight profitability and route performance
- Airport traffic volumes
- Delay reasons and weather impacts

This custom data source allows for controlled experimentation while maintaining realistic business behavior.

## Modelling

Data was imported and transformed using Power Query, then modeled within the Excel Data Model. Relationships were 
established between flights, bookings, customers, routes, and delays, enabling cross-domain analysis.

A set of explicit DAX measures was defined to compute costs, revenues, and profits dynamically based on scenario inputs.
These measures are responsive to slicers that adjust key assumptions – such as fuel cost multipliers and ticket price 
multipliers – to simulate different economic conditions.

## Analysis and Visualisation

### Booking Performance by Passenger Class and Day of Week

[Average Booked Rate by Passenger Class & Weekday](screenshots/(2)_class_bookings_weekdays.png)

- Booked rates peak on Fridays and Sundays, consistent with leisure and return travel patterns.
- First-class utilization is highest, suggesting efficient cabin capacity planning, while economy utilization is lowest,
  which aligns with expected demand tiers.

### Revenue by Top Airports

[Total Revenue by Top 10 Most Frequented Departure & Arrival Airports](screenshots/(3)_revenue_top_airports.png)

- Frankfurt serves as the most frequented hub overall.
- London Heathrow (departures) and Vienna International (arrivals) generate the highest total revenues.

### Route Profitability

[Top/Bottom 5 Routes by Profit Margin](screenshots/(4)_route_profit_margins.png)  
[Top/Bottom 5 Routes by Avg Profit per Flight](screenshots/(5)_route_avg_profits.png)

- Short-haul routes dominate the lowest profit margins and total profits.
- The highest profit per flight is achieved on long-haul routes, while short-to-medium-haul routes yield the 
  best margins percentage-wise.

### Delay Analysis

[Departure and Arrival Delays by Reason & Weather Delays by Weather Condition](screenshots/(8)_delay_reasons.png)

- The most frequent delay causes are technical issues and weather, with low visibility (fog) being the top 
  weather-related factor.

### What-If Analysis

[Profitability Scenarios by Flight Performance Tier & Distance Category](screenshots/(6a)_what_if_flight_profits.png)  
[Profitability Scenarios by Passenger Class Performance Tier](screenshots/(7a)_what_if_class_profits.png)

- Assuming a minimum 10% target profit margin, fuel costs could rise by up to 10% before breaching this threshold.
- Beyond that, short- and medium-haul flights and economy-class bookings would dip below target profit margins
  [(see here)](screenshots/(6b)_what_if_flight_profits.png) and the average profit margin of economy-class bookings would fall below 5% [(see here)](screenshots/(7b)_what_if_class_profits.png), 
  putting economy-only flights at risk of resulting in losses.
- To maintain profitability, ticket prices must increase by roughly 1.5% for every additional 5% rise in fuel costs.

## Conclusion

This Excel-based analysis demonstrates the power of combining structured airline simulation data with Excel’s 
analytical capabilities. Through dynamic dashboards and interactive what-if scenarios, it highlights critical 
relationships between operational costs, pricing, and profitability.

The findings emphasize that:

- Profitability is highly sensitive to fuel price fluctuations.
- Short-haul and economy-heavy routes are most vulnerable to margin compression.
- Demand patterns and capacity utilization align with expected business logic, validating the underlying simulation.

This workflow provides a robust analytical template for evaluating strategic airline decisions within a self-contained 
and interactive Excel environment.

## Authors
Jan H. Schüttler (Linkedin), Behzad Nematipour ([linkedin](https://linkedin.com/in/behzad-nematipour-99b8b4399))