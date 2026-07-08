# LeetCode SQL 50 — My Solutions

My solutions to the [SQL 50](https://leetcode.com/studyplan/top-sql-50/) study plan on LeetCode, a curated set of 50 problems covering everything from basic `SELECT` filtering to window functions.

Each solution is written in **MySQL** syntax and tested on LeetCode before being committed here.

## 📁 Repository Structure

```
sql50/
├── 01-select/
│   ├── 1757-recyclable-and-low-fat-products.sql
│   ├── 584-find-customer-referee.sql
│   └── ...
├── 02-basic-joins/
│   ├── 1378-replace-employee-id.sql
│   └── ...
├── 03-basic-aggregation/
├── 04-sorting-and-grouping/
├── 05-advanced-select-and-joins/
├── 06-subqueries/
├── 07-advanced-string-functions/
└── README.md
```

Each `.sql` file contains:
- The query itself

Example:
```sql
SELECT name
FROM Customer
WHERE referee_id <> 2 OR referee_id IS NULL;
```

## ✅ Progress

| # | Category | Problems | Status |
|---|----------|----------|--------|
| 1 | Select | 5 | ⬜ 2/5 |
| 2 | Basic Joins | 5 | ⬜ 0/5 |
| 3 | Basic Aggregation | 5 | ⬜ 0/5 |
| 4 | Sorting and Grouping | 4 | ⬜ 0/4 |
| 5 | Advanced Select and Joins | 6 | ⬜ 0/6 |
| 6 | Subqueries | 5 | ⬜ 0/5 |
| 7 | Advanced String Functions / Regex / Clause | 5 | ⬜ 0/5 |

**Total: 2 / 50** — updated as I go.

## 🧠 Concepts Covered

- `SELECT`, `WHERE`, `DISTINCT`, `NULL` handling
- `INNER JOIN`, `LEFT JOIN`, self-joins
- Aggregate functions: `COUNT`, `SUM`, `AVG`, `MAX`, `MIN`
- `GROUP BY` + `HAVING`
- Subqueries (simple, correlated, `IN` / `NOT IN` / `EXISTS`)
- `CASE WHEN` conditional logic
- `UNION` / `UNION ALL`
- String functions: `CONCAT`, `SUBSTRING`, `LIKE`, `REGEXP`
- Date functions: `DATEDIFF`, `BETWEEN`
- Window functions: `RANK`, `DENSE_RANK`, `ROW_NUMBER`, `LAG`/`LEAD`, `SUM() OVER`

## 🛠 How to Run Locally

1. Install MySQL (or use Docker):
   ```bash
   docker run --name sql50-db -e MYSQL_ROOT_PASSWORD=root -p 3306:3306 -d mysql:8
   ```
2. Create the schema/sample data for a given problem (LeetCode provides `Create Table` / `Insert` statements on each problem page — save these under a `schemas/` folder if you want to test locally).
3. Run a solution file:
   ```bash
   mysql -u root -p < 01-select/1757-recyclable-and-low-fat-products.sql
   ```

## 📚 Reference

- Study plan: [LeetCode SQL 50](https://leetcode.com/studyplan/top-sql-50/)

## 📄 License

Solutions shared for learning purposes only.