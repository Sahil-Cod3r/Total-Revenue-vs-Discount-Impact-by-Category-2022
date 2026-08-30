# Total Revenue vs Discount Impact by Category

## 📊 Project Objective
The Marketing Team wants to evaluate how discounts are affecting revenue across different product categories. This project creates a bar chart that compares **total revenue before and after discount** using `SUM(before_discount)` and `SUM(after_discount)`, grouped by category. A calculated field measures the discount impact, helping visualize how much revenue is reduced due to discounts in each category.

## 🧮 Calculated Field
```
discount_impact = before_discount - after_discount
```

## 🗂️ Dataset
**File:** `Online_Sales_Data_with_Discount`
(Sourced from Kaggle's Online Sales Dataset, with `before_discount`, `discount`, and `after_discount` columns added based on realistic category-wise discount percentages)

**Columns used:**
| Column | Description |
|---|---|
| `Product Category` | Category of the product (Electronics, Clothing, Books, etc.) |
| `before_discount` | Revenue before discount was applied |
| `after_discount` | Revenue after discount was applied |
| `discount` | Discount amount |
| `discount_impact` | Calculated field: before_discount − after_discount |

## 📈 Chart Details
- **Chart type:** Grouped bar chart
- **Dimension:** `Product Category`
- **Metrics:** `SUM(before_discount)` and `SUM(after_discount)`


## 🔍 Key Insight
**Electronics** generates the highest revenue overall, with the largest absolute revenue loss due to discounts. **Clothing** shows a proportionally larger gap between before and after discount revenue compared to other categories, indicating higher discount rates are applied there. Categories like **Beauty Products** and **Books** have the smallest revenue and discount impact.

## 🔗 Live Report
**Looker Studio Report:** [Revenue vs Discount Impact by Category](https://datastudio.google.com/reporting/a35e325b-b3c0-4e08-9b87-6280a6496de0)

## 🛠️ Tools Used
- Google Sheets (data source)
- Looker Studio (visualization)

## 👤 Author
**Sahil Kumar**
