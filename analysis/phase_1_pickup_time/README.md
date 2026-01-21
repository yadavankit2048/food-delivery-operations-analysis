# Phase 1: Order to Pickup Time Analysis

## Objective
To analyze how long it takes for orders to be picked up after being placed,
and to understand how this time varies across operational conditions.

---

## Key Questions Addressed
- How is order-to-pickup time distributed?
- Do averages hide operational delays?
- How does traffic density affect pickup time?
- Does city type influence pickup efficiency?

---

## Metrics Used
- Order_to_pickup_minutes
- Pickup time buckets (<5, 5–10, 10–15, >15 minutes)
- Percentage distribution
- Count distribution

---

## Analysis Approach
- Used Pivot Tables for aggregation
- Analyzed both count and percentage distributions
- Avoided relying only on averages to prevent misleading conclusions

---

## Output Files
- Excel file with pivot tables
- Written insights summarizing findings

---

## Key Insights (Phase 1)
- Order-to-pickup time averages appeared stable, but distribution analysis revealed a significant long tail (>15 minutes).
- Pickup delays were present even during low traffic conditions, indicating non-traffic-related operational issues.
- Metropolitan cities showed scale-driven delays rather than isolated inefficiencies.
- Percentage-based analysis exposed risks hidden by average metrics, similar to tail latency in large-scale systems.
---

## Excel Analysis File

The complete Phase 1 analysis is documented in the Excel workbook below:

📊 **pickup_time_analysis.xlsx**

This Excel file contains:
- Cleaned pivot tables (count-based analysis)
- Percentage distributions within traffic conditions
- Percentage distributions within city types
- Time bucket segmentation used for operational insights

Readers are encouraged to explore the Excel file alongside this README
to understand how insights were derived step by step.


