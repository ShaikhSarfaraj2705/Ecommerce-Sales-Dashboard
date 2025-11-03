# ECOMMERCE SALES DASHBOARD USING POWERBI 
```markdown
# 🛒 E-Commerce Sales Dashboard
 Interactive Power BI dashboard for analyzing e-commerce sales across states, categories, payment modes and time periods.
---

## 📌 Repository Contents



/Ecommerce-Sales-Dashboard
├─ README.md
├─ Ecommerce_Sales_Dashboard.pbix        # Power BI Desktop file (if included)
├─ data/
│  └─ ecommerce_sales.csv                # Example dataset (optional)
├─ assets/
│  └─ Screenshot%20(8).png              # Dashboard preview image
└─ docs/
└─ data_dictionary.md                # Column descriptions (optional)
````

---
## 📊 Dashboard Summary

**Key metrics shown**
- **Total Sales (Amount)**: 438K  
- **Total Profit**: 37K  
- **Total Quantity Sold**: 5615  
- **Average Order Value (AOV)**: 121K

**Main visuals**
- Sum of Amount by State (bar)
- Sum of Profit by Month (column)
- Sum of Quantity by Category (donut/pie)
- Sum of Amount by Customer Name (bar)
- Sum of Quantity by Payment Mode (donut/pie)
- Sum of Profit by Sub-Category (bar)
- Quarter and State slicers for dynamic filtering

---

## 🔧 Tools & Techniques

- **Power BI Desktop** (.pbix)
- Data source: CSV / Excel / Database
- Transformations: Power Query (M)
- Measures & calculations: DAX
- Visual design: custom theme (dark/purple), card visuals, donut & bar charts

---

## 🚀 Quick Start

1. Clone the repository:
```bash
git clone https://github.com/<your-username>/Ecommerce-Sales-Dashboard.git
cd Ecommerce-Sales-Dashboard
````

2. If a dataset is included, open `Ecommerce_Sales_Dashboard.pbix` in **Power BI Desktop** and verify data source paths.

3. If only CSV/Excel provided:

   * Open Power BI Desktop → **Get Data** → CSV / Excel → load `data/ecommerce_sales.csv`.
   * Recreate or import the `.pbix` file visuals.

---

## 🗂️ Data Requirements (example)

Your dataset should include (at minimum) the following columns:

* `OrderID` (string/number)
* `OrderDate` (date)
* `CustomerName` (string)
* `State` (string)
* `Category` (string)
* `SubCategory` (string)
* `PaymentMode` (string) — e.g., COD, UPI, Debit Card, Credit Card, EMI
* `Quantity` (number)
* `Amount` (number)
* `Profit` (number)

Add a `Month`/`Quarter` column or create them via DAX for time-based visuals.

---

## 🧾 Example DAX Measures

```dax
Total Amount = SUM('Sales'[Amount])
Total Profit = SUM('Sales'[Profit])
Total Quantity = SUM('Sales'[Quantity])
AOV = DIVIDE([Total Amount], DISTINCTCOUNT('Sales'[OrderID]))
Profit Margin % = DIVIDE([Total Profit], [Total Amount])
```

---

## 📷 Preview

<img width="1920" height="1080" alt="Ecommerce_sales" src="https://github.com/user-attachments/assets/2035c195-274c-4ef6-ad32-0a60cf66dfea" />

---

## 💡 Insights (from sample data)

* **Maharashtra** leads in sales amount.
* **Clothing** contributes the largest share of quantity sold (~63%).
* **COD** appears to be the most common payment mode.
* Profit spikes are visible in March and October — investigate campaigns or seasonality.

---

## 🤝 Contributing

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add feature"`
4. Push: `git push origin feature/your-feature`
5. Open a Pull Request.

Please include sample data or instructions to reproduce visuals when contributing.

---

---

*Replace placeholders (`<your-username>`, contact info, file names) with actual values before publishing.*

```

Would you like me to:  
- create this `README.md` file in the repo for you, or  
- generate a ready-to-download `README.md` file here?
```
