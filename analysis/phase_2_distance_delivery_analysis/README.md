# Phase 2: Distance vs Delivery Time Analysis

## Objective
The objective of Phase 2 is to understand how delivery distance impacts delivery time performance and to identify operational risk patterns that are not visible from averages alone.

This phase builds on Phase 1 by moving from pickup delays to last-mile delivery execution.

---

## Business Context
In food delivery operations, distance is often assumed to be the primary driver of delivery delays.

However, in real operations:
- Short distances can still experience delays
- Long distances increase risk but do not explain everything
- Customer dissatisfaction is driven by slow and very slow deliveries, not average time

This phase focuses on analyzing delivery time behavior across distance buckets.

---

## Data Preparation
From the cleaned dataset, the following steps were performed:

1. Verified latitude and longitude ranges to ensure realistic geographic values  
2. Calculated relative delivery distance using restaurant and delivery coordinates  
3. Created distance buckets:
   - Very Short
   - Short
   - Medium
   - Long
4. Created delivery time buckets:
   - Fast
   - Acceptable
   - Slow
   - Very Slow

All transformations were performed using Microsoft Excel.

---

## Analysis Methodology
Pivot tables were created to analyze:

1. Distance vs Delivery Time (Count)
2. Distance vs Delivery Time (% within Distance)

Percentage within distance was used to understand risk distribution rather than relying only on volume.

---

## Key Analysis Performed

### 1. Delivery Time Distribution Across Distance Buckets
Delivery outcomes were analyzed across increasing distance categories.

Observation:
- As distance increases, the proportion of Slow and Very Slow deliveries rises
- Risk increases gradually from Very Short to Long distances

---

### 2. Where Do “Very Slow” Deliveries Spike?
Very Slow deliveries were observed most frequently in:
- Long distance orders
- Medium distance orders to a noticeable extent

This indicates that distance increases risk, but distance alone is not the sole cause of delays.

---

### 3. Do Short Distances Still Show Delays?
Yes.

Even Short distance deliveries show:
- Approximately 24% Slow deliveries
- Around 2–3% Very Slow deliveries

This suggests execution-level issues such as:
- Rider availability
- Restaurant handoff delays
- Local routing inefficiencies

---

## Why Percentage Analysis Matters
Count-based analysis can be misleading because higher distance categories naturally contain more orders.

Percentage within distance answers a more meaningful question:
“If a customer places an order at this distance, what is the likelihood of a delay?”

This approach aligns better with real operational risk assessment.

---

## Key Insights (Phase 2)

- Delivery risk increases with distance, but not in a strictly linear manner
- Long distance orders carry the highest delay risk
- Short distance orders are not immune to delays
- Operational improvements must focus on execution quality, not distance alone
- Distribution analysis reveals customer pain points hidden by average metrics

---

## Tools Used
- Microsoft Excel
- Calculated columns
- Pivot Tables
- Count and percentage distribution analysis
- Business-oriented interpretation

---

## Phase 2 Outcome
Phase 2 identifies where delivery risk concentrates across distance categories and provides a clearer understanding of last-mile delivery behavior.

---

## What Comes Next
The next phase will focus on deeper operational drivers behind delivery delays and further segmentation to isolate root causes.
