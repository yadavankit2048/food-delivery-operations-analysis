# Cleaned Food Delivery Dataset

This folder contains the cleaned dataset used for analysis in the **Food Delivery Operations Analysis** project.

The dataset was cleaned and standardized in Microsoft Excel before any analysis was performed.

---

## File
- `food_delivery_clean_data.xlsx`

---

## Cleaning Summary

The following data cleaning and preparation steps were performed:

### Time & Date Handling
- Converted `Order_Date`, `Time_Ordered`, and `Time_Order_picked` into proper Excel date/time formats
- Fixed Excel time issues where time was stored as fractional day values
- Corrected cross-midnight cases while calculating time differences
- Created a derived column: `Order_to_pickup_minutes`

### Delivery Person Attributes
- Validated `Delivery_person_Age` and handled formatting issues
- Cleaned `Delivery_person_Ratings`
  - Removed invalid values (e.g., ratings greater than 5)
  - Verified rating range consistency

### Order & Vehicle Details
- Standardized `Type_of_order`
- Standardized `Type_of_vehicle` (converted to lowercase, removed inconsistencies)
- Cleaned `Multiple_deliveries` column and validated valid values

### Location & Environment Factors
- Standardized `City_type` (metropolitan / urban / semi_urban)
- Standardized `Road_traffic_density` (low / medium / high)
- Cleaned `Weather_conditions` and handled unknown / inconsistent entries

### Formatting & Consistency
- Removed formatting and conditional formatting issues
- Ensured consistent data types across all columns
- Verified no critical missing or invalid values remained

---

## Usage
This cleaned dataset acts as the **single source of truth** for all subsequent analysis in the `analysis/` folder.  
No data transformations are performed directly inside analysis files.

---

## Notes
- The dataset intentionally reflects real-world imperfections to simulate operational data
- GitHub cannot preview large Excel files; please download the file to explore locally

