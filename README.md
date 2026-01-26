# Food Delivery Operations Analysis (Excel Project)

## Project Overview
This project simulates a real-world operations analytics case study for food delivery platforms such as Swiggy and Zomato.

The objective is to understand where and why operational delays occur in food delivery workflows and how data-driven insights can help improve customer experience, delivery efficiency, and reliability.

The project is built entirely using Microsoft Excel, with a strong focus on analytical thinking, problem framing, and interpretation rather than tools alone.

---

## Business Context
In food delivery platforms, total delivery time is influenced by multiple operational stages:

- Order placed → Restaurant prepares food  
- Rider reaches restaurant (Pickup Time)  
- Rider delivers order to customer (Delivery Time)

While customers often tolerate food preparation time, delays after food is ready (pickup and delivery delays) lead to customer frustration, poor ratings, cancellations, and reduced platform trust.

This project breaks down the delivery process into phases to analyze delays systematically instead of relying on overall averages.

---

## Phase-wise Analysis Overview
This project is structured as a phase-wise operational analysis, where each phase answers a specific business question.

### Phase 1: Order-to-Pickup Time Analysis
Key question:  
How long does it take for orders to be picked up after being placed, and what factors influence this delay?

What was analyzed:
- Order-to-pickup time distribution
- Pickup delays across traffic conditions (Low / Medium / High)
- Pickup delays across city types (Metropolitan / Urban / Semi-Urban)

Key takeaway:
Average pickup times appeared stable, but distribution analysis revealed hidden long-tail delays, even under low-traffic conditions.

---

### Phase 2: Distance vs Delivery Time Analysis
Key question:  
Does delivery distance increase the risk of slow or very slow deliveries?

What was analyzed:
- Relative delivery distance using restaurant and delivery coordinates
- Distance buckets: Very Short, Short, Medium, Long
- Delivery time buckets: Fast, Acceptable, Slow, Very Slow
- Count and percentage distribution within each distance bucket

Key takeaway:
Delivery risk increases with distance, but distance alone does not explain all delays. Short-distance orders still experience significant delays, indicating execution issues beyond routing or distance.

---

## Why Distribution Analysis Matters
Relying only on averages can be misleading because:
- Averages hide extreme delays
- Customers experience individual delays, not overall performance
- Operational risk lies in the long tail (slow and very slow cases)

This project emphasizes distribution-based analysis, similar to how large-scale systems monitor tail latency and SLA breaches.

---

## Dataset Description
The dataset contains food delivery order records with attributes such as:
- Order and pickup timestamps
- Delivery time (minutes)
- Traffic density
- City type
- Delivery partner details
- Restaurant and delivery location coordinates

Raw data was cleaned and transformed before analysis.

---

## Tools Used
- Microsoft Excel
- Calculated columns
- Pivot Tables
- Count and percentage distribution analysis
- Business-oriented interpretation (no automation or scripting)

---

## Project Structure
food-delivery-operations-analysis/
│
├── README.md
├── data/
│   └── clean_data.xlsx
├── analysis/
│   ├── phase_1_pickup_time/
│   │   ├── README.md
│   │   └── phase_1_pickup_time_analysis.xlsx
│   └── phase_2_distance_delivery_analysis/
│       ├── README.md
│       ├── phase_2_clean_data.xlsx
│       └── phase_2_pivot_analysis.xlsx
└── screenshots/

---

## Key Skills Demonstrated
- Data cleaning and feature engineering in Excel
- Pivot table–based analysis
- Distribution and risk analysis
- Business-oriented interpretation
- Structured analytical documentation

---

## Project Roadmap
- Phase 1: Order-to-Pickup Time Analysis (Completed)
- Phase 2: Distance vs Delivery Time Analysis (Completed)
- Phase 3: End-to-End Delivery Time & Execution Drivers
- Phase 4: Operational Risk Identification & Recommendations

---

## Author
Ankit Yadav  
Aspiring Data Analyst | Operations Analytics | Excel

---

## Note
This project is intentionally built in Excel to demonstrate strong analytical fundamentals before moving to SQL, Python, and BI tools.
