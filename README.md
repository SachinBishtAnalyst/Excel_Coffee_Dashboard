# ☕ Coffee Sales Dashboard

An interactive Excel dashboard analyzing coffee sales data across the United States, Ireland, and the United Kingdom — built with dynamic slicers to explore sales by coffee type, roast, package size, and loyalty card status.

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

## 🔍 Dashboard Slicer Insights

The dashboard includes four interactive slicers. Here's what the data reveals when you filter by each dimension:

### 🔥 Roast Type Slicer
| Roast Type | Total Sales |
|---|---|
| Light | $17,354 |
| Medium | $14,600 |
| Dark | $13,179 |

- **Light roast** is the clear winner, generating ~19% more revenue than Medium and ~32% more than Dark.
- This pattern holds across loyalty card holders and non-holders alike, suggesting light roast is a universal preference rather than a niche segment.
- When combined with the size slicer, Light roast in the **2.5kg** package alone drives ~$8,986 — by far the highest-revenue combination.

---

### 📦 Package Size Slicer
| Size | Total Sales |
|---|---|
| 2.5 kg | $23,786 |
| 1.0 kg | $11,011 |
| 0.5 kg | $7,030 |
| 0.2 kg | $3,308 |

- The **2.5kg** size dominates, accounting for over 52% of total revenue — customers are clearly buying in bulk.
- Revenue drops steeply as package size decreases, with the 0.2kg size contributing only ~7% of total sales.
- This suggests a strong value-buying behavior, and could indicate that promotions on large-format packs would be especially effective.

---


## 📊 Project image

<img width="804" height="394" alt="image" src="https://github.com/user-attachments/assets/1646e8ae-d91c-404d-9710-ea8f44883c6e" />

---

### 🎴 Loyalty Card Slicer
| Loyalty Card | Total Sales | Orders |
|---|---|---|
| No | $24,216 | 521 |
| Yes | $20,918 | 479 |

- Non-loyalty card holders actually account for more total revenue (~54%) and more orders (~52%).
- This is a notable finding: the loyalty program has not yet flipped spending behavior in favor of card holders.
- Filtering by loyalty card + roast type shows that **non-holders** dominate Light roast sales ($9,944 vs $7,411), which is the highest-revenue roast — meaning the most valuable segment is not enrolled in the loyalty program.

---

## 🛠 Tools Used

- **Microsoft Excel** — Pivot Tables, Pivot Charts, Slicers, Data Validation
- **Data Cleaning** — Lookup formulas (XLOOKUP / INDEX-MATCH) to enrich raw orders with product and customer details
- **Dashboard Design** — Interactive filters for Coffee Type, Roast Type, Package Size, and Loyalty Card status

---

## 🚀 How to Use

1. Download or clone this repository
2. Open `Coffee_Dashboard_Project.xlsx` in Microsoft Excel (2016 or later recommended)
3. Navigate to the **Dashboard** sheet
4. Use the slicers to filter by:
   - Roast Type (Light, Medium, Dark)
   - Package Size (0.2 kg, 0.5 kg, 1 kg, 2.5 kg)
   - Loyalty Card status (Yes / No)
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
