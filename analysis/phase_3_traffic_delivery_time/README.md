# Phase 3 — Traffic Density vs Delivery Time Risk Analysis

## Objective
The objective of Phase 3 is to understand how **road traffic density impacts delivery-time risk**, and whether traffic acts as a **root cause of delays** or an **amplifier of existing operational issues**.

Rather than relying on averages, this phase focuses on **distribution-based analysis** to capture operational risk accurately.

---

## Business Question
- How does delivery-time risk change across **Low → Medium → High traffic**?
- At what traffic level do **Very Slow** deliveries begin to appear?
- Is traffic the primary cause of delays, or does it expose deeper execution gaps?

---

## Data Used
- `road_traffic_density` (Low / Medium / High)
- `delivery_time_bucket`  
  - Acceptable  
  - Fast  
  - Slow  
  - Very Slow  

---

## Analysis Approach

Two pivot tables were created:

### 1. Delivery Time Distribution by Traffic Density (Order Count)
- Shows absolute volume of orders across traffic levels
- Helps understand **load distribution**

### 2. Delivery Time Distribution by Traffic Density (Percentage Within Traffic Level)
- Normalizes risk within each traffic category
- Enables **fair comparison across traffic conditions**
- Highlights **tail risk (Slow + Very Slow deliveries)**

Percentage-based analysis was intentionally used because customers experience **individual outcomes**, not averages.

---

## Key Observations

### 1. Risk Exists Even in Low Traffic
- Low traffic conditions still show **Slow deliveries**
- Indicates delays are not solely traffic-driven

### 2. Medium Traffic Acts as an Early Warning Zone
- **Very Slow deliveries first appear** at medium traffic
- Suggests operational stress begins before peak congestion

### 3. High Traffic Is a Tipping Point
- Very Slow deliveries spike sharply under high traffic
- Risk increase is **non-linear**, not gradual

---

## Core Insight
Traffic density does not create delivery delays by itself.  
It **amplifies existing execution weaknesses**, such as:
- Rider allocation inefficiencies
- Restaurant readiness delays
- Local coordination gaps

High traffic acts as a **stress test** for the delivery system.

---

## Why Percentage-Based Analysis Matters
- Averages hide tail failures
- A small percentage of delayed orders can disproportionately impact:
  - Customer trust
  - Platform ratings
  - Repeat usage

This mirrors how large-scale operations monitor **risk distributions instead of summary metrics**.

---

## Phase 3 Conclusion
Traffic is not the root cause of delays.  
It is a **risk amplifier** that exposes hidden operational failures already present in the system.

---

## Output Files
- Excel file with:
  - Order count pivot table
  - Percentage distribution pivot table
- This README summarizing insights and interpretation

---

## Next Phase
**Phase 4 — Executive Dashboard & Operational Summary**
