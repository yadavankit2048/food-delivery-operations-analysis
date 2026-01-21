# Food Delivery Operations Analysis (Excel Project)

## Project Overview
This project simulates a real-world operations analysis for food delivery platforms such as **Swiggy** and **Zomato**.  
The goal is to understand how operational delays occur and how data-driven insights can help improve customer experience and delivery efficiency.

This project is built entirely using **Microsoft Excel**, focusing on analytical thinking rather than tools alone.

---

## Business Context
In food delivery platforms, total delivery time is influenced by multiple stages:
- Order placed → Restaurant prepares food
- Rider reaches restaurant (Pickup Time)
- Rider delivers to customer (Delivery Time)

While customers often tolerate food preparation time, **delays after food is ready (pickup & delivery delays)** lead to dissatisfaction, cancellations, and poor ratings.

This project focuses on **Order-to-Pickup Time** as Phase 1 of a larger analysis.

---

## Phase 1 Objective: Order-to-Pickup Time Analysis
The objective of Phase 1 is to:
- Understand how long it takes for orders to be picked up after being placed
- Analyze how this time varies across:
  - Traffic conditions
  - City types (Metropolitan, Urban, Semi-Urban)
- Identify whether averages hide operational risks

---

## Dataset Description
The dataset contains food delivery order records with attributes such as:
- Order-to-pickup time (in minutes)
- Traffic density (Low / Medium / High)
- City type
- Delivery partner details
- Restaurant and delivery locations

Raw data was cleaned before analysis.

---

## Methodology (Step-by-Step)
1. Cleaned raw data and standardized column formats
2. Created time buckets for Order-to-Pickup Time:
   - <5 minutes
   - 5–10 minutes
   - 10–15 minutes
   - >15 minutes
3. Built Pivot Tables to analyze:
   - Overall pickup time distribution
   - Pickup time distribution by traffic condition
   - Pickup time distribution by city type
4. Converted counts into percentages to analyze distributions
5. Compared averages vs distributions to uncover hidden insights

---

## Key Analyses Performed

### 1. Overall Order-to-Pickup Time Distribution
Analyzed how pickup times are distributed across defined time buckets.

**Insight:**  
Averages appeared stable, but distributions revealed that a significant portion of orders exceeded acceptable pickup times.

---

### 2. Pickup Time Distribution by Traffic Condition
Compared pickup times across:
- Low traffic
- Medium traffic
- High traffic

**Insight:**  
Even under low traffic, long pickup times (>15 min) existed, indicating issues beyond traffic alone (restaurant readiness, rider availability).

---

### 3. Pickup Time Distribution by City Type
Compared pickup behavior across:
- Metropolitan
- Urban
- Semi-Urban cities

**Insight:**  
Metropolitan cities showed higher volume but similar pickup distributions, suggesting scalability challenges rather than isolated delays.

---

## Why Distribution Matters More Than Average
Average pickup time remained around similar values across categories.

However:
- Averages hide tail delays
- Customers experience delays, not averages
- Operational risk lies in the **long tail (>15 min)**

This mirrors real-world metrics like **tail latency** used by large-scale tech companies.

---

## Tools Used
- Microsoft Excel
- Pivot Tables
- Percentage distribution analysis
- Business reasoning (no automation or scripts)

---

## Project Structure
food-delivery-operations-analysis/
│
├── README.md
├── data/
│ └── clean_data.xlsx
├── analysis/
│ └── Phase_1_Pickup_Time_Analysis.xlsx
├── reports/
│ └── Phase_1_Analysis_Report.pdf
└── screenshots/

---

---

## Next Steps
- Phase 2: Pickup-to-Delivery Time Analysis
- Phase 3: End-to-End Delivery Time vs Customer Ratings
- Phase 4: Operational Recommendations

---

## Author
Ankit Yadav  
Aspiring Data Analyst | Operations Analytics | Excel
