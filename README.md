# DATA-ANALYSIS-USING-SQL
Data loading on SQL server from csv files , analyse them &amp; generate necessary output of queries
# SQL Data Analysis Project

## 📌 Project Overview
This project demonstrates **SQL-based data analysis** on a retail sales dataset.  
It involves creating relational tables, loading CSV data, and running analytical queries to uncover business insights such as sales trends, customer behavior, and store performance.

## 📂 Dataset Description
The dataset contains **4 CSV files** representing different entities in a retail business:

| File Name       | Description |
|----------------|-------------|
| `customers.csv` | Customer details including name, city, state, and join date |
| `products.csv`  | Product details such as name, category, and price |
| `sales.csv`     | Transactional sales records with quantity, date, and related IDs |
| `stores.csv`    | Store details including location and name |

### **Data Preview**
#### customers.csv
| customer_id | name           | city         | state | join_date |
|-------------|---------------|--------------|-------|-----------|
| 1           | Laura Taylor  | New York     | NY    | 2023-04-24 |
| 2           | Emily Davis   | Los Angeles  | CA    | 2023-08-14 |

#### products.csv
| product_id | product_name   | category       | price |
|------------|---------------|----------------|-------|
| 101        | Laptop X1     | Electronics    | 899   |
| 102        | Coffee Maker  | Home Appliance | 120   |

#### sales.csv
| sale_id | customer_id | product_id | quantity | sale_date  | store_id |
|---------|-------------|------------|----------|------------|----------|
| 1       | 15          | 106        | 2        | 2023-03-01 | 4        |
| 2       | 9           | 107        | 5        | 2023-04-16 | 5        |

#### stores.csv
| store_id | store_name    | city        | state |
|----------|--------------|-------------|-------|
| 1        | Midtown      | New York    | NY    |
| 2        | Downtown     | Los Angeles | CA    |

---

## 🗄 Database Schema
The SQL script `Project SQL.sql` creates the following tables:
- **customers**
- **products**
- **sales**
- **stores**

**Relationships:**
- `sales.customer_id` → `customers.customer_id`
- `sales.product_id` → `products.product_id`
- `sales.store_id` → `stores.store_id`

---

## 📊 Analysis Performed
The SQL script contains queries to:
- Calculate **total revenue and units sold**
- Analyze **monthly sales trends**
- Find **top-selling products**
- Identify **best-performing stores**
- Compare **new vs. returning customers**
- Measure **customer lifetime value**

---

## 🚀 How to Run
1. Import the CSV files into your SQL environment (PostgreSQL, MySQL, etc.).
2. Execute the `Project SQL.sql` file to create tables and run analysis queries.
3. Modify queries to explore additional insights.

---

## 💡 Potential Improvements
- Add **visualizations** (e.g., in Power BI, Tableau, or Python)
- Perform **customer segmentation** analysis
- Integrate **forecasting models** for sales prediction

---

## 📜 License
This project is open-source. You can use and modify it for learning purposes.
