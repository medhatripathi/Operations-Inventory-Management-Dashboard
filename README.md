
# 📋  Operations-Inventory-Management-Dashboard
This project is an Excel-based analytics dashboard designed to monitor supply chain efficiency, evaluate supplier performance, and optimize inventory levels. It integrates procurement, sales, and warehouse data to provide a holistic view of the company's operational health, identifying bottlenecks in delivery times and opportunities to reduce excess stock.
[Operations-Inventory-Management-Dashboard](https://docs.google.com/spreadsheets/d/1eM9fw8KwYUIyoR3_v6sVFx6d3ZouvRJHr7SN4oj8znw/edit?usp=sharing)

---

# 🛠 Tech Stack

| Tool | Purpose |
|------|---------|
| **Microsoft Excel** | Core tool for data storage, data cleaning, and visualization |
| **Advanced Formulas** | Utilized for calculating "Days of Supply," Lead Times, and Delivery Delays |
| **Pivot Tables** | Used to aggregate large datasets for high-level summaries |
| **Inventory Logic** | Implementation of ABC Analysis and Safety Stock calculations |

---

# 📁 Data Source

The dataset consists of relational tables simulating a retail hardware/electronics business. It includes:

- Order Data: Purchase orders with timestamps, costs, and delivery statuses.
- Product Master: Metadata including Category, Sell Price, Safety Stock levels, and Reorder Points.
- Supplier Master: Location, Contract Costs, and Payment Terms for international suppliers (China, Vietnam, Mexico).
- Inventory Data: Stock levels distributed across four regional warehouses (North, South, East, West).
- Sales History: Historical monthly sales revenue and units sold (Oct 2023 - Feb 2024).

---

# ✨ Features & HighlightsBusiness Problem

# Business Problem

The business faced visibility challenges regarding supplier reliability (frequent late deliveries) and inventory bloating (holding too much cash in stock). Without a centralized view, it was difficult to determine which suppliers were underperforming and which products were overstocked.
Goal of the Dashboard

# To create a data-driven system that:

- Identifies reliable vs. unreliable suppliers based on "On-Time" metrics.
- Calculates the "Days of Supply" to flag overstocked items.
- Categorizes inventory value (ABC Analysis) to focus resources on high-impact products.

---

# Walkthrough of Key Visuals & Analysis

  ### Supplier Performance Matrix:
  - Analyzes PromisedDate vs. DeliveredDate.
  - Key Finding: The analysis highlights that Supplier S01 provides the shortest Average Lead Time (approx. 5.8 days) and the highest On-Time rate compared to S02 and S03.
  ![Supplier Performance Matrix](https://github.com/medhatripathi/Operations-Inventory-Management-Dashboard/blob/main/2.Supplier%20Performance%20Matrix.png)
  ### Inventory Health & Status:
  - Combines CurrentStock with AvgMonthlySales.
  - Key Finding: The "Status" column reveals that all major products (P101-P105) are currently flagged as "Excess," indicating the company is holding significantly more stock than the demand requires (e.g., P103 has 58 days of supply).
    ![Inventory Health & Status](https://github.com/medhatripathi/Operations-Inventory-Management-Dashboard/blob/main/3.Inventory%20Health%20%26%20Status.png)
   ### ABC Analysis:
   - Classifies products based on AnnualUsageValue.
   - Identifies which products contribute the most to the inventory cost, allowing management to prioritize auditing those items (Category A).
     ![ABC Analysis](https://github.com/medhatripathi/Operations-Inventory-Management-Dashboard/blob/main/4.ABC%20Analysis.png)
   ### Regional Distribution:
   - Breakdown of stock levels by Warehouse (North, South, East, West) to ensure inventory is positioned close to demand.
     ![Regional Distribution](https://github.com/medhatripathi/Operations-Inventory-Management-Dashboard/blob/main/5.Regional%20Distribution.png)

     ---
     
# Business Impact & Insights

- Procurement Optimization: The data suggests shifting volume to Supplier S01 (Alpha Parts Co) due to superior lead times and delivery reliability, potentially renegotiating contracts with S02/S03.
- Cash Flow Improvement: The analysis identified widespread Excess Inventory. Reducing stock levels for products like P103 (58 Days of Supply) down to the Reorder Point could free up significant working capital.
- Demand Planning: By linking historical sales trends with current stock, the business can move from reactive buying to data-driven forecasting.

