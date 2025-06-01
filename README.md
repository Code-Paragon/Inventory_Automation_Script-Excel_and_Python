# 📊 Inventory Automation Script (Excel + Python)

A lightweight automation script that analyzes inventory data from an Excel file and generates insights such as stock valuation, supplier-wise totals, and low-stock alerts. Built with Python and `openpyxl`, it is perfect for small businesses or students learning automation with spreadsheets.

---

##  Features

-  Count of products per supplier
-  Total inventory value per supplier
-  Flag items with inventory < 10
-  Automatically adds "total value" column to Excel
-  Generates a new Excel file with calculated data

---

##  File Structure

```
main.py                        # Script for reading and writing Excel inventory
inventory.xlsx                 # Input inventory file
inventory_with_total_value.xlsx # Output file with calculations
requirements.txt               # Dependencies
```

---

##  Getting Started

**Install Requirements:**

```
pip install -r requirements.txt
```

## Prepare Your Excel File

Make sure inventory.xlsx has the following column layout (Sheet1):
|Product | ID	Inventory |	Price |	Supplier Name|

**Run the Script**
```
python main.py
```
**Output:**
- Displays key metrics in the terminal
- Creates a new file: inventory_with_total_value.xlsx

## Example Output
```
{
 'Supplier A': 3,
 'Supplier B': 2
}

{
 'Supplier A': 540.0,
 'Supplier B': 320.0
}

{
 101: 5,
 103: 8
}
```
