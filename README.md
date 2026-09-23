# E-Commerce Order Data Analysis

## 📌 Project Overview

This project is about cleaning, analyzing, and understanding an **E-Commerce Order Dataset** using Python and Pandas.

The dataset contains information about customers, products, orders, payment modes, quantities, prices, discounts, and ratings.

## 🛠️ Technologies Used

* Python
* Pandas
* Google Colab / Jupyter Notebook
* CSV

## 📂 Dataset

**File:** `Ecommerce_Order_Test_Dataset.csv`

* **Rows:** 101
* **Columns:** 13

### Columns

| Column          | Description       |
| --------------- | ----------------- |
| `Order_ID`      | Unique order ID   |
| `Order_Date`    | Date of order     |
| `Delivery_Date` | Delivery date     |
| `Customer_Name` | Customer name     |
| `Gender`        | Customer gender   |
| `City`          | Customer city     |
| `Category`      | Product category  |
| `Product`       | Product name      |
| `Payment_Mode`  | Payment method    |
| `Quantity`      | Quantity ordered  |
| `Unit_Price`    | Price of one unit |
| `Discount`      | Discount value    |
| `Rating`        | Customer rating   |

## 🔍 Tasks Performed

### Q1. Load and Inspect

* Loaded the CSV file into a DataFrame named `df`.
* Displayed the first 5 rows.
* Displayed the number of rows and columns.
* Displayed all column names.

### Q2. Understand the Dataset

* Used `info()` to display basic information.
* Used `describe()` to display the statistical summary of numerical columns.

### Q3. Handle Missing Values

* Found missing values in each column.
* Filled missing `City` values with `"Unknown"`.
* Filled missing `Customer_Name` values with `"Unknown"`.
* Filled missing `Rating` values with the mean rating.
* Filled missing `Payment_Mode` values with `"Unknown"`.

### Q4. Remove Duplicates

* Found the number of duplicate rows.
* Removed duplicate rows.
* Displayed the new shape of the DataFrame.

### Q6. Clean Text Data

Cleaned the following columns:

* `Gender`
* `City`
* `Payment_Mode`

Used `strip()` to remove unnecessary spaces and `title()` to make the text formatting consistent.

Displayed the unique values after cleaning.

### Q7. Create New Columns

Created three new columns.

**Total Price**

```text
Total Price = Quantity × Unit Price
```

**Discount Amount**

```text
Discount Amount = Total Price × Discount
```

**Final Amount**

```text
Final Amount = Total Price - Discount Amount
```

Displayed:

* Order ID
* Product
* Quantity
* Total Price
* Discount Amount
* Final Amount

### Q8. Numerical Analysis

Calculated:

1. Total quantity ordered
2. Average unit price
3. Maximum unit price
4. Minimum unit price
5. Average rating

### Q9. Filtering

Performed the following filtering operations:

1. Orders where `Quantity > 3`
2. Orders where `Rating >= 4.5`
3. Orders where `Final Amount > 5000`
4. Orders from `Chennai`

Only the required filtered feature/value was displayed for each condition.

### Q10. Sorting

* Sorted the dataset by `Final Amount` from highest to lowest.
* Displayed the top 5 orders.
* Displayed only:

  * `Order_ID`
  * `Product`
  * `Category`
  * `Quantity`
  * `Final Amount`

## 📊 Key Operations Used

Some important Pandas functions used in this project:

```python
pd.read_csv()
df.head()
df.shape
df.columns
df.info()
df.describe()
df.isnull().sum()
df.fillna()
df.duplicated()
df.drop_duplicates()
df.sort_values()
df.loc[]
df.unique()
```

## 🎯 Objective

The main objective of this project is to learn the basic steps of **data preprocessing and analysis using Pandas**.

The project covers:

* Data loading
* Data inspection
* Missing value handling
* Duplicate removal
* Text cleaning
* Feature creation
* Numerical analysis
* Data filtering
* Data sorting

## 📁 Project Structure

```text
E-Commerce-Order-Analysis/
│
├── Ecommerce_Order_Test_Dataset.csv
├── ecommerce_order_analysis.ipynb
└── README.md
```

## ✅ Conclusion

This project demonstrates how **Python and Pandas** can be used to clean and analyze an E-Commerce dataset.

The dataset was successfully inspected, cleaned, processed, filtered, and sorted to obtain useful information about customer orders, quantities, prices, discounts, final amounts, and ratings.
