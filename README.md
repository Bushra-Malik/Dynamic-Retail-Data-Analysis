# 📊 Dynamic Retail Data Analysis

## Project Overview
**Dynamic Retail Data Analysis** is an end-to-end data analytics project exploring multi-store retail sales. The analysis evaluates how operational events (**holidays**, **promotional markdowns**) and external factors (**temperature**, **fuel prices**) drive weekly store revenue.

## Dataset
The analysis uses the [Retail Dataset](https://www.kaggle.com/datasets/manjeetsingh/retaildataset) by Manjeet Singh, containing:
- **Store Metadata**: Store types and store size.
- **Sales Figures**: Weekly departmental sales per store.
- **Economic & Environmental Factors**: CPI, Unemployment, Temperature, Fuel Prices, and **MarkDowns 1–5**.

---

## Data Cleaning & Pipeline Preprocessing
1. **Missing Values**: Imputed missing `MarkDown1-5` values with `0` (indicating no promotion run) and forward-filled (`ffill`) missing economic indicators (`CPI`, `Unemployment`).
2. **Datetime Formatting**: Converted date strings into standard Python `datetime64` objects.
3. **Data Integration**: Joined `Sales`, `Features`, and `Stores` on key attributes (`Store`, `Date`, `IsHoliday`).
4. **Feature Engineering**:
   - Calculated `Total_MarkDown` by summing all 5 markdown columns per record.
   - Binned continuous variables (`Temperature` and `Fuel_Price`) into 5 ordinal categories (*Very Low/Cold* to *Very High/Hot*).

---

## 💡 Key Findings & Insights
* **Holiday Sales Lift:** Sales experience a **+7.13% increase** during holiday weeks compared to standard weeks[cite: 1].
* **Promotional Impact:** Weeks with active promotional markdowns see a **+1.92% lift** in average weekly revenue[cite: 1].
* **Weather Effect:** Peak sales revenue occurs during **Moderate** temperature conditions[cite: 1].
* **Fuel Price Sensitivity:** Lower fuel prices correlate directly with higher weekly sales volume[cite: 1].

---

## 🎯 Strategic Recommendations
1. **Advance Holiday Inventory:** Ramp up store inventory and warehouse fulfillment 3–4 weeks prior to major holiday periods.
2. **Targeted Markdowns:** Focus promotional price cuts on high-margin or slow-moving items rather than broad store-wide discounting.
3. **Macroeconomic Pricing:** Monitor fuel price trends and scale up local marketing campaigns when pump prices drop, taking advantage of increased consumer spending power.
