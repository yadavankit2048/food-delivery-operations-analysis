# Food Delivery Operations Analysis (Excel Project)

## Project Overview
This project simulates a **real-world operations analytics case study** for food delivery platforms such as **Swiggy, Zomato, Blinkit**.

The objective is to move beyond basic Excel usage and demonstrate:
- Analytical thinking
- Business reasoning
- Risk identification
- How operational problems hide behind averages

The entire project is built using **Microsoft Excel**, with a strong emphasis on **asking the right questions before calculating answers**.

---

## Business Context
Food delivery operations consist of multiple stages:

1. Order placed → Food prepared  
2. Food picked up by delivery partner  
3. Order delivered to customer  

Customers do not experience averages.  
They experience **delays**.

This project breaks down delivery operations into **focused analytical phases**, each answering one operational question at a time.

---

## Dataset Overview
The dataset contains delivery-level records with attributes such as:
- Delivery time (minutes)
- Order-to-pickup time
- Delivery distance (calculated using latitude & longitude)
- Road traffic density (Low / Medium / High)
- City type
- Restaurant and delivery locations

The raw data was cleaned and enriched using Excel before analysis.

---

## Project Structure
The project is organized into **analysis phases**, each building on the previous one:

```
food-delivery-operations-analysis/
│
├── README.md
│
├── data/
│   └── clean_data.xlsx
│
├── analysis/
│   ├── phase_1_pickup_time_analysis/
│   ├── phase_2_distance_delivery_analysis/
│   └── phase_3_traffic_delivery_time/
│
└── screenshots/
```

---

## Phase 1 — Order to Pickup Time Risk Analysis
**Objective:**  
Understand how long it takes for orders to be picked up after being placed, and identify whether averages hide operational delays.

**Key Focus Areas:**
- Distribution of order-to-pickup time
- Pickup delays across traffic and city types
- Identifying hidden risk using distribution analysis

**Key Insight:**  
Average pickup times appeared stable, but distribution analysis revealed a consistent long tail of delayed pickups, indicating operational inefficiencies even under normal conditions.

---

## Phase 2 — Distance vs Delivery Time Risk Analysis
**Objective:**  
Analyze how delivery distance impacts delivery-time risk and whether distance alone explains delays.

**Key Focus Areas:**
- Delivery distance bucketing
- Percentage-based analysis within distance buckets
- Identification of slow and very slow deliveries

**Key Insight:**  
While longer distances increased delivery risk, significant delays also existed in short and medium distances, indicating that **execution gaps**, not distance alone, drive failures.

---

## Phase 3 — Traffic Density vs Delivery Time Risk Analysis
**Objective:**  
Evaluate how road traffic density impacts delivery performance and whether traffic acts as a root cause or a risk amplifier.

**Key Focus Areas:**
- Delivery time distribution across Low, Medium, and High traffic
- Percentage-based risk comparison
- Identification of tipping points

**Key Insight:**  
Traffic density does not create delays by itself.  
It **amplifies existing execution weaknesses**.  
Medium traffic acts as an early warning zone, while high traffic becomes a tipping point where very slow deliveries spike sharply.

---

## Why Distribution-Based Analysis Matters
Across all phases, this project avoids relying solely on averages because:
- Averages hide tail failures
- Customers experience individual outcomes
- A small percentage of delayed deliveries can disproportionately impact trust and platform reliability

This mirrors how real-world operations teams monitor **risk distributions instead of summary metrics**.

---

## Tools Used
- Microsoft Excel
- Pivot Tables
- Percentage distribution analysis
- Structured analytical reasoning

No macros, automation, or external tools were used.

---

## Key Takeaway
Operational problems rarely appear in averages.  
They reveal themselves under **stress, scale, and distribution analysis**.

This project demonstrates how structured thinking and careful Excel analysis can uncover insights that matter for real-world delivery operations.

---

## Author
**Ankit Yadav**  
Aspiring Data Analyst | Operations Analytics | Excel
