# SHREYAGUPTA_202401100400180
# 🛒 Market Basket Analysis using Apriori (Simulated Transactions)

This project performs **Market Basket Analysis** using the **Apriori algorithm** on a dataset containing only aisle-level product data. Since actual transactional data is missing, the script simulates transactions by grouping rows in fixed intervals.

---

## 📁 Dataset

**Filename:** `10. Market Basket Analysis.csv`  
**Columns:**
- `aisle_id`: Unique identifier for each aisle  
- `aisle`: Name of the aisle (e.g., "prepared soups salads", "granola bars")

⚠️ This dataset does **not** include real transaction data like order IDs or user purchases. The analysis uses **synthetic transactions** grouped by row index for demonstration purposes.

---

## 🔍 Objective

To simulate transaction behavior and perform **association rule mining** using:
- One-hot encoding
- Apriori algorithm
- Association rule metrics: **Support**, **Confidence**, and **Lift**
- Visualizing relationships between items

---

## ⚙️ Methodology

1. **Simulate Transactions**: Every 5 rows are grouped into a synthetic `transaction_id`.
2. **Basket Creation**: A one-hot encoded transaction-item matrix is generated using a pivot table.
3. **Apriori Algorithm**: Extracts frequent itemsets based on minimum support threshold.
4. **Association Rules**: Generated from the frequent itemsets using confidence and lift metrics.
5. **Visualization**: A scatter plot showing `Support` vs `Confidence`, color-coded by `Lift`.

---

## 📦 Dependencies

Install required packages using pip:

```bash
pip install pandas mlxtend matplotlib
