# ☕ Coffee Sales Dashboard

An interactive Excel dashboard analyzing coffee sales data across the United States, Ireland, and the United Kingdom — covering order trends, product performance, and customer insights.

---

## 📊 Project Overview

This project involves building a dynamic sales dashboard in Microsoft Excel using raw transaction data from a coffee retail business. The dataset spans multiple years and includes detailed order-level records across four coffee types, three roast levels, and five package sizes.

---

## 📁 Dataset Description

The workbook contains the following sheets:

| Sheet | Description |
|---|---|
| `orders` | Raw transaction data — the source of truth |
| `Dashboard` | Interactive visual summary with slicers/filters |
| `Total Sales` | Pivot table: monthly sales by coffee type (2019–2022) |
| `Country Bar Chart` | Aggregated sales by country |
| `Top 5 Customers` | Ranked list of highest-spending customers |

### Orders Schema

| Column | Description |
|---|---|
| Order ID | Unique identifier per transaction |
| Order Date | Date of purchase |
| Customer ID | Unique customer reference |
| Product ID | Encoded product identifier (e.g. `R-M-1` = Robusta, Medium roast, 1kg) |
| Quantity | Units ordered |
| Customer Name | Full name of the customer |
| Email | Customer email address |
| Country | United States, Ireland, or United Kingdom |
| Coffee Type | `Ara` (Arabica), `Exc` (Excelsa), `Lib` (Liberica), `Rob` (Robusta) |
| Roast Type | `L` (Light), `M` (Medium), `D` (Dark) |
| Size | Package weight in kg (0.2, 0.5, 1, 2.5) |
| Unit Price | Price per unit (USD) |
| Sales | Total sale value (Quantity × Unit Price) |
| Coffee Type Name | Full coffee type name |
| Roast Type Name | Full roast type name |
| Loyalty Card | Whether the customer has a loyalty card (Yes/No) |

---
## 📊 Project image

<img width="804" height="394" alt="image" src="https://github.com/user-attachments/assets/1646e8ae-d91c-404d-9710-ea8f44883c6e" />



## 🔍 Key Insights

- **United States** accounts for the majority of total revenue (~$14,035), far exceeding Ireland (~$2,510) and the United Kingdom (~$1,380)
- **Excelsa** and **Liberica** varieties show strong seasonal peaks across mid-year months
- Top customer **Terri Farra** leads in spend at ~$211, with a tightly clustered top-5
- Loyalty card holders are distributed across all three markets

---

## 🛠 Tools Used

- **Microsoft Excel** — Pivot Tables, Pivot Charts, Slicers, Data Validation
- **Data Cleaning** — Lookup formulas (XLOOKUP / INDEX-MATCH) to enrich raw orders with product and customer details
- **Dashboard Design** — Interactive filters by roast type, package size, and loyalty card status

---

## 🚀 How to Use

1. Download or clone this repository
2. Open `Coffee_Dashboard_Project.xlsx` in Microsoft Excel (2016 or later recommended)
3. Navigate to the **Dashboard** sheet
4. Use the slicers to filter by:
   - Coffee Type
   - Roast Type
   - Package Size
   - Loyalty Card status
5. Charts and KPIs will update dynamically

---

## 📂 File Structure

```
📦 coffee-sales-dashboard
 ┣ 📊 Coffee_Dashboard_Project.xlsx
 ┗ 📄 README.md
```

---

## 🙋 Author

Feel free to connect or reach out if you have questions about the project methodology or want to collaborate!
