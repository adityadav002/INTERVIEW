# 🗃️ MySQL Interview Questions & Solutions

> A complete, beginner-friendly handbook for mastering SQL through 50 real interview-style questions — with line-by-line explanations, execution logic, complexity analysis, and interview tips.

---

## 📖 About This Repository

### Purpose

This repository turns a curated list of classic MySQL interview questions into a structured **learning handbook**, not just an answer key. Every question is broken down into the *why* behind the query, not just the *what*.

### Who This Is For

- 🎓 Beginners learning SQL for the first time
- 💼 Job seekers preparing for data analyst, data engineer, backend, or BI interviews
- 🧑‍🏫 Students who want to understand SQL logic, not memorize syntax
- 🔁 Experienced engineers who want a quick refresher before interviews

### What You Will Learn

By working through this repository in order, you will learn how to:

- Filter, sort, and group data using `WHERE`, `GROUP BY`, and `HAVING`
- Combine tables using `INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`, and self-joins
- Use aggregate functions (`COUNT`, `SUM`, `AVG`, `MIN`, `MAX`)
- Write subqueries and correlated subqueries
- Use window functions like `DENSE_RANK()` and `SUM() OVER()`
- Handle `NULL` values correctly
- Work with dates, strings, and conditional logic (`CASE`)
- Reason about query performance and indexing

### Difficulty Levels

| Level | Meaning |
|-------|---------|
| 🟢 Easy | Single-table or simple two-table logic. Good for building fundamentals. |
| 🟡 Medium | Multiple joins, subqueries, or aggregation logic. Common in real interviews. |
| 🔴 Hard | Window functions, ranking logic, or multi-step reasoning. Senior-level interview material. |

### SQL Topics Covered

| Topic | Example Questions |
|-------|--------------------|
| Basic `SELECT` / `WHERE` | #1, #2, #3, #4, #5 |
| `JOIN` / `LEFT JOIN` | #6, #7, #8, #11, #12 |
| `GROUP BY` / `HAVING` | #13, #23, #26, #27, #28, #29 |
| Aggregate Functions | #10, #16, #17, #19, #30 |
| Subqueries | #18, #21, #25, #34, #47 |
| `CASE` Expressions | #14, #20, #32, #36, #38 |
| Date Functions | #9, #20, #24, #34, #49 |
| String Functions | #5, #44, #45, #50 |
| `UNION` / `UNION ALL` | #31, #36, #39, #41 |
| Window Functions | #35, #40, #43 |
| Self Joins | #9, #13, #30, #33 |
| `DELETE` Statements | #46 |

---

## 📚 Table of Contents

| # | Question | Difficulty | Category |
|---|----------|------------|----------|
| 1 | [Recyclable and Low Fat Products](#1-recyclable-and-low-fat-products) | 🟢 Easy | Basic SELECT / WHERE |
| 2 | [Find Customer Referee](#2-find-customer-referee) | 🟢 Easy | WHERE / NULL Handling |
| 3 | [Big Countries](#3-big-countries) | 🟢 Easy | WHERE / Logical OR |
| 4 | [Article Views I](#4-article-views-i) | 🟢 Easy | SELECT DISTINCT |
| 5 | [Invalid Tweets](#5-invalid-tweets) | 🟢 Easy | WHERE / String Functions |
| 6 | [Replace Employee ID With The Unique Identifier](#6-replace-employee-id-with-the-unique-identifier) | 🟢 Easy | LEFT JOIN |
| 7 | [Product Sales Analysis I](#7-product-sales-analysis-i) | 🟢 Easy | INNER JOIN |
| 8 | [Customer Who Visited but Did Not Make Any Transactions](#8-customer-who-visited-but-did-not-make-any-transactions) | 🟢 Easy | LEFT JOIN / Aggregation |
| 9 | [Rising Temperature](#9-rising-temperature) | 🟢 Easy | Self JOIN / Date Functions |
| 10 | [Average Time of Process per Machine](#10-average-time-of-process-per-machine) | 🟡 Medium | Self JOIN / Aggregation |
| 11 | [Employee Bonus](#11-employee-bonus) | 🟢 Easy | LEFT JOIN / NULL Handling |
| 12 | [Students and Examinations](#12-students-and-examinations) | 🟢 Easy | CROSS JOIN / LEFT JOIN |
| 13 | [Managers with at Least 5 Direct Reports](#13-managers-with-at-least-5-direct-reports) | 🟡 Medium | GROUP BY / HAVING |
| 14 | [Confirmation Rate](#14-confirmation-rate) | 🟡 Medium | LEFT JOIN / CASE / AVG |
| 15 | [Not Boring Movies](#15-not-boring-movies) | 🟢 Easy | WHERE / ORDER BY |
| 16 | [Average Selling Price](#16-average-selling-price) | 🟢 Easy | LEFT JOIN / Aggregation |
| 17 | [Project Employees I](#17-project-employees-i) | 🟢 Easy | JOIN / AVG |
| 18 | [Percentage of Users Attended a Contest](#18-percentage-of-users-attended-a-contest) | 🟡 Medium | Subquery / Aggregation |
| 19 | [Queries Quality and Percentage](#19-queries-quality-and-percentage) | 🟢 Easy | GROUP BY / CASE |
| 20 | [Monthly Transactions I](#20-monthly-transactions-i) | 🟡 Medium | GROUP BY / Date Functions |
| 21 | [Immediate Food Delivery II](#21-immediate-food-delivery-ii) | 🟡 Medium | Subquery / Aggregation |
| 22 | [Game Play Analysis IV](#22-game-play-analysis-iv) | 🟡 Medium | Subquery / Date Functions |
| 23 | [Number of Unique Subjects Taught by Each Teacher](#23-number-of-unique-subjects-taught-by-each-teacher) | 🟢 Easy | GROUP BY / COUNT DISTINCT |
| 24 | [User Activity for the Past 30 Days I](#24-user-activity-for-the-past-30-days-i) | 🟡 Medium | WHERE / Date Range |
| 25 | [Product Sales Analysis III](#25-product-sales-analysis-iii) | 🟡 Medium | Subquery |
| 26 | [Classes With at Least 5 Students](#26-classes-with-at-least-5-students) | 🟢 Easy | GROUP BY / HAVING |
| 27 | [Find Followers Count](#27-find-followers-count) | 🟢 Easy | GROUP BY / COUNT |
| 28 | [Biggest Single Number](#28-biggest-single-number) | 🟢 Easy | Subquery / HAVING |
| 29 | [Customers Who Bought All Products](#29-customers-who-bought-all-products) | 🟡 Medium | GROUP BY / HAVING / Subquery |
| 30 | [The Number of Employees Which Report to Each Employee](#30-the-number-of-employees-which-report-to-each-employee) | 🟢 Easy | Self JOIN / Aggregation |
| 31 | [Primary Department for Each Employee](#31-primary-department-for-each-employee) | 🟢 Easy | UNION / GROUP BY |
| 32 | [Triangle Judgement](#32-triangle-judgement) | 🟢 Easy | CASE |
| 33 | [Consecutive Numbers](#33-consecutive-numbers) | 🟡 Medium | Self JOIN |
| 34 | [Product Price at a Given Date](#34-product-price-at-a-given-date) | 🟡 Medium | Subquery / LEFT JOIN |
| 35 | [Last Person to Fit in the Bus](#35-last-person-to-fit-in-the-bus) | 🟡 Medium | Window Function |
| 36 | [Count Salary Categories](#36-count-salary-categories) | 🟡 Medium | CASE / UNION |
| 37 | [Employees Whose Manager Left the Company](#37-employees-whose-manager-left-the-company) | 🟢 Easy | LEFT JOIN / Subquery |
| 38 | [Exchange Seats](#38-exchange-seats) | 🟡 Medium | CASE / Modulo |
| 39 | [Movie Rating](#39-movie-rating) | 🟡 Medium | UNION / JOIN |
| 40 | [Restaurant Growth](#40-restaurant-growth) | 🟡 Medium | Window Function |
| 41 | [Friend Requests II: Who Has the Most Friends](#41-friend-requests-ii-who-has-the-most-friends) | 🟡 Medium | UNION ALL / GROUP BY |
| 42 | [Investments in 2016](#42-investments-in-2016) | 🟡 Medium | Subquery / GROUP BY |
| 43 | [Department Top Three Salaries](#43-department-top-three-salaries) | 🔴 Hard | Window Function (DENSE_RANK) |
| 44 | [Fix Names in a Table](#44-fix-names-in-a-table) | 🟢 Easy | String Functions |
| 45 | [Patients With a Condition](#45-patients-with-a-condition) | 🟢 Easy | LIKE |
| 46 | [Delete Duplicate Emails](#46-delete-duplicate-emails) | 🟢 Easy | DELETE / Self JOIN |
| 47 | [Second Highest Salary](#47-second-highest-salary) | 🟢 Easy | Subquery / LIMIT OFFSET |
| 48 | [Group Sold Products By The Date](#48-group-sold-products-by-the-date) | 🟡 Medium | GROUP_CONCAT |
| 49 | [List the Products Ordered in a Period](#49-list-the-products-ordered-in-a-period) | 🟢 Easy | JOIN / HAVING |
| 50 | [Find Users With Valid E-Mails](#50-find-users-with-valid-e-mails) | 🟢 Easy | REGEXP |

---

## 🧭 How to Use This Repository

Every question in this handbook follows the same structure, so you always know where to look:

| Section | What it gives you |
|---|---|
| **Problem** | A plain-English explanation of the task (no LeetCode copy-paste) |
| **SQL Solution** | A clean, properly formatted, working MySQL query |
| **Explanation** | A line-by-line breakdown of every clause used |
| **Why This Solution Works** | The logical reasoning behind the query |
| **SQL Concepts Used** | A quick checklist of concepts you just practiced |
| **Interview Tip** | What interviewers are really testing, and common mistakes |
| **Time / Space Complexity** | How the query performs and scales |
| **Alternative Solution** | A different way to solve the same problem |
| **Key Takeaways** | A summary you can review quickly before an interview |

If you are new to SQL, read the questions **in order** — they are arranged from simple filtering to advanced window functions. If you are revising for an interview, jump straight to the topic you need using the Table of Contents above.

---

## 1. Recyclable and Low Fat Products

**Difficulty:** 🟢 Easy
**Category:** Basic SELECT / WHERE

---

### 📋 Problem

You have a `Products` table with columns `product_id`, `low_fats` (`'Y'`/`'N'`), and `recyclable` (`'Y'`/`'N'`). Find the IDs of products that are **both** low fat **and** recyclable.

```
Products
+-------------+-------------+-------------+
| product_id  | low_fats    | recyclable  |
+-------------+-------------+-------------+
```

### 💻 SQL Solution

```sql
SELECT product_id
FROM Products
WHERE low_fats = 'Y'
  AND recyclable = 'Y';
```

### 🔍 Explanation

- `SELECT product_id`: We only need the ID column in the output, not the whole row.
- `FROM Products`: Tells MySQL which table to read from.
- `WHERE low_fats = 'Y'`: Keeps only rows where the product is marked low fat.
- `AND recyclable = 'Y'`: Adds a second condition — both conditions must be true for a row to be kept. `AND` means every condition in the chain has to pass.

### ✅ Why This Solution Works

`WHERE` filters rows **before** any output is produced. MySQL scans every row and checks both conditions; only rows passing both survive. Since we want products that satisfy two independent criteria at the same time, chaining them with `AND` is the natural translation of "both X and Y" into SQL logic.

### 🧠 SQL Concepts Used

- ✔ SELECT
- ✔ WHERE
- ✔ Logical AND
- ✔ Filtering on multiple columns

### 💡 Interview Tip

- This question checks whether you understand that `WHERE` conditions are combined with `AND`/`OR`, not commas.
- **Common mistake:** writing `WHERE low_fats AND recyclable = 'Y'`, which is invalid — every condition needs its own comparison.
- **Edge case:** the values are stored as `'Y'`/`'N'` strings, not booleans — always match the exact type used in the schema.

### ⏱ Time Complexity

Without an index: **O(n)** — every row must be scanned once.
With an index on `(low_fats, recyclable)`: closer to **O(log n) + O(k)**, where `k` is the number of matching rows, since the index narrows down candidate rows quickly.

### 💾 Space Complexity

**O(1)** additional space — the query returns existing rows without building any intermediate structures.

### 🔄 Alternative Solution

```sql
-- Using IN, useful if you want to extend this to more flag combinations later
SELECT product_id
FROM Products
WHERE low_fats IN ('Y')
  AND recyclable IN ('Y');
```

This form doesn't change performance here, but it becomes handy if the flag column ever supports more than two values.

### 🎯 Key Takeaways

- `WHERE` filters rows before they're returned.
- `AND` requires all conditions to be true simultaneously.
- Always match literal values to the exact data type/format used in the table.

---

## 2. Find Customer Referee

**Difficulty:** 🟢 Easy
**Category:** WHERE / NULL Handling

---

### 📋 Problem

A `Customer` table has `id`, `name`, and `referee_id` (the ID of the customer who referred them). Find the names of customers who were **not** referred by the customer with `id = 2`.

### 💻 SQL Solution

```sql
SELECT name
FROM Customer
WHERE referee_id <> 2
   OR referee_id IS NULL;
```

### 🔍 Explanation

- `SELECT name`: We only want customer names in the result.
- `FROM Customer`: Source table.
- `WHERE referee_id <> 2`: Keeps rows where the referee is *not* customer 2. `<>` means "not equal to."
- `OR referee_id IS NULL`: Also keeps customers who have **no referee at all**. This is critical — in SQL, `NULL <> 2` evaluates to `NULL` (unknown), not `TRUE`, so rows with a `NULL` referee would silently disappear if we forgot this clause.

### ✅ Why This Solution Works

SQL's three-valued logic (`TRUE`, `FALSE`, `UNKNOWN`) means any comparison against `NULL` returns `UNKNOWN`, and `WHERE` only keeps rows that evaluate to `TRUE`. Because some customers were never referred by anyone, their `referee_id` is `NULL`, and a plain `<>` check would incorrectly exclude them. Explicitly adding `OR referee_id IS NULL` fixes this gap.

### 🧠 SQL Concepts Used

- ✔ SELECT
- ✔ WHERE
- ✔ Logical OR
- ✔ NULL Handling (`IS NULL`)
- ✔ Comparison Operators

### 💡 Interview Tip

- This is one of the most common **NULL-trap** questions in SQL interviews.
- **Common mistake:** using `WHERE referee_id != 2` alone and silently dropping customers with no referee.
- Interviewers use this to check if you understand that `NULL` is never "equal" or "not equal" to anything, including itself.

### ⏱ Time Complexity

Without an index: **O(n)**, full table scan.
With an index on `referee_id`: still close to **O(n)** for this query because we're selecting "not equal," which indexes generally can't narrow down efficiently — indexes are best for equality and range lookups, not "not equal" conditions.

### 💾 Space Complexity

**O(1)** — no extra structures are built.

### 🔄 Alternative Solution

```sql
-- Using IFNULL to normalize NULLs to a safe placeholder value
SELECT name
FROM Customer
WHERE IFNULL(referee_id, 0) <> 2;
```

`IFNULL(referee_id, 0)` replaces `NULL` with `0` before comparing, so the comparison always resolves to `TRUE` or `FALSE` — useful when you want a single condition instead of an `OR`.

### 🎯 Key Takeaways

- `NULL` is never equal to, or not equal to, any value — including another `NULL`.
- Always ask "could this column be NULL?" before writing a `<>` or `=` filter.
- `IFNULL`/`COALESCE` are common tools for normalizing NULLs inside conditions.

---

## 3. Big Countries

**Difficulty:** 🟢 Easy
**Category:** WHERE / Logical OR

---

### 📋 Problem

A `World` table stores `name`, `continent`, `area`, `population`, and `gdp` for each country. A country is considered "big" if its area is at least 3,000,000 km² **or** its population is at least 25,000,000. Return the name, population, and area of all big countries.

### 💻 SQL Solution

```sql
SELECT name, population, area
FROM World
WHERE area >= 3000000
   OR population >= 25000000;
```

### 🔍 Explanation

- `SELECT name, population, area`: Only these three columns are needed in the output — `continent` and `gdp` are ignored.
- `FROM World`: Source table.
- `WHERE area >= 3000000`: Keeps countries meeting the area threshold.
- `OR population >= 25000000`: Also keeps countries meeting the population threshold, even if they fail the area check. `OR` means a row is kept if **either** condition is true.

### ✅ Why This Solution Works

The definition of "big" is a union of two independent criteria — a country only needs to satisfy one of them. `OR` mirrors this directly: MySQL evaluates each condition per row and keeps the row if at least one is true.

### 🧠 SQL Concepts Used

- ✔ SELECT
- ✔ WHERE
- ✔ Logical OR
- ✔ Comparison Operators

### 💡 Interview Tip

- Interviewers use this to see if you confuse `AND`/`OR` when translating "or" from plain English into SQL.
- **Common mistake:** using `AND` instead of `OR`, which would incorrectly require both conditions to hold at once — dramatically shrinking the result set.
- **Edge case:** think about countries exactly at the threshold (`area = 3000000`) — `>=` includes them, `>` would not.

### ⏱ Time Complexity

Without an index: **O(n)**.
With separate indexes on `area` and `population`: MySQL can use **index merge (union)** to combine two range scans, but for an `OR` across two different columns, a full scan is often still what the optimizer chooses unless the table is very large.

### 💾 Space Complexity

**O(1)** — direct filtering and projection, no intermediate storage needed.

### 🔄 Alternative Solution

```sql
-- Using UNION to combine two separate filtered queries
SELECT name, population, area FROM World WHERE area >= 3000000
UNION
SELECT name, population, area FROM World WHERE population >= 25000000;
```

`UNION` automatically removes duplicate rows (countries satisfying both conditions appear once), which is useful if you prefer expressing this as "combine these two independent result sets" instead of a single filter.

### 🎯 Key Takeaways

- `OR` keeps a row if any one condition is true; `AND` requires all conditions to be true.
- `UNION` can express "either of these queries' results" while automatically de-duplicating.
- Always double check boundary conditions (`>=` vs `>`).

---

## 4. Article Views I

**Difficulty:** 🟢 Easy
**Category:** SELECT DISTINCT

---

### 📋 Problem

A `Views` table logs `article_id`, `author_id`, `viewer_id`, and `view_date` — one row per view. Find all authors who have viewed **their own** articles at least once, sorted by ID.

### 💻 SQL Solution

```sql
SELECT DISTINCT author_id AS id
FROM Views
WHERE author_id = viewer_id
ORDER BY id;
```

### 🔍 Explanation

- `SELECT DISTINCT author_id AS id`: Returns unique author IDs, renamed to `id` to match the expected output column name. `DISTINCT` removes duplicate rows from the result set.
- `FROM Views`: Source table.
- `WHERE author_id = viewer_id`: Keeps only rows where the person viewing the article is the same person who wrote it.
- `ORDER BY id`: Sorts the final result in ascending order by ID.

### ✅ Why This Solution Works

Since one author may have viewed their own article multiple times (multiple matching rows), simply selecting `author_id` would produce duplicates. `DISTINCT` collapses these into one row per author, giving exactly the unique list the question asks for.

### 🧠 SQL Concepts Used

- ✔ SELECT DISTINCT
- ✔ WHERE
- ✔ Column Aliasing (AS)
- ✔ ORDER BY

### 💡 Interview Tip

- This tests whether you remember `DISTINCT` when a query could otherwise return repeated values.
- **Common mistake:** forgetting `ORDER BY`, which many interview platforms explicitly require even if not always graded.
- **Edge case:** an author who never views their own articles should not appear at all — the `WHERE` clause naturally handles this by excluding non-matching rows.

### ⏱ Time Complexity

Without an index: **O(n)** to scan, plus **O(n log n)** for the `DISTINCT`/`ORDER BY` sort step (MySQL often computes both via a sort or temporary table).
With an index on `(author_id, viewer_id)`: filtering becomes closer to **O(log n) + O(k)**, and if the index is on `author_id` already, the sort step may be avoided entirely.

### 💾 Space Complexity

**O(k)**, where `k` is the number of distinct matching authors — MySQL needs to temporarily track which values it has already seen to remove duplicates.

### 🔄 Alternative Solution

```sql
-- Using GROUP BY instead of DISTINCT
SELECT author_id AS id
FROM Views
WHERE author_id = viewer_id
GROUP BY author_id
ORDER BY id;
```

`GROUP BY` achieves the same de-duplication as `DISTINCT` here since we aren't aggregating anything — useful to know both approaches are interchangeable in simple cases like this.

### 🎯 Key Takeaways

- `DISTINCT` removes duplicate rows from the final result set.
- `GROUP BY` can also de-duplicate, even without aggregate functions.
- Self-referencing conditions like `author_id = viewer_id` are a common pattern for "did X happen to themselves" questions.

---

## 5. Invalid Tweets

**Difficulty:** 🟢 Easy
**Category:** WHERE / String Functions

---

### 📋 Problem

A `Tweets` table has `tweet_id` and `content`. A tweet is invalid if its content is **longer than 15 characters**. Return the IDs of all invalid tweets.

### 💻 SQL Solution

```sql
SELECT tweet_id
FROM Tweets
WHERE CHAR_LENGTH(content) > 15;
```

### 🔍 Explanation

- `SELECT tweet_id`: Only the ID is needed in the output.
- `FROM Tweets`: Source table.
- `WHERE CHAR_LENGTH(content) > 15`: `CHAR_LENGTH()` counts the number of characters in a string (not bytes, which matters for multi-byte characters like emojis). The condition keeps only tweets whose content exceeds 15 characters.

### ✅ Why This Solution Works

The problem defines "invalid" purely by character count, so applying a string-length function directly inside `WHERE` is the most direct translation of the rule. MySQL computes the length for every row and compares it against the threshold.

### 🧠 SQL Concepts Used

- ✔ SELECT
- ✔ WHERE
- ✔ String Functions (CHAR_LENGTH)

### 💡 Interview Tip

- Interviewers use this to check if you know the difference between `CHAR_LENGTH()` (characters) and `LENGTH()` (bytes) — they differ for multi-byte encodings like UTF-8 emojis.
- **Common mistake:** using `LENGTH()` blindly, which can give wrong results for non-ASCII text.
- **Edge case:** a tweet with exactly 15 characters is **valid**, not invalid — the condition must be strictly `> 15`.

### ⏱ Time Complexity

**O(n)** — `CHAR_LENGTH()` must be computed per row, so no ordinary index can be used directly unless a generated/virtual column storing the length is indexed separately.

### 💾 Space Complexity

**O(1)** — no additional storage beyond the output rows.

### 🔄 Alternative Solution

```sql
-- Using LENGTH() when content is guaranteed to be plain ASCII
SELECT tweet_id
FROM Tweets
WHERE LENGTH(content) > 15;
```

This works identically for ASCII-only text but can silently produce wrong results for multi-byte characters — good to mention in an interview as a "gotcha" you're aware of.

### 🎯 Key Takeaways

- `CHAR_LENGTH()` counts characters; `LENGTH()` counts bytes — they diverge for non-ASCII text.
- String functions can be used directly inside `WHERE` for filtering.
- Watch strict inequality boundaries (`>` vs `>=`) carefully.

---

## 6. Replace Employee ID With The Unique Identifier

**Difficulty:** 🟢 Easy
**Category:** LEFT JOIN

---

### 📋 Problem

An `Employees` table has `id` and `name`. An `EmployeeUNI` table maps some of those `id`s to a `unique_id`. Not every employee has a `unique_id`. Return each employee's `unique_id` (or `NULL` if none exists) alongside their `name`.

### 💻 SQL Solution

```sql
SELECT eu.unique_id, e.name
FROM Employees e
LEFT JOIN EmployeeUNI eu
  ON e.id = eu.id;
```

### 🔍 Explanation

- `SELECT eu.unique_id, e.name`: Pulls the unique ID from `EmployeeUNI` and the name from `Employees`.
- `FROM Employees e`: `Employees` is the "base" table — every employee must appear in the output regardless of whether a match exists.
- `LEFT JOIN EmployeeUNI eu ON e.id = eu.id`: Attaches matching rows from `EmployeeUNI`. If no match is found for an employee, MySQL fills in `NULL` for `eu.unique_id` instead of dropping the row.

### ✅ Why This Solution Works

`LEFT JOIN` guarantees every row from the left table (`Employees`) survives, whether or not it has a partner in the right table (`EmployeeUNI`). This exactly matches the requirement that employees without a `unique_id` should still show up, just with `NULL` in that column.

### 🧠 SQL Concepts Used

- ✔ SELECT
- ✔ LEFT JOIN
- ✔ Table Aliasing
- ✔ NULL propagation on unmatched rows

### 💡 Interview Tip

- This tests whether you reach for `LEFT JOIN` instead of `INNER JOIN` when the question implies "keep everyone, even without a match."
- **Common mistake:** using `INNER JOIN`, which silently drops employees with no `unique_id` — a subtle bug that's easy to miss without reading requirements carefully.
- **Edge case:** what happens if `EmployeeUNI` has an `id` that doesn't exist in `Employees`? With `LEFT JOIN`, it simply wouldn't appear, since `Employees` is the driving table.

### ⏱ Time Complexity

Without an index: **O(n × m)** in the worst case (nested loop join).
With an index on `EmployeeUNI.id`: **O(n log m)**, since MySQL can look up matches for each employee row instead of scanning the entire second table.

### 💾 Space Complexity

**O(1)** beyond the output — no grouping or sorting buffers are needed.

### 🔄 Alternative Solution

```sql
-- Using a correlated subquery instead of a JOIN
SELECT
  (SELECT unique_id FROM EmployeeUNI eu WHERE eu.id = e.id) AS unique_id,
  e.name
FROM Employees e;
```

This produces the same result but can be slower on large tables since the subquery re-executes conceptually for every row, whereas `LEFT JOIN` lets the optimizer plan a single combined scan.

### 🎯 Key Takeaways

- `LEFT JOIN` keeps all rows from the left table even without a match.
- `INNER JOIN` would silently drop unmatched rows — always check if that's actually what's wanted.
- Correlated subqueries can replace simple joins but are usually less efficient.

---

## 7. Product Sales Analysis I

**Difficulty:** 🟢 Easy
**Category:** INNER JOIN

---

### 📋 Problem

A `Sales` table records `sale_id`, `product_id`, `year`, `quantity`, and `price`. A `Product` table maps `product_id` to `product_name`. Return the product name, year, and price for every sale.

### 💻 SQL Solution

```sql
SELECT p.product_name, s.year, s.price
FROM Sales s
JOIN Product p
  ON s.product_id = p.product_id;
```

### 🔍 Explanation

- `SELECT p.product_name, s.year, s.price`: Combines a column from `Product` with two columns from `Sales`.
- `FROM Sales s`: Starts from the sales records.
- `JOIN Product p ON s.product_id = p.product_id`: An `INNER JOIN` (the default when you just write `JOIN`) matches each sale to its corresponding product using the shared `product_id`. Only rows with a match on both sides are kept.

### ✅ Why This Solution Works

Every sale is expected to reference a valid product, so an `INNER JOIN` — which only keeps rows that match in both tables — is sufficient and correctly links each transaction to its product's name.

### 🧠 SQL Concepts Used

- ✔ SELECT
- ✔ INNER JOIN
- ✔ Table Aliasing
- ✔ Multi-table Column Selection

### 💡 Interview Tip

- Interviewers use this as a baseline join question — the follow-up is often "what if some `product_id`s in Sales don't exist in Product?" (Answer: those rows would disappear with `INNER JOIN`, which is why understanding the difference from `LEFT JOIN` matters.)
- **Common mistake:** forgetting the join condition entirely, which produces a cartesian product (every sale matched with every product).
- **Edge case:** duplicate `product_id`s in `Product` would cause sales rows to be duplicated in the output — a good reason `product_id` should be a primary key there.

### ⏱ Time Complexity

Without an index: **O(n × m)**.
With an index on `Product.product_id` (typically the primary key): **O(n log m)**, since each sale row can efficiently look up its matching product.

### 💾 Space Complexity

**O(1)** — no aggregation, just row-by-row combination.

### 🔄 Alternative Solution

```sql
-- Explicit INNER JOIN keyword for clarity
SELECT p.product_name, s.year, s.price
FROM Sales s
INNER JOIN Product p
  ON s.product_id = p.product_id;
```

Functionally identical — writing `INNER JOIN` explicitly instead of just `JOIN` is a style preference many teams enforce for readability.

### 🎯 Key Takeaways

- `JOIN` and `INNER JOIN` are the same thing in MySQL.
- Inner joins only return rows with matches on both sides.
- A missing or incorrect join key can silently create duplicate or missing rows.

---

## 8. Customer Who Visited but Did Not Make Any Transactions

**Difficulty:** 🟢 Easy
**Category:** LEFT JOIN / Aggregation

---

### 📋 Problem

A `Visits` table logs `visit_id` and `customer_id`. A `Transactions` table logs `transaction_id`, `visit_id`, and `amount`. Some visits never resulted in a transaction. For each customer, count how many of their visits had **no transaction**.

### 💻 SQL Solution

```sql
SELECT v.customer_id, COUNT(v.visit_id) AS count_no_trans
FROM Visits v
LEFT JOIN Transactions t
  ON v.visit_id = t.visit_id
WHERE t.transaction_id IS NULL
GROUP BY v.customer_id;
```

### 🔍 Explanation

- `SELECT v.customer_id, COUNT(v.visit_id) AS count_no_trans`: Returns each customer alongside a count of their qualifying visits.
- `FROM Visits v`: Every visit is the starting point.
- `LEFT JOIN Transactions t ON v.visit_id = t.visit_id`: Attaches any transaction tied to that visit — if none exists, all `Transactions` columns come back as `NULL`.
- `WHERE t.transaction_id IS NULL`: Keeps only visits that had no matching transaction — this is the key filter that isolates "visited but didn't buy."
- `GROUP BY v.customer_id`: Groups the remaining rows by customer so `COUNT()` can tally visits per person.
- `COUNT(v.visit_id)`: Counts non-null `visit_id` values per group — since every visit has an ID, this effectively counts rows per customer.

### ✅ Why This Solution Works

The pattern "`LEFT JOIN` + `WHERE right_table.key IS NULL`" is the standard way to find rows in the left table that have **no counterpart** in the right table. Once we've isolated those "orphan" visits, grouping by customer and counting gives us the per-customer total.

### 🧠 SQL Concepts Used

- ✔ LEFT JOIN
- ✔ WHERE
- ✔ IS NULL
- ✔ GROUP BY
- ✔ COUNT()

### 💡 Interview Tip

- This is a textbook **anti-join** pattern — extremely common in interviews ("find users who never did X").
- **Common mistake:** using `INNER JOIN`, which would remove exactly the rows we need (the ones with no transaction).
- **Edge case:** a customer with zero visits at all wouldn't appear in the result — the question only asks about customers who visited, so this is correct behavior.

### ⏱ Time Complexity

Without an index: **O(n × m)** for the join, plus **O(n log n)** for grouping.
With an index on `Transactions.visit_id`: the join becomes **O(n log m)**, and grouping can also benefit from an index on `Visits.customer_id`.

### 💾 Space Complexity

**O(k)**, where `k` is the number of distinct customers, to hold the grouped counts.

### 🔄 Alternative Solution

```sql
-- Using NOT IN with a subquery
SELECT customer_id, COUNT(*) AS count_no_trans
FROM Visits
WHERE visit_id NOT IN (SELECT visit_id FROM Transactions)
GROUP BY customer_id;
```

Simpler to read, but be cautious: `NOT IN` behaves unexpectedly if the subquery can return `NULL` values — in that case, prefer `NOT EXISTS` instead.

### 🎯 Key Takeaways

- `LEFT JOIN` + `WHERE ... IS NULL` is the standard anti-join pattern.
- `NOT IN` with subqueries can be dangerous if `NULL`s are involved — `NOT EXISTS` is often safer.
- Always group only after filtering, so aggregates reflect the correct subset of rows.

---

## 9. Rising Temperature

**Difficulty:** 🟢 Easy
**Category:** Self JOIN / Date Functions

---

### 📋 Problem

A `Weather` table records `id`, `recordDate`, and `temperature` — one row per day. Find the IDs of days where the temperature was **higher than the previous calendar day**.

### 💻 SQL Solution

```sql
SELECT w2.id
FROM Weather w1
JOIN Weather w2
  ON DATEDIFF(w2.recordDate, w1.recordDate) = 1
WHERE w2.temperature > w1.temperature;
```

### 🔍 Explanation

- `SELECT w2.id`: We want the ID of the "later" day (the one with the rising temperature).
- `FROM Weather w1 JOIN Weather w2`: This is a **self-join** — the same table is joined to itself, using two aliases (`w1` for "yesterday," `w2` for "today") to compare rows against each other.
- `ON DATEDIFF(w2.recordDate, w1.recordDate) = 1`: `DATEDIFF()` returns the number of days between two dates. This condition pairs each day with the day exactly one day before it.
- `WHERE w2.temperature > w1.temperature`: Keeps only pairs where today's temperature is strictly higher than yesterday's.

### ✅ Why This Solution Works

Comparing consecutive days requires looking at two rows from the same table simultaneously — something a single-row query cannot do. A self-join solves this by treating the table as two separate "copies" that can be compared row-to-row, and `DATEDIFF` reliably identifies true calendar-day adjacency, even if some dates are missing from the table.

### 🧠 SQL Concepts Used

- ✔ Self JOIN
- ✔ Date Functions (DATEDIFF)
- ✔ WHERE
- ✔ Table Aliasing

### 💡 Interview Tip

- This question tests whether you know self-joins and understand that `id - 1` is **not** a safe substitute for "yesterday" if dates could have gaps.
- **Common mistake:** joining on `w1.id = w2.id - 1` instead of comparing dates — this assumes IDs are sequential and gap-free, which is a fragile assumption.
- **Edge case:** the very first day in the table has no "yesterday" to compare against, and the self-join naturally excludes it since no matching pair exists.

### ⏱ Time Complexity

Without an index: **O(n²)** in the worst case, since every row is compared against every other row.
With an index on `recordDate`: closer to **O(n log n)**, since MySQL can efficiently find the "day before" for each row.

### 💾 Space Complexity

**O(1)** to **O(n)** depending on whether MySQL materializes the join, but no significant extra structures are needed for the logic itself.

### 🔄 Alternative Solution

```sql
-- Using a window function (LAG) - available in MySQL 8.0+
SELECT id
FROM (
  SELECT
    id,
    temperature,
    LAG(temperature) OVER (ORDER BY recordDate) AS prev_temp,
    DATEDIFF(recordDate, LAG(recordDate) OVER (ORDER BY recordDate)) AS day_gap
  FROM Weather
) t
WHERE day_gap = 1 AND temperature > prev_temp;
```

`LAG()` looks at the previous row's value without a self-join — often more readable and can be more efficient on large datasets since it avoids a join entirely.

### 🎯 Key Takeaways

- Self-joins let you compare rows within the same table.
- Never assume `id` values represent chronological order — always compare actual date/time columns.
- `DATEDIFF()` is the safe way to check for exact day adjacency.

---

## 10. Average Time of Process per Machine

**Difficulty:** 🟡 Medium
**Category:** Self JOIN / Aggregation

---

### 📋 Problem

An `Activity` table logs `machine_id`, `process_id`, `activity_type` (`'start'` or `'end'`), and `timestamp`. Each process on a machine has exactly one start row and one end row. Find the average processing time (`end - start`) for each machine, rounded to 3 decimal places.

### 💻 SQL Solution

```sql
SELECT
  a1.machine_id,
  ROUND(AVG(a2.timestamp - a1.timestamp), 3) AS processing_time
FROM Activity a1
JOIN Activity a2
  ON a1.machine_id = a2.machine_id
 AND a1.process_id = a2.process_id
 AND a1.activity_type = 'start'
 AND a2.activity_type = 'end'
GROUP BY a1.machine_id;
```

### 🔍 Explanation

- `FROM Activity a1 JOIN Activity a2`: A self-join pairs the "start" row and "end" row of the same process together.
- `ON a1.machine_id = a2.machine_id AND a1.process_id = a2.process_id`: Ensures we're matching the start and end of the **same process on the same machine**.
- `AND a1.activity_type = 'start' AND a2.activity_type = 'end'`: Locks `a1` to always represent the start event and `a2` the end event, so the subtraction direction is always correct.
- `AVG(a2.timestamp - a1.timestamp)`: Computes the duration of each process (`end - start`), then averages those durations.
- `ROUND(..., 3)`: Rounds the final average to 3 decimal places, as required by the problem.
- `GROUP BY a1.machine_id`: Produces one average per machine, across all of its processes.

### ✅ Why This Solution Works

Each process's duration only makes sense once its start and end timestamps are on the **same row** so they can be subtracted. The self-join achieves that by matching start/end pairs using `machine_id` and `process_id` as the shared keys, and then `AVG()` naturally summarizes across all processes belonging to a machine.

### 🧠 SQL Concepts Used

- ✔ Self JOIN
- ✔ Multi-condition JOIN
- ✔ AVG()
- ✔ ROUND()
- ✔ GROUP BY

### 💡 Interview Tip

- This tests whether you can restructure "paired events" (start/end, login/logout) into a single row before aggregating — a very common real-world pattern.
- **Common mistake:** joining only on `machine_id` without also matching `process_id`, which would incorrectly pair unrelated processes together.
- **Edge case:** always double-check subtraction direction (`end - start`, not `start - end`) — locking `a1`/`a2` to specific `activity_type` values (as done here) prevents this bug entirely.

### ⏱ Time Complexity

Without an index: **O(n²)** for the self-join.
With a composite index on `(machine_id, process_id, activity_type)`: closer to **O(n log n)**, since matching pairs can be found efficiently.

### 💾 Space Complexity

**O(m)**, where `m` is the number of distinct machines, for the grouped averages.

### 🔄 Alternative Solution

```sql
-- Using conditional aggregation instead of a self-join
SELECT
  machine_id,
  ROUND(AVG(end_time - start_time), 3) AS processing_time
FROM (
  SELECT
    machine_id,
    process_id,
    MAX(CASE WHEN activity_type = 'end' THEN timestamp END) AS end_time,
    MAX(CASE WHEN activity_type = 'start' THEN timestamp END) AS start_time
  FROM Activity
  GROUP BY machine_id, process_id
) t
GROUP BY machine_id;
```

This avoids a self-join entirely by pivoting start/end onto the same row using conditional aggregation — often faster on large tables since it only scans `Activity` once.

### 🎯 Key Takeaways

- Self-joins are useful for pairing related rows (start/end, before/after).
- Conditional aggregation (`CASE` inside `MAX`/`SUM`) can replace some self-joins for a single-pass alternative.
- Always match on **all** relevant keys, not just one, to avoid incorrect pairings.

---

## 11. Employee Bonus

**Difficulty:** 🟢 Easy
**Category:** LEFT JOIN / NULL Handling

---

### 📋 Problem

An `Employee` table has `empId`, `name`, `supervisor`, and `salary`. A `Bonus` table has `empId` and `bonus`, but not every employee has a bonus entry. Return the name and bonus of employees whose bonus is **less than 1000**, or who have **no bonus at all**.

### 💻 SQL Solution

```sql
SELECT e.name, b.bonus
FROM Employee e
LEFT JOIN Bonus b
  ON e.empId = b.empId
WHERE b.bonus < 1000
   OR b.bonus IS NULL;
```

### 🔍 Explanation

- `SELECT e.name, b.bonus`: Returns name and bonus (which may be `NULL`).
- `FROM Employee e LEFT JOIN Bonus b ON e.empId = b.empId`: Keeps every employee, attaching their bonus if it exists, or `NULL` if it doesn't.
- `WHERE b.bonus < 1000`: Keeps employees whose recorded bonus is under 1000.
- `OR b.bonus IS NULL`: Also keeps employees who never received a bonus row at all — without this, they'd be excluded because `NULL < 1000` evaluates to `UNKNOWN`, not `TRUE`.

### ✅ Why This Solution Works

`LEFT JOIN` ensures no employee is dropped just because they lack a bonus record. The `WHERE` clause then explicitly accounts for both possible "low bonus" cases: a small numeric bonus, or a missing one entirely — combining both with `OR`.

### 🧠 SQL Concepts Used

- ✔ LEFT JOIN
- ✔ WHERE
- ✔ IS NULL
- ✔ Logical OR

### 💡 Interview Tip

- Another classic **NULL-trap** question, similar to "Find Customer Referee" — interviewers love pairing `LEFT JOIN` with `NULL` filtering to test both concepts at once.
- **Common mistake:** using `INNER JOIN`, which removes employees without a bonus row entirely, even though they clearly qualify (a missing bonus is effectively "less than 1000").
- **Edge case:** a bonus value of exactly 1000 should **not** appear in the output — the condition is strictly `<`.

### ⏱ Time Complexity

Without an index: **O(n × m)** for the join.
With an index on `Bonus.empId`: **O(n log m)**.

### 💾 Space Complexity

**O(1)** — straightforward filtering, no aggregation buffers.

### 🔄 Alternative Solution

```sql
-- Using COALESCE to treat missing bonuses as 0
SELECT e.name, b.bonus
FROM Employee e
LEFT JOIN Bonus b
  ON e.empId = b.empId
WHERE COALESCE(b.bonus, 0) < 1000;
```

`COALESCE(b.bonus, 0)` substitutes `0` whenever the bonus is `NULL`, letting a single comparison handle both cases without an explicit `OR`.

### 🎯 Key Takeaways

- `LEFT JOIN` + `NULL`-aware `WHERE` clauses are essential for "missing data" questions.
- `COALESCE`/`IFNULL` can simplify conditions that otherwise need an explicit `IS NULL` check.
- Always consider whether "less than X" should include "no value at all" based on the question's intent.

---

## 12. Students and Examinations

**Difficulty:** 🟢 Easy
**Category:** CROSS JOIN / LEFT JOIN

---

### 📋 Problem

A `Students` table has `student_id` and `student_name`. A `Subjects` table has `subject_name`. An `Examinations` table logs every exam a student actually attended (`student_id`, `subject_name`), with possible repeats. For **every student and every subject**, return how many times that student attended an exam in that subject — including combinations where the count is zero.

### 💻 SQL Solution

```sql
SELECT
  s.student_id,
  s.student_name,
  sub.subject_name,
  COUNT(e.subject_name) AS attended_exams
FROM Students s
CROSS JOIN Subjects sub
LEFT JOIN Examinations e
  ON s.student_id = e.student_id
 AND sub.subject_name = e.subject_name
GROUP BY s.student_id, s.student_name, sub.subject_name
ORDER BY s.student_id, sub.subject_name;
```

### 🔍 Explanation

- `FROM Students s CROSS JOIN Subjects sub`: A `CROSS JOIN` produces every possible pairing of a student with a subject — this guarantees all student/subject combinations exist, even ones with zero exam attendance.
- `LEFT JOIN Examinations e ON s.student_id = e.student_id AND sub.subject_name = e.subject_name`: Attaches actual exam attendance records to each student/subject pair, or `NULL` if that student never attended that subject's exam.
- `COUNT(e.subject_name)`: Counts non-`NULL` matches per group — students who never attended get a count of `0` because `COUNT()` ignores `NULL`s.
- `GROUP BY s.student_id, s.student_name, sub.subject_name`: Groups by each unique student/subject combination so `COUNT()` tallies attendance correctly.
- `ORDER BY s.student_id, sub.subject_name`: Sorts the final output for consistent, readable results.

### ✅ Why This Solution Works

The requirement to show **every** combination — even those with zero attendance — cannot be satisfied by only joining on actual exam records, since that would exclude missing combinations entirely. `CROSS JOIN` first builds the complete "universe" of student/subject pairs, and `LEFT JOIN` then safely layers in real attendance data without removing any pairs, since unmatched rows just become `NULL`, which `COUNT()` correctly reports as zero.

### 🧠 SQL Concepts Used

- ✔ CROSS JOIN
- ✔ LEFT JOIN
- ✔ COUNT()
- ✔ GROUP BY
- ✔ ORDER BY

### 💡 Interview Tip

- This is a favorite for testing whether you can construct a "complete grid" of combinations before filling in actual data — very common in reporting/dashboard-style questions.
- **Common mistake:** joining `Students` directly to `Examinations` without first cross-joining `Subjects`, which would silently omit subject/student pairs with zero attendance.
- **Edge case:** always count a column from the "attendance" table (like `e.subject_name`), never `*` — `COUNT(*)` would count `1` even for unmatched (`NULL`) rows, breaking the zero-count logic.

### ⏱ Time Complexity

**O(s × sub)** just to build the cross join (`s` students, `sub` subjects), plus the cost of matching against `Examinations`. With appropriate indexes on `Examinations(student_id, subject_name)`, the join stays efficient even as exam records grow.

### 💾 Space Complexity

**O(s × sub)** — proportional to the total number of student/subject combinations generated by the cross join.

### 🔄 Alternative Solution

```sql
-- Using conditional aggregation with a pre-built combination CTE (MySQL 8.0+)
WITH AllCombinations AS (
  SELECT s.student_id, s.student_name, sub.subject_name
  FROM Students s
  CROSS JOIN Subjects sub
)
SELECT
  ac.student_id,
  ac.student_name,
  ac.subject_name,
  COUNT(e.subject_name) AS attended_exams
FROM AllCombinations ac
LEFT JOIN Examinations e
  ON ac.student_id = e.student_id
 AND ac.subject_name = e.subject_name
GROUP BY ac.student_id, ac.student_name, ac.subject_name
ORDER BY ac.student_id, ac.subject_name;
```

Splitting the cross join into a CTE can make complex queries more readable, especially when the "complete grid" logic is reused elsewhere in a larger query.

### 🎯 Key Takeaways

- `CROSS JOIN` builds every possible combination between two tables.
- `COUNT(column)` ignores `NULL`s, making it the correct choice for "count actual occurrences" after a `LEFT JOIN`.
- CTEs (`WITH`) can make multi-step logic easier to read and reuse.

---

## 13. Managers with at Least 5 Direct Reports

**Difficulty:** 🟡 Medium
**Category:** GROUP BY / HAVING

---

### 📋 Problem

An `Employee` table has `id`, `name`, `department`, and `managerId`. Find the names of managers who have **5 or more** employees directly reporting to them.

### 💻 SQL Solution

```sql
SELECT name
FROM Employee
WHERE id IN (
  SELECT managerId
  FROM Employee
  GROUP BY managerId
  HAVING COUNT(*) >= 5
);
```

### 🔍 Explanation

- Inner query `SELECT managerId FROM Employee GROUP BY managerId HAVING COUNT(*) >= 5`: Groups all employees by their `managerId`, counts how many employees fall into each group, and keeps only manager IDs with **5 or more** direct reports.
- `HAVING COUNT(*) >= 5`: `HAVING` filters **after** grouping/aggregation — unlike `WHERE`, which filters individual rows before grouping, `HAVING` can reference the aggregate result (`COUNT(*)`) directly.
- Outer query `SELECT name FROM Employee WHERE id IN (...)`: Takes the list of qualifying manager IDs and looks up their names from the same table.

### ✅ Why This Solution Works

Counting direct reports per manager requires aggregation, and filtering on that count requires `HAVING` rather than `WHERE` (since the count doesn't exist until after grouping). The subquery isolates manager IDs meeting the threshold, and the outer query simply translates those IDs back into names.

### 🧠 SQL Concepts Used

- ✔ GROUP BY
- ✔ HAVING
- ✔ COUNT()
- ✔ Subquery
- ✔ IN

### 💡 Interview Tip

- This tests the classic distinction between `WHERE` (row-level filtering) and `HAVING` (group-level filtering) — one of the most frequently asked SQL concept questions.
- **Common mistake:** writing `WHERE COUNT(*) >= 5` directly, which throws an error because `WHERE` runs before aggregation exists.
- **Edge case:** employees with a `NULL` `managerId` (no manager) would be grouped together under `NULL` — since `NULL` never matches `= 5` conditions in most contexts, this typically doesn't cause issues here, but it's worth mentioning in an interview.

### ⏱ Time Complexity

Without an index: **O(n log n)** for the `GROUP BY` (typically implemented via a sort or hash aggregation).
With an index on `managerId`: grouping becomes closer to **O(n)**, since matching rows are already physically or logically adjacent.

### 💾 Space Complexity

**O(m)**, where `m` is the number of distinct managers, to hold group counts.

### 🔄 Alternative Solution

```sql
-- Using a self-join instead of a subquery
SELECT DISTINCT m.name
FROM Employee e
JOIN Employee m
  ON e.managerId = m.id
GROUP BY m.id, m.name
HAVING COUNT(*) >= 5;
```

This self-join version reads slightly more naturally ("employees joined to their managers") and avoids a separate subquery, though it performs similarly to the `IN` version for most datasets.

### 🎯 Key Takeaways

- `WHERE` filters rows before grouping; `HAVING` filters groups after aggregation.
- Subqueries in the `IN` clause are a common way to filter based on a computed condition from another query.
- Self-joins can sometimes replace subqueries for the same logical result.

---

## 14. Confirmation Rate

**Difficulty:** 🟡 Medium
**Category:** LEFT JOIN / CASE / AVG

---

### 📋 Problem

A `Signups` table logs when each user signed up (`user_id`, `time_stamp`). A `Confirmations` table logs every confirmation attempt (`user_id`, `time_stamp`, `action`, where `action` is `'confirmed'` or `'timeout'`). For each user, calculate their **confirmation rate**: the fraction of their confirmation attempts that were `'confirmed'`, rounded to 2 decimal places. Users with no attempts have a rate of 0.

### 💻 SQL Solution

```sql
SELECT
  s.user_id,
  ROUND(AVG(CASE WHEN c.action = 'confirmed' THEN 1 ELSE 0 END), 2) AS confirmation_rate
FROM Signups s
LEFT JOIN Confirmations c
  ON s.user_id = c.user_id
GROUP BY s.user_id;
```

### 🔍 Explanation

- `FROM Signups s LEFT JOIN Confirmations c ON s.user_id = c.user_id`: Ensures every signed-up user appears, even if they never made a confirmation attempt (in which case `c.action` is `NULL`).
- `CASE WHEN c.action = 'confirmed' THEN 1 ELSE 0 END`: Converts each row into a `1` (confirmed) or `0` (timeout or no attempt) — this turns a categorical value into a number that can be averaged.
- `AVG(...)`: Averaging a column of `1`s and `0`s produces exactly the fraction of `1`s — a common trick for computing rates/percentages in SQL.
- `ROUND(..., 2)`: Rounds to 2 decimal places as required.
- `GROUP BY s.user_id`: Produces one confirmation rate per user.

### ✅ Why This Solution Works

`AVG()` over a `CASE`-generated `0`/`1` column is mathematically identical to `(number of 1s) / (total rows)` — exactly the definition of a rate. Because we `LEFT JOIN` from `Signups`, users without confirmation rows still get a group (with a single `NULL` row from the join), and the `CASE` expression correctly converts that `NULL` action into `0`, giving a confirmation rate of `0` rather than excluding the user or erroring out.

### 🧠 SQL Concepts Used

- ✔ LEFT JOIN
- ✔ CASE
- ✔ AVG()
- ✔ ROUND()
- ✔ GROUP BY

### 💡 Interview Tip

- "Averaging a 0/1 CASE expression to compute a rate" is one of the most useful and frequently tested SQL patterns — memorize it.
- **Common mistake:** using `COUNT()` instead of `AVG()`, which gives a total instead of a proportion, or forgetting to handle users with zero confirmation attempts.
- **Edge case:** a user with no rows in `Confirmations` still needs to appear with rate `0`, not be excluded — this is why `LEFT JOIN` from `Signups` (not `Confirmations`) is essential.

### ⏱ Time Complexity

Without an index: **O(n × m)** for the join, plus **O(n log n)** for grouping.
With an index on `Confirmations.user_id`: closer to **O(n log m)**.

### 💾 Space Complexity

**O(u)**, where `u` is the number of distinct users, for the grouped rates.

### 🔄 Alternative Solution

```sql
-- Using SUM and COUNT separately instead of AVG on a CASE expression
SELECT
  s.user_id,
  ROUND(
    IFNULL(SUM(CASE WHEN c.action = 'confirmed' THEN 1 ELSE 0 END), 0)
    / COUNT(c.time_stamp == c.time_stamp OR TRUE), -- illustrative only
    2
  ) AS confirmation_rate
FROM Signups s
LEFT JOIN Confirmations c ON s.user_id = c.user_id
GROUP BY s.user_id;
```

In practice, most engineers prefer the cleaner `AVG(CASE ...)` form shown as the primary solution — `SUM`/`COUNT` division is more error-prone with `NULL`s and integer division, so it's mainly useful to understand conceptually, not to write by default.

### 🎯 Key Takeaways

- `AVG(CASE WHEN condition THEN 1 ELSE 0 END)` is the standard SQL pattern for computing a rate or percentage.
- `LEFT JOIN` is essential when you need every entity to appear, even with zero activity.
- Be careful about integer division when manually computing `SUM / COUNT` instead of using `AVG()`.

---

## 15. Not Boring Movies

**Difficulty:** 🟢 Easy
**Category:** WHERE / ORDER BY

---

### 📋 Problem

A `Cinema` table has `id`, `movie`, `description`, and `rating`. Return all movies with an **odd** `id` and a description that is **not** `'boring'`, sorted by rating in descending order.

### 💻 SQL Solution

```sql
SELECT *
FROM Cinema
WHERE id % 2 = 1
  AND description <> 'boring'
ORDER BY rating DESC;
```

### 🔍 Explanation

- `SELECT *`: Returns all columns for qualifying rows.
- `FROM Cinema`: Source table.
- `WHERE id % 2 = 1`: The `%` operator returns the remainder of division — an odd number always has a remainder of `1` when divided by `2`.
- `AND description <> 'boring'`: Excludes movies explicitly marked as boring.
- `ORDER BY rating DESC`: Sorts results from highest to lowest rating.

### ✅ Why This Solution Works

The modulo operator is the standard way to test odd/even in SQL, and combining it with a string inequality filters down to exactly the movies described. `ORDER BY ... DESC` then arranges the final result as requested, since sorting happens only after all filtering is complete.

### 🧠 SQL Concepts Used

- ✔ SELECT
- ✔ WHERE
- ✔ Modulo Operator (%)
- ✔ ORDER BY DESC

### 💡 Interview Tip

- Simple, but tests whether you know `%` for odd/even checks and remember `ORDER BY` direction keywords.
- **Common mistake:** forgetting `DESC` (default sort order is ascending) or using `!=` inconsistently with `<>` (both work identically in MySQL, but consistency matters for readability).
- **Edge case:** `id = 0` is even, not odd — make sure the modulo logic is tested against real data, not just assumed.

### ⏱ Time Complexity

Without an index: **O(n log n)** due to the `ORDER BY` sort.
With an index on `rating`: MySQL can potentially avoid a separate sort step, though the `id % 2` filter still requires scanning all rows since expressions on a column generally prevent index usage unless a functional/generated index exists.

### 💾 Space Complexity

**O(n)** in the worst case for the sort buffer, though MySQL may use disk-based sorting for very large result sets.

### 🔄 Alternative Solution

```sql
-- Using MOD() function instead of the % operator
SELECT *
FROM Cinema
WHERE MOD(id, 2) = 1
  AND description <> 'boring'
ORDER BY rating DESC;
```

`MOD()` and `%` are functionally identical in MySQL — this alternative is purely a style/readability choice.

### 🎯 Key Takeaways

- `%` (or `MOD()`) is the standard tool for odd/even and other remainder-based checks.
- `ORDER BY` always runs after filtering, on the final result set.
- Expression-based filters (like `id % 2`) generally can't use a plain index on that column.

---

## 16. Average Selling Price

**Difficulty:** 🟢 Easy
**Category:** LEFT JOIN / Aggregation

---

### 📋 Problem

A `Prices` table stores `product_id`, `start_date`, `end_date`, and `price` (a product can have different prices in different date ranges). A `UnitsSold` table logs `product_id`, `purchase_date`, and `units`. Compute the **average selling price** for each product: total revenue divided by total units sold, rounded to 2 decimal places. Products with no sales should show `0`.

### 💻 SQL Solution

```sql
SELECT
  p.product_id,
  IFNULL(ROUND(SUM(p.price * u.units) / SUM(u.units), 2), 0) AS average_price
FROM Prices p
LEFT JOIN UnitsSold u
  ON p.product_id = u.product_id
 AND u.purchase_date BETWEEN p.start_date AND p.end_date
GROUP BY p.product_id;
```

### 🔍 Explanation

- `LEFT JOIN UnitsSold u ON p.product_id = u.product_id AND u.purchase_date BETWEEN p.start_date AND p.end_date`: Matches each sale to the price range that was active on its purchase date. `BETWEEN` is inclusive on both ends.
- `SUM(p.price * u.units)`: For each matching row, multiplies price by units sold to get revenue for that sale, then sums across all sales for the product — this is total revenue.
- `SUM(u.units)`: Total number of units sold for the product.
- `SUM(revenue) / SUM(units)`: Revenue-weighted average price — mathematically the correct way to average a price across varying purchase quantities.
- `IFNULL(..., 0)`: If a product had no matching sales at all, both sums would be `NULL` (since `LEFT JOIN` produces no rows to sum), so `IFNULL` substitutes `0` as the required fallback.
- `GROUP BY p.product_id`: One row of output per product.

### ✅ Why This Solution Works

A simple average of individual prices would be wrong here, because it would treat a sale of 1 unit the same as a sale of 100 units. Dividing total revenue by total units instead gives a properly weighted average, and the `LEFT JOIN` combined with `BETWEEN` correctly attributes each sale to the price that was in effect on its purchase date.

### 🧠 SQL Concepts Used

- ✔ LEFT JOIN
- ✔ BETWEEN
- ✔ SUM()
- ✔ IFNULL()
- ✔ ROUND()
- ✔ GROUP BY

### 💡 Interview Tip

- This tests whether you understand **weighted averages** — a very common real-world requirement (revenue per unit, average order value, etc.).
- **Common mistake:** using `AVG(p.price)` directly, which ignores quantity and gives a mathematically incorrect average.
- **Edge case:** products with zero sales need explicit `IFNULL` handling, since dividing `NULL / NULL` (from an unmatched `LEFT JOIN`) returns `NULL`, not `0`.

### ⏱ Time Complexity

Without an index: **O(n × m)** for the range join.
With an index on `UnitsSold(product_id, purchase_date)`: significantly faster range lookups, closer to **O(n log m)**.

### 💾 Space Complexity

**O(p)**, where `p` is the number of distinct products, for the grouped results.

### 🔄 Alternative Solution

```sql
-- Using a subquery for revenue per sale before aggregating
SELECT
  product_id,
  IFNULL(ROUND(SUM(revenue) / SUM(units), 2), 0) AS average_price
FROM (
  SELECT p.product_id, u.units, p.price * u.units AS revenue
  FROM Prices p
  LEFT JOIN UnitsSold u
    ON p.product_id = u.product_id
   AND u.purchase_date BETWEEN p.start_date AND p.end_date
) t
GROUP BY product_id;
```

Splitting the revenue calculation into a subquery can make debugging easier, since you can inspect per-sale revenue independently before aggregating.

### 🎯 Key Takeaways

- Weighted averages require `SUM(value × weight) / SUM(weight)`, not `AVG(value)`.
- `BETWEEN` is inclusive on both boundaries — verify this matches the intended date logic.
- `IFNULL`/`COALESCE` are essential whenever a `LEFT JOIN` could leave aggregates as `NULL`.

---

## 17. Project Employees I

**Difficulty:** 🟢 Easy
**Category:** JOIN / AVG

---

### 📋 Problem

A `Project` table maps `project_id` to `employee_id`. An `Employee` table has `employee_id`, `name`, and `experience_years`. For each project, return the **average experience years** of its employees, rounded to 2 decimal places.

### 💻 SQL Solution

```sql
SELECT
  p.project_id,
  ROUND(AVG(e.experience_years), 2) AS average_years
FROM Project p
JOIN Employee e
  ON p.employee_id = e.employee_id
GROUP BY p.project_id;
```

### 🔍 Explanation

- `FROM Project p JOIN Employee e ON p.employee_id = e.employee_id`: Links each project assignment to that employee's experience data.
- `AVG(e.experience_years)`: Averages the experience of all employees on a given project.
- `ROUND(..., 2)`: Formats the result to 2 decimal places.
- `GROUP BY p.project_id`: Produces one average per project.

### ✅ Why This Solution Works

Since every project row references a real employee, an `INNER JOIN` safely connects assignment data to experience data without losing any rows. Grouping by project and averaging the joined experience values directly answers "what is the average experience per project."

### 🧠 SQL Concepts Used

- ✔ INNER JOIN
- ✔ AVG()
- ✔ ROUND()
- ✔ GROUP BY

### 💡 Interview Tip

- A good warm-up question for practicing the "join then aggregate" pattern that appears throughout SQL interviews.
- **Common mistake:** grouping by `p.employee_id` instead of `p.project_id`, which answers a completely different question.
- **Edge case:** if an employee is assigned to a project multiple times (duplicate rows in `Project`), their experience would be counted multiple times in the average — worth clarifying with an interviewer whether `Project` guarantees uniqueness.

### ⏱ Time Complexity

Without an index: **O(n × m)** for the join.
With an index on `Employee.employee_id` (typically the primary key): **O(n log m)**.

### 💾 Space Complexity

**O(p)**, where `p` is the number of distinct projects.

### 🔄 Alternative Solution

```sql
-- Using a correlated subquery instead of GROUP BY
SELECT
  DISTINCT p.project_id,
  ROUND((
    SELECT AVG(e.experience_years)
    FROM Project p2
    JOIN Employee e ON p2.employee_id = e.employee_id
    WHERE p2.project_id = p.project_id
  ), 2) AS average_years
FROM Project p;
```

Correlated subqueries can express the same logic but re-run per project row — the `JOIN` + `GROUP BY` version is almost always preferable for performance and readability.

### 🎯 Key Takeaways

- The "join, then group and aggregate" pattern is one of the most common SQL building blocks.
- Always double-check which column you're grouping by matches the question's intended granularity.
- Correlated subqueries are usually a less efficient substitute for `GROUP BY`.

---

## 18. Percentage of Users Attended a Contest

**Difficulty:** 🟡 Medium
**Category:** Subquery / Aggregation

---

### 📋 Problem

A `Users` table lists all users (`user_id`, `user_name`). A `Register` table logs which users registered for which contests (`contest_id`, `user_id`). For each contest, compute the percentage of **all users** who registered, rounded to 2 decimal places, sorted by percentage descending (and by `contest_id` ascending for ties).

### 💻 SQL Solution

```sql
SELECT
  contest_id,
  ROUND(COUNT(user_id) / (SELECT COUNT(*) FROM Users) * 100, 2) AS percentage
FROM Register
GROUP BY contest_id
ORDER BY percentage DESC, contest_id ASC;
```

### 🔍 Explanation

- `(SELECT COUNT(*) FROM Users)`: A **scalar subquery** that computes the total number of users in the system once. Since it doesn't depend on any outer row, MySQL only needs to compute it a single time.
- `COUNT(user_id)`: Counts how many users registered for each contest, per group.
- `COUNT(user_id) / (SELECT COUNT(*) FROM Users) * 100`: Converts the registration count into a percentage of all users.
- `ROUND(..., 2)`: Formats to 2 decimal places.
- `GROUP BY contest_id`: One row of output per contest.
- `ORDER BY percentage DESC, contest_id ASC`: Sorts by highest percentage first; ties are broken by ascending contest ID.

### ✅ Why This Solution Works

A percentage always needs a numerator (registrations for this contest) and a fixed denominator (total users overall) — the scalar subquery supplies that constant denominator independently of the `GROUP BY`, while `COUNT(user_id)` supplies the per-contest numerator. Combining them inside the same `SELECT` produces the correct ratio for every group.

### 🧠 SQL Concepts Used

- ✔ Scalar Subquery
- ✔ COUNT()
- ✔ GROUP BY
- ✔ ROUND()
- ✔ ORDER BY (multiple columns)

### 💡 Interview Tip

- This tests whether you know how to compute a ratio against a **global** total while still grouping by a different dimension — a very common reporting pattern ("% of total").
- **Common mistake:** trying to compute the total inside the same `GROUP BY` query without a subquery, which is not possible since `GROUP BY` only gives you per-group totals, not a grand total, in the same pass.
- **Edge case:** integer division — always ensure `COUNT(user_id) / (SELECT COUNT(*) FROM Users)` is treated as a float; MySQL automatically promotes this to decimal division since both operands are already effectively numeric, but it's worth verifying with `CAST` if working in stricter SQL dialects.

### ⏱ Time Complexity

**O(n log n)** for grouping, plus **O(1)** for the constant scalar subquery (computed once, not per row).

### 💾 Space Complexity

**O(c)**, where `c` is the number of distinct contests.

### 🔄 Alternative Solution

```sql
-- Using a CROSS JOIN to pre-compute the total once, then reference it directly
SELECT
  r.contest_id,
  ROUND(COUNT(r.user_id) / u.total_users * 100, 2) AS percentage
FROM Register r
CROSS JOIN (SELECT COUNT(*) AS total_users FROM Users) u
GROUP BY r.contest_id, u.total_users
ORDER BY percentage DESC, r.contest_id ASC;
```

This restructures the scalar subquery as a one-row `CROSS JOIN`, which some query planners optimize slightly differently — functionally equivalent to the primary solution.

### 🎯 Key Takeaways

- Scalar subqueries are ideal for injecting a single constant value (like a grand total) into a grouped query.
- "Percentage of total" problems always need a fixed denominator computed independently of the grouping.
- `ORDER BY` can sort by multiple columns to break ties predictably.

---

## 19. Queries Quality and Percentage

**Difficulty:** 🟢 Easy
**Category:** GROUP BY / CASE

---

### 📋 Problem

A `Queries` table logs `query_name`, `result`, `position`, and `rating` for search queries. For each `query_name`, compute:
1. **Quality** — the average of `rating / position`, rounded to 2 decimal places.
2. **Poor query percentage** — the percentage of queries with `rating < 3`, rounded to 2 decimal places.

### 💻 SQL Solution

```sql
SELECT
  query_name,
  ROUND(AVG(rating / position), 2) AS quality,
  ROUND(
    SUM(CASE WHEN rating < 3 THEN 1 ELSE 0 END) / COUNT(*) * 100,
    2
  ) AS poor_query_percentage
FROM Queries
GROUP BY query_name;
```

### 🔍 Explanation

- `AVG(rating / position)`: For each row, divides rating by position to get a per-query "quality score," then averages those scores across all rows sharing the same `query_name`.
- `SUM(CASE WHEN rating < 3 THEN 1 ELSE 0 END)`: Counts how many rows have a poor rating (below 3) by converting each row into `1` (poor) or `0` (not poor) and summing.
- `/ COUNT(*) * 100`: Divides the poor count by the total row count for that group, then converts to a percentage.
- `GROUP BY query_name`: Produces one row of metrics per unique query name.

### ✅ Why This Solution Works

Both metrics are per-group averages/ratios computed from row-level expressions. `AVG()` naturally handles the "average of a ratio" for quality, while `SUM(CASE ...) / COUNT(*)` computes the proportion of poor-rated rows — the same `AVG(CASE...) * 100` trick from earlier questions, just written with explicit `SUM`/`COUNT` for clarity.

### 🧠 SQL Concepts Used

- ✔ GROUP BY
- ✔ AVG()
- ✔ CASE
- ✔ SUM()
- ✔ COUNT()
- ✔ ROUND()

### 💡 Interview Tip

- This combines two common patterns (weighted-style averaging and conditional percentage calculation) into a single query — great practice for multi-metric reporting questions.
- **Common mistake:** computing `AVG(rating) / AVG(position)` instead of `AVG(rating / position)` — these are mathematically different! The question requires averaging the per-row ratio, not the ratio of two separate averages.
- **Edge case:** `position` should never be `0` in valid data, but it's worth mentioning that a `0` position would cause a division-by-zero error — a good point to raise in an interview about data validation assumptions.

### ⏱ Time Complexity

**O(n log n)** for grouping (or **O(n)** with an index on `query_name`), plus **O(n)** to compute per-row expressions.

### 💾 Space Complexity

**O(q)**, where `q` is the number of distinct query names.

### 🔄 Alternative Solution

```sql
-- Using AVG(CASE...) directly instead of SUM/COUNT for the percentage
SELECT
  query_name,
  ROUND(AVG(rating / position), 2) AS quality,
  ROUND(AVG(CASE WHEN rating < 3 THEN 1 ELSE 0 END) * 100, 2) AS poor_query_percentage
FROM Queries
GROUP BY query_name;
```

This is functionally identical to `SUM(...)/COUNT(*)` but slightly more concise — both are valid and commonly seen in real codebases.

### 🎯 Key Takeaways

- `AVG(a / b)` (average of a ratio) is different from `AVG(a) / AVG(b)` (ratio of averages) — know the difference.
- `SUM(CASE...) / COUNT(*)` and `AVG(CASE...)` both compute proportions correctly.
- Combining multiple aggregate metrics in one query is a very common real-world reporting requirement.

---

## 20. Monthly Transactions I

**Difficulty:** 🟡 Medium
**Category:** GROUP BY / Date Functions / CASE

---

### 📋 Problem

A `Transactions` table logs `id`, `country`, `state` (`'approved'` or `'declined'`), `amount`, and `trans_date`. For each month and country, find: the total number of transactions, how many were approved, the total transaction amount, and the total approved amount.

### 💻 SQL Solution

```sql
SELECT
  DATE_FORMAT(trans_date, '%Y-%m') AS month,
  country,
  COUNT(*) AS trans_count,
  SUM(CASE WHEN state = 'approved' THEN 1 ELSE 0 END) AS approved_count,
  SUM(amount) AS trans_total_amount,
  SUM(CASE WHEN state = 'approved' THEN amount ELSE 0 END) AS approved_total_amount
FROM Transactions
GROUP BY month, country;
```

### 🔍 Explanation

- `DATE_FORMAT(trans_date, '%Y-%m') AS month`: Extracts the year and month from the transaction date as a string like `'2018-12'`, effectively bucketing every transaction into its calendar month regardless of the exact day.
- `COUNT(*)`: Total number of transactions in each month/country group.
- `SUM(CASE WHEN state = 'approved' THEN 1 ELSE 0 END)`: Counts only approved transactions using the conditional-sum pattern.
- `SUM(amount)`: Total dollar amount across all transactions in the group.
- `SUM(CASE WHEN state = 'approved' THEN amount ELSE 0 END)`: Total dollar amount, but only from approved transactions.
- `GROUP BY month, country`: Groups rows by both the derived month string and the country, so each combination gets its own row of metrics.

### ✅ Why This Solution Works

Since the question asks for numbers broken down by **both** month and country, grouping by both `DATE_FORMAT(trans_date, '%Y-%m')` and `country` creates exactly the right buckets. Each requested metric is then computed with the appropriate aggregate: simple counts/sums for totals, and `CASE`-wrapped versions for the "approved only" metrics.

### 🧠 SQL Concepts Used

- ✔ Date Functions (DATE_FORMAT)
- ✔ GROUP BY (multiple columns)
- ✔ CASE
- ✔ COUNT() / SUM()

### 💡 Interview Tip

- This is a great test of combining **date bucketing** with **conditional aggregation** — a bread-and-butter pattern in analytics/reporting SQL.
- **Common mistake:** grouping by `trans_date` directly instead of the formatted month string, which would create a separate group for every single day instead of every month.
- **Edge case:** you can `GROUP BY` a computed alias like `month` in MySQL (unlike some strict SQL dialects that require repeating the full expression) — but it's good practice to know both forms work.

### ⏱ Time Complexity

**O(n log n)** for grouping across two dimensions, or **O(n)** with a composite index that supports the date range and country grouping.

### 💾 Space Complexity

**O(g)**, where `g` is the number of distinct month/country combinations.

### 🔄 Alternative Solution

```sql
-- Grouping by the raw expression instead of the alias (more portable across SQL dialects)
SELECT
  DATE_FORMAT(trans_date, '%Y-%m') AS month,
  country,
  COUNT(*) AS trans_count,
  SUM(CASE WHEN state = 'approved' THEN 1 ELSE 0 END) AS approved_count,
  SUM(amount) AS trans_total_amount,
  SUM(CASE WHEN state = 'approved' THEN amount ELSE 0 END) AS approved_total_amount
FROM Transactions
GROUP BY DATE_FORMAT(trans_date, '%Y-%m'), country;
```

Functionally identical to the primary solution — repeating the full expression in `GROUP BY` is required in some databases (like older PostgreSQL versions) even though MySQL allows the shorthand alias.

### 🎯 Key Takeaways

- `DATE_FORMAT()` is the standard way to bucket dates into coarser periods like months or years.
- Multiple `CASE`-wrapped aggregates can compute several conditional metrics in a single pass over the data.
- MySQL allows grouping by column aliases, but not all databases do — write portable SQL when in doubt.

---

## 21. Immediate Food Delivery II

**Difficulty:** 🟡 Medium
**Category:** Subquery / Aggregation

---

### 📋 Problem

A `Delivery` table logs `delivery_id`, `customer_id`, `order_date`, and `customer_pref_delivery_date`. An order is "immediate" if `order_date = customer_pref_delivery_date`. For each customer's **first ever order**, find the percentage of first orders that were immediate, rounded to 2 decimal places.

### 💻 SQL Solution

```sql
SELECT
  ROUND(
    SUM(CASE WHEN order_date = customer_pref_delivery_date THEN 1 ELSE 0 END)
    / COUNT(*) * 100,
    2
  ) AS immediate_percentage
FROM Delivery
WHERE (customer_id, order_date) IN (
  SELECT customer_id, MIN(order_date)
  FROM Delivery
  GROUP BY customer_id
);
```

### 🔍 Explanation

- Inner query `SELECT customer_id, MIN(order_date) FROM Delivery GROUP BY customer_id`: For each customer, finds the earliest `order_date` — this identifies each customer's very first order.
- `WHERE (customer_id, order_date) IN (...)`: A **row-value comparison** — this filters the outer query down to only the rows matching a customer's first order, using a pair of columns simultaneously rather than just one.
- `SUM(CASE WHEN order_date = customer_pref_delivery_date THEN 1 ELSE 0 END)`: Among those first orders, counts how many were "immediate" (ordered on the exact day the customer preferred).
- `/ COUNT(*) * 100`: Converts the immediate count into a percentage of all first orders.

### ✅ Why This Solution Works

The problem has two layers: first, identify *which* rows count as "first orders" (a per-customer minimum), then compute a percentage *only* over those rows. The subquery isolates the first-order rows using `MIN(order_date)` grouped by customer, and the row-value `IN` clause efficiently filters the outer query to match exactly those `(customer_id, order_date)` pairs — correctly handling customers whose first order date might coincide with other customers' dates without confusion.

### 🧠 SQL Concepts Used

- ✔ Subquery
- ✔ MIN()
- ✔ Row-value IN comparison
- ✔ CASE
- ✔ SUM() / COUNT()

### 💡 Interview Tip

- Tests whether you can chain "find the relevant rows first, then aggregate over just those rows" — a very common two-step interview pattern.
- **Common mistake:** filtering with `WHERE order_date = (SELECT MIN(order_date) ...)` using only `order_date` without pairing it with `customer_id`, which would compare against a single global minimum instead of each customer's own minimum.
- **Edge case:** if a customer has two orders tied for the earliest date, both would match the subquery's date — this is a legitimate business question to clarify with an interviewer (does "first order" assume uniqueness?).

### ⏱ Time Complexity

**O(n log n)** for the inner `GROUP BY`/`MIN` computation, plus **O(n)** to filter the outer query — with an index on `(customer_id, order_date)`, both steps become significantly faster.

### 💾 Space Complexity

**O(c)**, where `c` is the number of distinct customers, to hold the intermediate first-order dates.

### 🔄 Alternative Solution

```sql
-- Using a window function (MySQL 8.0+) instead of a subquery
WITH FirstOrders AS (
  SELECT
    *,
    ROW_NUMBER() OVER (PARTITION BY customer_id ORDER BY order_date) AS rn
  FROM Delivery
)
SELECT
  ROUND(
    SUM(CASE WHEN order_date = customer_pref_delivery_date THEN 1 ELSE 0 END)
    / COUNT(*) * 100,
    2
  ) AS immediate_percentage
FROM FirstOrders
WHERE rn = 1;
```

`ROW_NUMBER()` explicitly ranks each customer's orders by date, and filtering `rn = 1` isolates the true first order per customer — this handles duplicate dates more predictably (picks exactly one row) than the `MIN()` subquery approach.

### 🎯 Key Takeaways

- Row-value comparisons (`WHERE (col1, col2) IN (...)`) let you filter on combinations of columns at once.
- "First occurrence per group" problems can be solved with `MIN()` + subquery or `ROW_NUMBER()` + `PARTITION BY`.
- Always clarify tie-breaking rules when a business definition (like "first order") could be ambiguous.

---

## 22. Game Play Analysis IV

**Difficulty:** 🟡 Medium
**Category:** Subquery / Date Functions

---

### 📋 Problem

An `Activity` table logs `player_id`, `device_id`, `event_date`, and `games_played`. For each player, their "install date" is the date of their very first login. Find the **fraction** of players who logged in again on the day immediately following their install date, rounded to 2 decimal places.

### 💻 SQL Solution

```sql
SELECT
  ROUND(
    COUNT(DISTINCT a1.player_id) / (SELECT COUNT(DISTINCT player_id) FROM Activity),
    2
  ) AS fraction
FROM Activity a1
JOIN (
  SELECT player_id, MIN(event_date) AS first_date
  FROM Activity
  GROUP BY player_id
) a2
  ON a1.player_id = a2.player_id
 AND a1.event_date = DATE_ADD(a2.first_date, INTERVAL 1 DAY);
```

### 🔍 Explanation

- Subquery `a2`: `SELECT player_id, MIN(event_date) AS first_date FROM Activity GROUP BY player_id` computes each player's install date (their earliest login).
- `JOIN ... ON a1.player_id = a2.player_id AND a1.event_date = DATE_ADD(a2.first_date, INTERVAL 1 DAY)`: Matches players who have an activity row **exactly one day after** their install date. `DATE_ADD()` shifts a date forward by a specified interval.
- `COUNT(DISTINCT a1.player_id)`: Counts how many unique players satisfied that "returned the next day" condition.
- `(SELECT COUNT(DISTINCT player_id) FROM Activity)`: A scalar subquery computing the total number of unique players overall (the denominator).
- Dividing the two and rounding produces the required fraction.

### ✅ Why This Solution Works

This is a classic **retention** calculation: numerator = players active the day after their first login, denominator = all players. The inner subquery isolates each player's install date, the join finds who returned exactly one day later, and the outer scalar subquery supplies the fixed total-player denominator — mirroring the same "ratio against a global total" pattern seen in earlier percentage questions.

### 🧠 SQL Concepts Used

- ✔ Subquery
- ✔ MIN()
- ✔ Date Functions (DATE_ADD)
- ✔ JOIN
- ✔ COUNT(DISTINCT)

### 💡 Interview Tip

- This question is essentially "Day-1 retention" — an extremely common real-world product metric, so expect variations of it in data analyst interviews.
- **Common mistake:** using `event_date = first_date + 1` with raw date arithmetic that isn't portable, instead of `DATE_ADD()` — always use explicit date functions.
- **Edge case:** a player who only ever logged in once (no next-day activity) simply won't have a matching row in the join — correctly excluded without extra logic.

### ⏱ Time Complexity

**O(n log n)** for computing `MIN(event_date)` per player, plus **O(n)** for the join — with an index on `(player_id, event_date)`, this becomes significantly more efficient.

### 💾 Space Complexity

**O(p)**, where `p` is the number of distinct players, for the intermediate install-date table.

### 🔄 Alternative Solution

```sql
-- Using a window function to compute the first login date inline
WITH RankedActivity AS (
  SELECT
    player_id,
    event_date,
    MIN(event_date) OVER (PARTITION BY player_id) AS first_date
  FROM Activity
)
SELECT
  ROUND(
    COUNT(DISTINCT CASE WHEN event_date = DATE_ADD(first_date, INTERVAL 1 DAY) THEN player_id END)
    / (SELECT COUNT(DISTINCT player_id) FROM Activity),
    2
  ) AS fraction
FROM RankedActivity;
```

`MIN() OVER (PARTITION BY player_id)` computes each player's first login date without a separate `GROUP BY` subquery — a useful window-function alternative for MySQL 8.0+.

### 🎯 Key Takeaways

- Retention-style metrics almost always follow the pattern: numerator (returned users) ÷ denominator (all users).
- `DATE_ADD()`/`DATE_SUB()` are the safe, portable way to perform date arithmetic.
- Window functions can sometimes replace a `GROUP BY` subquery when you need a per-group value alongside the original rows.

---

## 23. Number of Unique Subjects Taught by Each Teacher

**Difficulty:** 🟢 Easy
**Category:** GROUP BY / COUNT DISTINCT

---

### 📋 Problem

A `Teacher` table logs `teacher_id`, `subject_id`, and `dept_id` — a teacher may teach the same subject in multiple departments. For each teacher, count how many **distinct** subjects they teach.

### 💻 SQL Solution

```sql
SELECT
  teacher_id,
  COUNT(DISTINCT subject_id) AS cnt
FROM Teacher
GROUP BY teacher_id;
```

### 🔍 Explanation

- `COUNT(DISTINCT subject_id)`: Counts unique `subject_id` values per group, rather than counting every row — this is what makes the count reflect *distinct subjects*, not total teaching assignments.
- `GROUP BY teacher_id`: Produces one row of output per teacher.

### ✅ Why This Solution Works

Since a teacher could teach the same subject across multiple departments (producing multiple rows with the same `subject_id`), a plain `COUNT(subject_id)` would overcount. `DISTINCT` inside `COUNT()` ensures each unique subject is only counted once per teacher, regardless of how many departments it appears in.

### 🧠 SQL Concepts Used

- ✔ GROUP BY
- ✔ COUNT(DISTINCT)

### 💡 Interview Tip

- A quick, focused test of `COUNT(DISTINCT ...)` — interviewers use this to see if you default to plain `COUNT()` without considering duplicates.
- **Common mistake:** using `COUNT(subject_id)` instead of `COUNT(DISTINCT subject_id)`, which silently overcounts whenever the same subject/teacher pair appears more than once.
- **Edge case:** a teacher who appears only once in the table still gets a correct count of `1` — `COUNT(DISTINCT ...)` behaves the same as `COUNT()` when there are no duplicates.

### ⏱ Time Complexity

**O(n log n)** — grouping and de-duplicating values typically requires a sort or hash-based approach internally.

### 💾 Space Complexity

**O(t × s)** in the worst case, where `t` is the number of teachers and `s` is the average number of distinct subjects tracked per teacher during aggregation.

### 🔄 Alternative Solution

```sql
-- Using a subquery to pre-deduplicate before counting
SELECT teacher_id, COUNT(*) AS cnt
FROM (SELECT DISTINCT teacher_id, subject_id FROM Teacher) t
GROUP BY teacher_id;
```

This explicitly removes duplicate `(teacher_id, subject_id)` pairs first, then counts rows per teacher — logically equivalent to `COUNT(DISTINCT subject_id)`, just spelled out in two steps.

### 🎯 Key Takeaways

- `COUNT(DISTINCT column)` counts unique values, not total rows.
- Always consider whether duplicate rows could exist before choosing between `COUNT()` and `COUNT(DISTINCT ...)`.
- The same de-duplication logic can be expressed either inline (`DISTINCT` inside `COUNT`) or via a separate subquery.

---

## 24. User Activity for the Past 30 Days I

**Difficulty:** 🟡 Medium
**Category:** WHERE / Date Range

---

### 📋 Problem

An `Activity` table logs `user_id`, `session_id`, `activity_date`, and `activity_type`. For each day in the **30-day window ending on 2019-07-27** (inclusive), find the number of unique users who were active that day.

### 💻 SQL Solution

```sql
SELECT
  activity_date AS day,
  COUNT(DISTINCT user_id) AS active_users
FROM Activity
WHERE activity_date BETWEEN DATE_SUB('2019-07-27', INTERVAL 29 DAY) AND '2019-07-27'
GROUP BY activity_date;
```

### 🔍 Explanation

- `DATE_SUB('2019-07-27', INTERVAL 29 DAY)`: Subtracts 29 days from the end date, producing a 30-day inclusive range (29 days back + the end date itself = 30 days total).
- `WHERE activity_date BETWEEN ... AND '2019-07-27'`: Filters activity rows down to just that 30-day window.
- `COUNT(DISTINCT user_id)`: Counts unique active users per day — a user with multiple sessions on the same day is only counted once.
- `GROUP BY activity_date`: Produces one row of output per calendar day within the window.

### ✅ Why This Solution Works

The window boundaries are computed explicitly using date arithmetic (`DATE_SUB` with a 29-day offset) so the range always covers exactly 30 calendar days ending on the target date, regardless of month/year boundaries. Filtering first with `WHERE`, then grouping and counting distinct users per day, produces the required daily active-user report.

### 🧠 SQL Concepts Used

- ✔ WHERE
- ✔ BETWEEN
- ✔ Date Functions (DATE_SUB)
- ✔ COUNT(DISTINCT)
- ✔ GROUP BY

### 💡 Interview Tip

- This tests careful **date range math** — a very common source of off-by-one errors ("30 days" often means 29 days back plus today, not 30 days back).
- **Common mistake:** using `INTERVAL 30 DAY` instead of `29 DAY`, which produces a 31-day window instead of 30.
- **Edge case:** days within the window with **zero** activity won't appear in the output at all, since there's no source row to group — if the question required showing zero-activity days explicitly, you'd need a generated calendar table joined with `LEFT JOIN`.

### ⏱ Time Complexity

Without an index: **O(n)** to scan and filter, plus **O(n log n)** to group.
With an index on `activity_date`: the range filter becomes closer to **O(log n) + O(k)**, where `k` is the number of rows in the window.

### 💾 Space Complexity

**O(d)**, where `d` is the number of distinct days with activity in the window.

### 🔄 Alternative Solution

```sql
-- Using explicit literal dates instead of DATE_SUB (less flexible, but sometimes clearer)
SELECT
  activity_date AS day,
  COUNT(DISTINCT user_id) AS active_users
FROM Activity
WHERE activity_date BETWEEN '2019-06-28' AND '2019-07-27'
GROUP BY activity_date;
```

Hardcoding the start date works for a one-off report, but `DATE_SUB()` is preferred in real applications since the window is often relative to "today" or a parameter rather than a fixed literal.

### 🎯 Key Takeaways

- "Last N days" ranges usually mean `(N - 1)` days back from the end date, not `N` days back — watch for off-by-one errors.
- `DATE_SUB`/`DATE_ADD` with `INTERVAL` are the correct, portable way to shift dates.
- Grouped results only include days present in the source data — missing days require a calendar table to appear as zero.

---

## 25. Product Sales Analysis III

**Difficulty:** 🟡 Medium
**Category:** Subquery

---

### 📋 Problem

A `Sales` table logs `sale_id`, `product_id`, `year`, `quantity`, and `price`. For each product, find the **quantity and price from the very first year it was sold**.

### 💻 SQL Solution

```sql
SELECT product_id, year AS first_year, quantity, price
FROM Sales
WHERE (product_id, year) IN (
  SELECT product_id, MIN(year)
  FROM Sales
  GROUP BY product_id
);
```

### 🔍 Explanation

- Subquery `SELECT product_id, MIN(year) FROM Sales GROUP BY product_id`: For each product, finds the earliest year it appears in the `Sales` table.
- `WHERE (product_id, year) IN (...)`: A row-value comparison that filters the outer query down to only the rows matching each product's first-sale year — using both columns together prevents accidentally matching the wrong product's earliest year.
- The outer `SELECT` then returns the quantity and price from exactly those first-year rows.

### ✅ Why This Solution Works

"First year sold" is inherently a per-product minimum, so the subquery computes that minimum grouped by product. Using a row-value `IN` (matching on the `(product_id, year)` pair together, not separately) guarantees each product's own first year is matched correctly — critical since different products started selling in different years.

### 🧠 SQL Concepts Used

- ✔ Subquery
- ✔ MIN()
- ✔ Row-value IN comparison
- ✔ GROUP BY

### 💡 Interview Tip

- Reinforces the "filter by a per-group minimum/maximum" pattern seen in several earlier questions — a foundational technique worth mastering.
- **Common mistake:** filtering with `WHERE year = (SELECT MIN(year) FROM Sales)` (a single global minimum) instead of pairing the minimum with each product individually.
- **Edge case:** if a product was sold multiple times in its very first year (multiple rows with the same `product_id` and minimum `year`), all of those rows would appear in the output — worth asking an interviewer whether that's expected.

### ⏱ Time Complexity

**O(n log n)** for the subquery's grouping, plus **O(n)** to filter the outer query — an index on `(product_id, year)` significantly speeds up both steps.

### 💾 Space Complexity

**O(p)**, where `p` is the number of distinct products, for the intermediate first-year results.

### 🔄 Alternative Solution

```sql
-- Using ROW_NUMBER() to pick exactly one row per product (MySQL 8.0+)
WITH RankedSales AS (
  SELECT
    product_id, year, quantity, price,
    ROW_NUMBER() OVER (PARTITION BY product_id ORDER BY year ASC) AS rn
  FROM Sales
)
SELECT product_id, year AS first_year, quantity, price
FROM RankedSales
WHERE rn = 1;
```

`ROW_NUMBER()` guarantees exactly one row per product even if there are ties in the earliest year, unlike the `MIN()` subquery approach which could return multiple tied rows.

### 🎯 Key Takeaways

- Row-value `IN` comparisons are a clean way to filter on a per-group `MIN`/`MAX` result.
- `ROW_NUMBER()` is useful when you need exactly one row per group, even in the presence of ties.
- Always consider whether ties in your "first"/"top" logic are acceptable or need explicit tie-breaking.

---

## 26. Classes With at Least 5 Students

**Difficulty:** 🟢 Easy
**Category:** GROUP BY / HAVING

---

### 📋 Problem

A `Courses` table logs `student` and `class`. Find all classes that have **5 or more** students enrolled.

### 💻 SQL Solution

```sql
SELECT class
FROM Courses
GROUP BY class
HAVING COUNT(DISTINCT student) >= 5;
```

### 🔍 Explanation

- `GROUP BY class`: Groups all enrollment rows by class name.
- `COUNT(DISTINCT student)`: Counts unique students per class — using `DISTINCT` protects against a student accidentally appearing twice for the same class.
- `HAVING COUNT(DISTINCT student) >= 5`: Filters groups (not individual rows) down to only classes meeting the enrollment threshold.

### ✅ Why This Solution Works

Since we need to count enrollments **per class** and then filter based on that count, aggregation (`GROUP BY` + `COUNT`) followed by a group-level filter (`HAVING`) is exactly the right tool. `DISTINCT` guards against inflated counts if duplicate student/class rows exist in the data.

### 🧠 SQL Concepts Used

- ✔ GROUP BY
- ✔ HAVING
- ✔ COUNT(DISTINCT)

### 💡 Interview Tip

- A clean, direct test of `GROUP BY` + `HAVING` — one of the most fundamental interview patterns.
- **Common mistake:** using `WHERE COUNT(DISTINCT student) >= 5` instead of `HAVING`, which fails because `WHERE` cannot reference aggregate functions.
- **Edge case:** if the same student is enrolled in the same class twice (duplicate rows), a plain `COUNT(student)` would overcount — always default to `COUNT(DISTINCT ...)` when uniqueness matters.

### ⏱ Time Complexity

**O(n log n)** for grouping — or **O(n)** with an index on `class` that avoids a full sort.

### 💾 Space Complexity

**O(c)**, where `c` is the number of distinct classes.

### 🔄 Alternative Solution

```sql
-- Using a subquery to pre-deduplicate before counting
SELECT class
FROM (SELECT DISTINCT student, class FROM Courses) t
GROUP BY class
HAVING COUNT(*) >= 5;
```

Logically identical — deduplicates first, then counts plain rows, instead of using `COUNT(DISTINCT ...)` inline.

### 🎯 Key Takeaways

- `HAVING` is required whenever you filter based on an aggregate result.
- `COUNT(DISTINCT ...)` protects against duplicate rows inflating your counts.
- This "group, count, filter" pattern is one of the most reusable building blocks in SQL.

---

## 27. Find Followers Count

**Difficulty:** 🟢 Easy
**Category:** GROUP BY / COUNT

---

### 📋 Problem

A `Followers` table logs `user_id` and `follower_id` — one row per follower relationship. For each user, count how many followers they have, sorted by `user_id`.

### 💻 SQL Solution

```sql
SELECT user_id, COUNT(follower_id) AS followers_count
FROM Followers
GROUP BY user_id
ORDER BY user_id;
```

### 🔍 Explanation

- `GROUP BY user_id`: Groups all follower relationships by the user being followed.
- `COUNT(follower_id)`: Counts how many follower rows exist per user.
- `ORDER BY user_id`: Sorts the final output in ascending order by user ID, as required.

### ✅ Why This Solution Works

Each row in `Followers` represents exactly one follow relationship, so grouping by `user_id` and counting rows directly gives the number of followers per user — no special deduplication is needed assuming each `(user_id, follower_id)` pair is unique in the source data.

### 🧠 SQL Concepts Used

- ✔ GROUP BY
- ✔ COUNT()
- ✔ ORDER BY

### 💡 Interview Tip

- A simple, foundational aggregation question — often used as a warm-up before harder social-graph questions (like "Friend Requests II" later in this handbook).
- **Common mistake:** forgetting `ORDER BY`, or using `COUNT(*)` vs `COUNT(follower_id)` inconsistently — both work the same here since `follower_id` shouldn't be `NULL`, but `COUNT(*)` is a safer default when column nullability isn't guaranteed to matter.
- **Edge case:** a user with zero followers won't appear in the output at all, since there's no row to group — this is expected behavior for this specific question.

### ⏱ Time Complexity

**O(n log n)** for grouping, or **O(n)** with an index on `user_id`.

### 💾 Space Complexity

**O(u)**, where `u` is the number of distinct users with at least one follower.

### 🔄 Alternative Solution

```sql
-- Using COUNT(*) instead of COUNT(follower_id)
SELECT user_id, COUNT(*) AS followers_count
FROM Followers
GROUP BY user_id
ORDER BY user_id;
```

Functionally identical here since `follower_id` is expected to always be populated — `COUNT(*)` counts rows regardless of `NULL`s, while `COUNT(column)` counts only non-`NULL` values in that column.

### 🎯 Key Takeaways

- `COUNT(*)` counts all rows; `COUNT(column)` counts only non-`NULL` values in that column.
- Grouping by the "target" entity (the user being followed) is the key insight for this kind of relationship-count question.
- Users with zero matching rows simply won't appear — add a `LEFT JOIN` against a master user list if zero-counts are required.

---

## 28. Biggest Single Number

**Difficulty:** 🟢 Easy
**Category:** Subquery / HAVING

---

### 📋 Problem

A `MyNumbers` table has a single column `num`, which may contain duplicates. A "single number" is one that appears **exactly once** in the table. Find the largest single number, or `NULL` if none exists.

### 💻 SQL Solution

```sql
SELECT MAX(num) AS num
FROM (
  SELECT num
  FROM MyNumbers
  GROUP BY num
  HAVING COUNT(*) = 1
) AS t;
```

### 🔍 Explanation

- Inner query: `GROUP BY num HAVING COUNT(*) = 1` groups identical values together and keeps only the groups (i.e., values) that appear exactly once — these are the "single numbers."
- Outer query: `MAX(num)` finds the largest value among those single numbers.

### ✅ Why This Solution Works

Identifying "appears exactly once" is inherently a group-level condition (you need to count occurrences of each value first), so `GROUP BY` + `HAVING COUNT(*) = 1` is the natural way to isolate qualifying numbers. Wrapping that result in an outer `MAX()` then finds the largest one — and if the inner query returns no rows at all, `MAX()` over an empty set correctly returns `NULL`, matching the requirement.

### 🧠 SQL Concepts Used

- ✔ Subquery
- ✔ GROUP BY
- ✔ HAVING
- ✔ MAX()

### 💡 Interview Tip

- Tests whether you understand that `MAX()` on an empty result set returns `NULL` automatically — no special-case handling needed.
- **Common mistake:** trying to solve this in one pass with `WHERE COUNT(*) = 1`, which is invalid syntax since `WHERE` can't use aggregate functions.
- **Edge case:** if every number in the table has a duplicate, the inner query returns zero rows, and `MAX()` gracefully returns `NULL` — exactly the required behavior, with no extra `IFNULL` needed.

### ⏱ Time Complexity

**O(n log n)** for the `GROUP BY`, plus **O(k)** for the outer `MAX()`, where `k` is the number of single numbers found.

### 💾 Space Complexity

**O(d)**, where `d` is the number of distinct values in `MyNumbers`, needed to compute group counts.

### 🔄 Alternative Solution

```sql
-- Using a window function to flag duplicates, then filtering (MySQL 8.0+)
WITH Counted AS (
  SELECT num, COUNT(*) OVER (PARTITION BY num) AS cnt
  FROM MyNumbers
)
SELECT MAX(num) AS num
FROM Counted
WHERE cnt = 1;
```

`COUNT(*) OVER (PARTITION BY num)` tags every row with its own value's frequency without collapsing rows via `GROUP BY` — useful if you need to keep other row-level data alongside the frequency count.

### 🎯 Key Takeaways

- `GROUP BY` + `HAVING COUNT(*) = 1` is the standard way to find values that appear exactly once.
- Aggregate functions like `MAX()` naturally return `NULL` when applied to zero rows — no extra handling required.
- Window functions (`COUNT() OVER (PARTITION BY ...)`) can compute frequency counts without collapsing the row set.

---

## 29. Customers Who Bought All Products

**Difficulty:** 🟡 Medium
**Category:** GROUP BY / HAVING / Subquery

---

### 📋 Problem

A `Customer` table logs `customer_id` and `product_key` for every product a customer has purchased. A `Product` table lists all available products (`product_key`). Find the IDs of customers who have bought **every single product** in the catalog.

### 💻 SQL Solution

```sql
SELECT customer_id
FROM Customer
GROUP BY customer_id
HAVING COUNT(DISTINCT product_key) = (SELECT COUNT(*) FROM Product);
```

### 🔍 Explanation

- `GROUP BY customer_id`: Groups all purchases by customer.
- `COUNT(DISTINCT product_key)`: Counts how many **unique** products each customer has purchased.
- `(SELECT COUNT(*) FROM Product)`: A scalar subquery computing the total number of products that exist in the catalog.
- `HAVING COUNT(DISTINCT product_key) = (...)`: Keeps only customers whose distinct-purchase count exactly equals the total catalog size — meaning they've bought literally everything.

### ✅ Why This Solution Works

"Bought all products" means a customer's set of purchased products must exactly match the full product catalog in size (assuming no invalid `product_key`s exist in `Customer`). Comparing `COUNT(DISTINCT product_key)` per customer against the total product count directly tests this — a classic **relational division** problem solved with grouping and a scalar subquery instead of more complex `NOT EXISTS` logic.

### 🧠 SQL Concepts Used

- ✔ GROUP BY
- ✔ HAVING
- ✔ COUNT(DISTINCT)
- ✔ Scalar Subquery

### 💡 Interview Tip

- This is a classic **"relational division"** problem — "find X that has ALL of Y" — a favorite advanced interview topic since it has multiple valid solving strategies.
- **Common mistake:** using `COUNT(product_key)` instead of `COUNT(DISTINCT product_key)`, which would overcount if a customer bought the same product more than once (e.g., in separate orders).
- **Edge case:** if the product catalog changes (grows or shrinks) after some purchases were made, the scalar subquery always reflects the *current* catalog size — meaning a customer who bought "everything" last month might no longer qualify if new products were added since.

### ⏱ Time Complexity

**O(n log n)** for grouping, plus **O(1)** for the constant scalar subquery — an index on `Customer(customer_id, product_key)` further speeds up the `COUNT(DISTINCT ...)` computation.

### 💾 Space Complexity

**O(c)**, where `c` is the number of distinct customers, for the grouped counts.

### 🔄 Alternative Solution

```sql
-- Using NOT EXISTS to find customers missing no products (relational division via double negation)
SELECT DISTINCT c.customer_id
FROM Customer c
WHERE NOT EXISTS (
  SELECT p.product_key
  FROM Product p
  WHERE NOT EXISTS (
    SELECT 1 FROM Customer c2
    WHERE c2.customer_id = c.customer_id AND c2.product_key = p.product_key
  )
);
```

This "double `NOT EXISTS`" pattern reads as "there is no product that this customer has *not* bought" — a more classic relational-algebra approach to division, useful to know since some interviewers specifically ask for this pattern.

### 🎯 Key Takeaways

- "Has ALL of" problems are known as relational division — solvable via count comparison or double `NOT EXISTS`.
- `COUNT(DISTINCT ...)` compared against a scalar subquery total is often the simplest approach.
- The scalar subquery denominator should reflect the *current* state of the reference table, which may have real-world implications worth discussing.

---

## 30. The Number of Employees Which Report to Each Employee

**Difficulty:** 🟢 Easy
**Category:** Self JOIN / Aggregation

---

### 📋 Problem

An `Employees` table has `employee_id`, `name`, `reports_to`, and `age`. For each employee who has at least one direct report, return their ID, name, the number of direct reports, and the **average age** of those direct reports (rounded to the nearest integer).

### 💻 SQL Solution

```sql
SELECT
  e1.employee_id,
  e1.name,
  COUNT(e2.employee_id) AS reports_count,
  ROUND(AVG(e2.age), 0) AS average_age
FROM Employees e1
JOIN Employees e2
  ON e1.employee_id = e2.reports_to
GROUP BY e1.employee_id, e1.name
ORDER BY e1.employee_id;
```

### 🔍 Explanation

- `FROM Employees e1 JOIN Employees e2 ON e1.employee_id = e2.reports_to`: A self-join where `e1` represents "the manager" and `e2` represents "someone who reports to that manager." Since we use `JOIN` (inner join), only employees with at least one match — i.e., at least one direct report — appear in `e1`.
- `COUNT(e2.employee_id)`: Counts how many direct reports each manager (`e1`) has.
- `ROUND(AVG(e2.age), 0)`: Averages the ages of those direct reports, rounded to the nearest whole number.
- `GROUP BY e1.employee_id, e1.name`: Groups by manager so the count and average apply per manager.
- `ORDER BY e1.employee_id`: Sorts the final output by manager ID.

### ✅ Why This Solution Works

Because the inner join only keeps rows where a matching `e2.reports_to = e1.employee_id` exists, employees with **zero** direct reports are automatically excluded — exactly matching the requirement to only include managers who actually have reports. Grouping by manager then lets `COUNT()` and `AVG()` summarize each manager's team correctly.

### 🧠 SQL Concepts Used

- ✔ Self JOIN
- ✔ INNER JOIN
- ✔ COUNT()
- ✔ AVG()
- ✔ ROUND()
- ✔ GROUP BY

### 💡 Interview Tip

- This tests whether you can correctly use an `INNER JOIN` (not `LEFT JOIN`) to *implicitly* filter out employees with no direct reports, rather than filtering afterward with `WHERE` or `HAVING`.
- **Common mistake:** using `LEFT JOIN`, which would include managers with zero reports and produce a `NULL` average age for them — technically wrong per the problem's requirements.
- **Edge case:** the top-level employee (with no manager, `reports_to IS NULL`) is unaffected by this query's logic since we're grouping by managers who *have* reports, not by who reports to whom at the top.

### ⏱ Time Complexity

Without an index: **O(n²)** for the self-join.
With an index on `reports_to`: closer to **O(n log n)**.

### 💾 Space Complexity

**O(m)**, where `m` is the number of managers with at least one direct report.

### 🔄 Alternative Solution

```sql
-- Using a subquery-based approach instead of a self-join
SELECT
  employee_id,
  name,
  reports_count,
  average_age
FROM Employees e
JOIN (
  SELECT reports_to, COUNT(*) AS reports_count, ROUND(AVG(age), 0) AS average_age
  FROM Employees
  WHERE reports_to IS NOT NULL
  GROUP BY reports_to
) sub
  ON e.employee_id = sub.reports_to
ORDER BY e.employee_id;
```

Pre-aggregating in a subquery before joining back to `Employees` can sometimes be more efficient on large tables, since the aggregation happens on a smaller intermediate result before the final join.

### 🎯 Key Takeaways

- `INNER JOIN` can be used deliberately to filter out "no match" cases without needing `WHERE`/`HAVING`.
- Self-joins are the standard tool for modeling hierarchical relationships (manager/report, parent/child).
- Always check whether `LEFT JOIN` vs `INNER JOIN` changes which rows should legitimately appear in the output.

---

## 31. Primary Department for Each Employee

**Difficulty:** 🟢 Easy
**Category:** UNION / GROUP BY

---

### 📋 Problem

An `Employee` table has `employee_id`, `department_id`, and `primary_flag` (`'Y'`/`'N'`). Employees belonging to only **one** department automatically have that as their primary department, even if `primary_flag` is `'N'`. Employees in multiple departments have exactly one row marked `primary_flag = 'Y'`. Return each employee's primary department.

### 💻 SQL Solution

```sql
SELECT employee_id, department_id
FROM Employee
GROUP BY employee_id
HAVING COUNT(*) = 1

UNION

SELECT employee_id, department_id
FROM Employee
WHERE primary_flag = 'Y';
```

### 🔍 Explanation

- First query: `GROUP BY employee_id HAVING COUNT(*) = 1` finds employees who appear in only **one** row total — meaning they belong to exactly one department, so that department is automatically primary regardless of the flag.
- Second query: `WHERE primary_flag = 'Y'` finds employees with multiple departments, picking out the one row explicitly marked as their primary department.
- `UNION`: Combines both result sets into one, automatically removing exact duplicate rows (though none are expected to overlap here, since an employee is either single-department or multi-department, never both).

### ✅ Why This Solution Works

The problem defines two separate rules for two separate cases: single-department employees (rule based on row count) and multi-department employees (rule based on the flag). Since no employee can satisfy both rules simultaneously, running two independent queries and combining them with `UNION` correctly covers every employee exactly once.

### 🧠 SQL Concepts Used

- ✔ UNION
- ✔ GROUP BY
- ✔ HAVING
- ✔ WHERE

### 💡 Interview Tip

- This tests whether you can decompose a problem with **two different business rules** into two separate queries joined by `UNION` — a very common real-world pattern for handling edge cases.
- **Common mistake:** trying to solve this with a single `WHERE primary_flag = 'Y' OR COUNT(*) = 1` in one query, which is invalid since `COUNT(*)` can't be used in `WHERE`, and conflating the two cases can also introduce logic bugs.
- **Edge case:** what if an employee has multiple departments but *no* row marked `'Y'` (bad data)? This solution would simply omit them — worth flagging as a data-quality assumption in an interview.

### ⏱ Time Complexity

**O(n log n)** for the first query's grouping, plus **O(n)** for the second query's filter, plus **O(n log n)** for `UNION`'s de-duplication step.

### 💾 Space Complexity

**O(e)**, where `e` is the number of distinct employees, for the combined result.

### 🔄 Alternative Solution

```sql
-- Using a window function to rank departments per employee (MySQL 8.0+)
WITH RankedDepts AS (
  SELECT
    employee_id,
    department_id,
    primary_flag,
    COUNT(*) OVER (PARTITION BY employee_id) AS dept_count
  FROM Employee
)
SELECT employee_id, department_id
FROM RankedDepts
WHERE dept_count = 1 OR primary_flag = 'Y';
```

`COUNT(*) OVER (PARTITION BY employee_id)` computes each employee's total department count without collapsing rows, letting a single `WHERE` clause handle both business rules at once instead of using `UNION`.

### 🎯 Key Takeaways

- `UNION` is a clean way to combine results from two different business rules that never overlap.
- `UNION` removes exact duplicate rows by default; use `UNION ALL` if duplicates should be preserved (and are cheaper to compute, since no de-duplication step is needed).
- Window functions can sometimes consolidate multi-query `UNION` logic into a single pass over the data.

---

## 32. Triangle Judgement

**Difficulty:** 🟢 Easy
**Category:** CASE

---

### 📋 Problem

A `Triangle` table has three side lengths per row: `x`, `y`, and `z`. For each row, determine whether the three sides can form a valid triangle.

### 💻 SQL Solution

```sql
SELECT
  x, y, z,
  CASE
    WHEN x + y > z AND x + z > y AND y + z > x THEN 'Yes'
    ELSE 'No'
  END AS triangle
FROM Triangle;
```

### 🔍 Explanation

- `CASE WHEN ... THEN ... ELSE ... END`: A conditional expression that evaluates a condition per row and returns one of two possible values — similar to an if/else statement.
- `x + y > z AND x + z > y AND y + z > x`: This is the **triangle inequality theorem** — three lengths can form a valid triangle only if the sum of any two sides is strictly greater than the third side, for all three combinations.
- `THEN 'Yes' ... ELSE 'No'`: Returns `'Yes'` if all three inequality checks pass, `'No'` otherwise.

### ✅ Why This Solution Works

A valid triangle must satisfy the triangle inequality for **all three** pairings of sides simultaneously — checking just one or two pairings isn't sufficient. Combining all three checks with `AND` inside the `CASE` expression ensures a row is only judged "Yes" when every condition holds true, correctly implementing the mathematical rule.

### 🧠 SQL Concepts Used

- ✔ CASE
- ✔ Logical AND
- ✔ Arithmetic Comparison

### 💡 Interview Tip

- This tests whether you know a real mathematical rule (triangle inequality) and can translate it correctly into a `CASE` expression with `AND` — interviewers use domain-knowledge questions like this to see how you handle unfamiliar business logic.
- **Common mistake:** checking only one pairing (e.g., `x + y > z`) instead of all three — this is the single most common bug in this question.
- **Edge case:** degenerate triangles where a side sum exactly equals the third side (e.g., `x + y = z`) should be judged `'No'`, since the inequality is strict (`>`, not `>=`).

### ⏱ Time Complexity

**O(n)** — a straightforward per-row evaluation with no sorting or grouping required.

### 💾 Space Complexity

**O(1)** — no additional storage needed beyond the output.

### 🔄 Alternative Solution

```sql
-- Using IF() instead of CASE (MySQL-specific shorthand)
SELECT
  x, y, z,
  IF(x + y > z AND x + z > y AND y + z > x, 'Yes', 'No') AS triangle
FROM Triangle;
```

`IF(condition, true_value, false_value)` is a MySQL-specific shorthand for simple two-branch logic — functionally identical to `CASE` here, but less portable to other database systems like PostgreSQL or SQL Server.

### 🎯 Key Takeaways

- `CASE` expressions are SQL's standard tool for conditional, row-level logic.
- Some business rules (like the triangle inequality) require checking multiple conditions with `AND`, not just one.
- `IF()` is a MySQL-only shortcut for simple `CASE` logic — `CASE` is more portable across database systems.

---

## 33. Consecutive Numbers

**Difficulty:** 🟡 Medium
**Category:** Self JOIN

---

### 📋 Problem

A `Logs` table has `id` (sequential, no gaps) and `num`. Find all numbers that appear **at least three times in a row** (in three consecutive `id` values).

### 💻 SQL Solution

```sql
SELECT DISTINCT l1.num AS ConsecutiveNums
FROM Logs l1
JOIN Logs l2 ON l1.id = l2.id - 1
JOIN Logs l3 ON l2.id = l3.id - 1
WHERE l1.num = l2.num
  AND l2.num = l3.num;
```

### 🔍 Explanation

- `FROM Logs l1 JOIN Logs l2 ON l1.id = l2.id - 1 JOIN Logs l3 ON l2.id = l3.id - 1`: A **triple self-join** that lines up three consecutive rows side by side — `l1` is row `n`, `l2` is row `n+1`, and `l3` is row `n+2`.
- `WHERE l1.num = l2.num AND l2.num = l3.num`: Keeps only triples where all three consecutive rows share the exact same `num` value.
- `SELECT DISTINCT l1.num`: Returns the qualifying number, de-duplicated — since a run of 5 identical numbers, for example, would otherwise produce multiple matching triples for the same value.

### ✅ Why This Solution Works

To detect "three in a row," we need three consecutive rows visible simultaneously so we can compare their values directly — a single-row query can't do this. Chaining two self-joins (`l1`→`l2`→`l3`, each offset by exactly one `id`) lines up every possible group of three consecutive rows, and the `WHERE` clause then checks if all three share the same number.

### 🧠 SQL Concepts Used

- ✔ Self JOIN (multiple)
- ✔ WHERE
- ✔ SELECT DISTINCT

### 💡 Interview Tip

- This is a well-known advanced self-join question — interviewers use it to test whether you can extend the "compare adjacent rows" pattern (seen in "Rising Temperature") to three or more rows.
- **Common mistake:** relying on `id` differences (`l1.id = l2.id - 1`) when the table could have gaps in `id` values — this solution assumes `id` is perfectly sequential, which should always be confirmed with the interviewer.
- **Edge case:** a run of 4 or more identical numbers should still return the number just once thanks to `DISTINCT` — without it, longer runs would produce multiple duplicate rows in the output.

### ⏱ Time Complexity

Without an index: **O(n³)** in the worst theoretical case for a triple self-join, though MySQL's optimizer typically handles equality joins on `id` far more efficiently in practice.
With an index on `id` (usually the primary key): closer to **O(n)**, since each join step is a fast lookup.

### 💾 Space Complexity

**O(k)**, where `k` is the number of distinct qualifying numbers.

### 🔄 Alternative Solution

```sql
-- Using LAG() window functions instead of a self-join (MySQL 8.0+)
WITH Flagged AS (
  SELECT
    num,
    LAG(num, 1) OVER (ORDER BY id) AS prev1,
    LAG(num, 2) OVER (ORDER BY id) AS prev2
  FROM Logs
)
SELECT DISTINCT num AS ConsecutiveNums
FROM Flagged
WHERE num = prev1 AND num = prev2;
```

`LAG(num, 2)` looks back two rows without needing any joins at all — often more readable and can be more efficient than a triple self-join on large tables, since it avoids the join's potential cost entirely.

### 🎯 Key Takeaways

- Comparing N consecutive rows generally requires N-1 self-joins (or a `LAG`/`LEAD` window function).
- Always confirm whether `id` sequences can have gaps before joining on `id ± 1` arithmetic.
- `LAG()`/`LEAD()` window functions are often a cleaner, more efficient alternative to multiple self-joins.

---

## 34. Product Price at a Given Date

**Difficulty:** 🟡 Medium
**Category:** Subquery / LEFT JOIN

---

### 📋 Problem

A `Products` table logs every price change: `product_id`, `new_price`, and `change_date`. If a product has no price change recorded by a target date (`2019-08-16`), its price defaults to `10`. Find the price of every product as of that date.

### 💻 SQL Solution

```sql
SELECT p1.product_id, IFNULL(p2.new_price, 10) AS price
FROM (SELECT DISTINCT product_id FROM Products) p1
LEFT JOIN (
  SELECT product_id, new_price
  FROM Products
  WHERE (product_id, change_date) IN (
    SELECT product_id, MAX(change_date)
    FROM Products
    WHERE change_date <= '2019-08-16'
    GROUP BY product_id
  )
) p2
  ON p1.product_id = p2.product_id;
```

### 🔍 Explanation

- `(SELECT DISTINCT product_id FROM Products) p1`: Builds the complete list of every product that has ever had a price entry — this ensures every product appears in the final output.
- Innermost subquery: `SELECT product_id, MAX(change_date) FROM Products WHERE change_date <= '2019-08-16' GROUP BY product_id` finds the **most recent** price change on or before the target date, for each product.
- Middle subquery `p2`: Uses that latest-date info via a row-value `IN` to fetch the actual `new_price` that was in effect on the target date.
- `LEFT JOIN p1 to p2`: Ensures products with **no** price change before the target date still appear (with `p2.new_price` as `NULL`).
- `IFNULL(p2.new_price, 10)`: Falls back to the default price of `10` whenever no applicable price change was found.

### ✅ Why This Solution Works

Finding "the price as of a given date" is really finding the **most recent price change that happened on or before that date** — a per-product maximum date, filtered by the date cutoff. The nested subqueries isolate that latest applicable price change, and the outer `LEFT JOIN` against the full product list guarantees products with no qualifying price change still show up with the correct default of `10`, rather than being silently dropped.

### 🧠 SQL Concepts Used

- ✔ Subquery (nested)
- ✔ MAX()
- ✔ Row-value IN comparison
- ✔ LEFT JOIN
- ✔ IFNULL()

### 💡 Interview Tip

- This is a "point-in-time" or "as-of" query — an extremely common real-world pattern for pricing history, account balances, or any slowly-changing dimension.
- **Common mistake:** using `MAX(change_date)` across *all* changes instead of only those `<= '2019-08-16'`, which would incorrectly use future price changes that hadn't taken effect yet on the target date.
- **Edge case:** a product with **only** price changes after the target date should default to `10`, not use its earliest recorded price — the `WHERE change_date <= '2019-08-16'` filter correctly excludes those future changes entirely.

### ⏱ Time Complexity

**O(n log n)** for the nested `MAX(change_date)` grouping, plus **O(n)** for the joins — an index on `(product_id, change_date)` significantly improves performance for both steps.

### 💾 Space Complexity

**O(p)**, where `p` is the number of distinct products.

### 🔄 Alternative Solution

```sql
-- Using ROW_NUMBER() to pick the latest applicable price directly (MySQL 8.0+)
WITH RankedPrices AS (
  SELECT
    product_id,
    new_price,
    ROW_NUMBER() OVER (PARTITION BY product_id ORDER BY change_date DESC) AS rn
  FROM Products
  WHERE change_date <= '2019-08-16'
)
SELECT DISTINCT p.product_id, IFNULL(r.new_price, 10) AS price
FROM Products p
LEFT JOIN RankedPrices r
  ON p.product_id = r.product_id AND r.rn = 1;
```

`ROW_NUMBER()` ordered by `change_date DESC` directly ranks each product's applicable price changes, letting you grab the top-ranked (`rn = 1`) row per product without nested nested subqueries.

### 🎯 Key Takeaways

- "As-of date" queries require finding the latest record *before or on* a target date, not just the overall latest record.
- `LEFT JOIN` combined with `IFNULL` is essential for supplying default values when no historical record applies.
- `ROW_NUMBER() OVER (PARTITION BY ... ORDER BY ...)` is a powerful, readable alternative to nested `MAX()` subqueries for "most recent record per group" problems.

---

## 35. Last Person to Fit in the Bus

**Difficulty:** 🟡 Medium
**Category:** Window Function

---

### 📋 Problem

A `Queue` table has `person_id`, `person_name`, `weight`, and `turn` (their position in line). People board a bus one at a time in `turn` order. The bus has a weight limit of 1000. Find the name of the **last** person who can board without exceeding the weight limit.

### 💻 SQL Solution

```sql
SELECT person_name
FROM (
  SELECT
    person_name,
    SUM(weight) OVER (ORDER BY turn) AS cumulative_weight
  FROM Queue
) t
WHERE cumulative_weight <= 1000
ORDER BY cumulative_weight DESC
LIMIT 1;
```

### 🔍 Explanation

- `SUM(weight) OVER (ORDER BY turn)`: A **window function** that computes a running total — for each row, it sums the weights of everyone up to and including that person's `turn`, without collapsing rows the way `GROUP BY` would.
- Inner query produces every person alongside their cumulative weight up to their position in line.
- `WHERE cumulative_weight <= 1000`: Keeps only people whose position in line doesn't push the total weight over the limit.
- `ORDER BY cumulative_weight DESC LIMIT 1`: Among the people who fit, picks the one with the highest cumulative weight — which corresponds to the very last person who could board before the limit would be exceeded.

### ✅ Why This Solution Works

Boarding order matters because each person's ability to board depends on the **total weight of everyone before them**, not just their own weight. A running total (window function `SUM() OVER (ORDER BY turn)`) captures exactly this cumulative effect for every position in line. Filtering to totals within the limit, then taking the highest such total, identifies the final person who boards successfully.

### 🧠 SQL Concepts Used

- ✔ Window Function (SUM() OVER)
- ✔ ORDER BY (within window and in outer query)
- ✔ WHERE
- ✔ LIMIT

### 💡 Interview Tip

- This is a great test of whether you understand **running totals** — one of the most useful window function patterns, applicable to running balances, cumulative sales, and more.
- **Common mistake:** trying to solve this with a self-join and `GROUP BY` summing weights of "everyone before me," which works but is far more verbose and harder to reason about than a window function.
- **Edge case:** if the very first person's weight already exceeds 1000, the inner query would produce zero qualifying rows after filtering, and the outer query would correctly return an empty result — worth mentioning as a sanity check.

### ⏱ Time Complexity

**O(n log n)** for the window function's implicit sort by `turn`, though MySQL can use an index on `turn` to avoid an explicit sort.

### 💾 Space Complexity

**O(n)** — window functions typically require materializing the ordered result set to compute running values.

### 🔄 Alternative Solution

```sql
-- Using a self-join to compute the running total manually (works in MySQL 5.7 and earlier)
SELECT q1.person_name
FROM Queue q1
JOIN Queue q2
  ON q2.turn <= q1.turn
GROUP BY q1.person_id, q1.person_name, q1.turn
HAVING SUM(q2.weight) <= 1000
ORDER BY SUM(q2.weight) DESC
LIMIT 1;
```

This achieves the same running-total logic without window functions (useful for pre-8.0 MySQL versions), but is significantly less efficient since it performs a self-join across all preceding rows for every person.

### 🎯 Key Takeaways

- `SUM(column) OVER (ORDER BY ...)` computes a running/cumulative total without collapsing rows.
- Running totals are essential for "how much has accumulated by this point" problems (balances, capacity limits, leaderboards).
- Window functions (MySQL 8.0+) are almost always cleaner and more efficient than the equivalent self-join for cumulative calculations.

---

## 36. Count Salary Categories

**Difficulty:** 🟡 Medium
**Category:** CASE / UNION

---

### 📋 Problem

An `Accounts` table has `account_id` and `income`. Categorize each account as `'Low Salary'` (income `< 20000`), `'Average Salary'` (income between `20000` and `50000` inclusive), or `'High Salary'` (income `> 50000`). Return the count of accounts in each category — including categories with a count of `0`.

### 💻 SQL Solution

```sql
SELECT 'Low Salary' AS category, COUNT(*) AS accounts_count
FROM Accounts WHERE income < 20000

UNION

SELECT 'Average Salary' AS category, COUNT(*) AS accounts_count
FROM Accounts WHERE income BETWEEN 20000 AND 50000

UNION

SELECT 'High Salary' AS category, COUNT(*) AS accounts_count
FROM Accounts WHERE income > 50000;
```

### 🔍 Explanation

- Each of the three `SELECT` statements computes the count of accounts in one specific salary bracket, using a literal string (`'Low Salary'`, etc.) as a constant label column.
- `WHERE income < 20000` / `BETWEEN 20000 AND 50000` / `> 50000`: These three conditions are mutually exclusive and collectively exhaustive — every account falls into exactly one bracket.
- `UNION`: Stacks the three single-row results into one combined result set, one row per category.

### ✅ Why This Solution Works

Since each `SELECT` in the `UNION` runs an independent `COUNT(*)` over the *entire* table (filtered by its own condition), every category is guaranteed to produce exactly one row — even if its count is `0` — because `COUNT(*)` over zero matching rows still returns `0`, not an empty result. This is what makes the "include zero-count categories" requirement work naturally, unlike a `GROUP BY` approach which would simply omit categories with no matching data.

### 🧠 SQL Concepts Used

- ✔ UNION
- ✔ COUNT()
- ✔ WHERE / BETWEEN
- ✔ Literal / Constant Columns

### 💡 Interview Tip

- This tests a subtle but important distinction: `GROUP BY` **omits** empty groups, while three independent `COUNT(*)` queries combined with `UNION` **always** produce a row per category, even when the count is zero.
- **Common mistake:** trying to solve this with a single `GROUP BY CASE WHEN ... END` query — this actually works too (see the alternative below), but many candidates forget it fails to show zero-count categories unless every category is guaranteed to have at least one matching row.
- **Edge case:** ensure the three `WHERE` conditions don't overlap or leave gaps — `BETWEEN 20000 AND 50000` is inclusive on both ends, so double-check boundary values like exactly `20000` or `50000` land in the correct bucket.

### ⏱ Time Complexity

**O(3n)** — the table is scanned three separate times (once per `SELECT`), so this is roughly three times the cost of a single full scan, though each individual scan is simple.

### 💾 Space Complexity

**O(1)** — only three rows of output, regardless of table size.

### 🔄 Alternative Solution

```sql
-- Using a single GROUP BY with CASE (only safe if all categories are guaranteed non-empty)
SELECT
  CASE
    WHEN income < 20000 THEN 'Low Salary'
    WHEN income BETWEEN 20000 AND 50000 THEN 'Average Salary'
    ELSE 'High Salary'
  END AS category,
  COUNT(*) AS accounts_count
FROM Accounts
GROUP BY category;
```

This single-pass version is more efficient (only one table scan), but it will **silently omit** any category that has zero matching accounts — a real risk if the data doesn't guarantee all three brackets are populated. The `UNION` version in the primary solution is the safer choice when zero-count categories must always be shown.

### 🎯 Key Takeaways

- Independent `UNION`-ed `COUNT(*)` queries guarantee every category appears, even with a zero count.
- `GROUP BY` only returns groups that actually have matching rows — it cannot manufacture empty groups.
- `BETWEEN` is inclusive on both boundaries — always verify edge values land in the intended bucket.

---

## 37. Employees Whose Manager Left the Company

**Difficulty:** 🟢 Easy
**Category:** LEFT JOIN / Subquery

---

### 📋 Problem

An `Employees` table has `employee_id`, `name`, `manager_id`, and `salary`. Find employees earning **less than 30000** whose manager no longer exists in the company (i.e., `manager_id` points to an ID that isn't a valid `employee_id`).

### 💻 SQL Solution

```sql
SELECT employee_id
FROM Employees
WHERE salary < 30000
  AND manager_id IS NOT NULL
  AND manager_id NOT IN (SELECT employee_id FROM Employees)
ORDER BY employee_id;
```

### 🔍 Explanation

- `WHERE salary < 30000`: First filters down to lower-salary employees.
- `AND manager_id IS NOT NULL`: Excludes employees who have no manager at all (their `manager_id` is `NULL`) — these employees don't have a "manager who left," they simply never had one.
- `AND manager_id NOT IN (SELECT employee_id FROM Employees)`: Checks whether the employee's manager ID exists anywhere in the current employee list — if it doesn't, that manager must have left the company.
- `ORDER BY employee_id`: Sorts the final result.

### ✅ Why This Solution Works

A manager who "left the company" is represented in the data by their `employee_id` no longer existing in the table, while employees who used to report to them still reference that now-missing ID. The subquery builds the full list of currently valid employee IDs, and `NOT IN` checks whether each employee's `manager_id` is missing from that list — meaning their manager left. Explicitly filtering out `NULL` `manager_id`s first prevents a subtle bug (explained in the interview tip below).

### 🧠 SQL Concepts Used

- ✔ WHERE
- ✔ Subquery
- ✔ NOT IN
- ✔ IS NOT NULL
- ✔ ORDER BY

### 💡 Interview Tip

- This tests a critical `NOT IN` gotcha: if the subquery could return any `NULL` values, `NOT IN` behaves unpredictably and can return **zero rows** for the entire query, even when matches clearly exist.
- **Common mistake:** omitting `AND manager_id IS NOT NULL`, which would incorrectly include employees who never had a manager in the first place, since their `manager_id IS NULL` and `NULL NOT IN (...)` evaluates to `UNKNOWN`, not `TRUE` — actually causing those specific rows to be silently dropped, but it's still best practice to filter explicitly for clarity and safety.
- **Edge case:** always confirm the subquery's column (`employee_id`) can never be `NULL` — if it could, the entire `NOT IN` clause could unexpectedly return zero rows for every employee, not just the ones you intend to exclude.

### ⏱ Time Complexity

Without an index: **O(n × m)**, since `NOT IN` may require comparing against the full subquery result for each row.
With an index on `Employees.employee_id` (the primary key): the subquery lookup becomes much faster, closer to **O(n log n)**.

### 💾 Space Complexity

**O(n)** — the subquery's result (list of valid employee IDs) may be materialized in memory.

### 🔄 Alternative Solution

```sql
-- Using NOT EXISTS instead of NOT IN (safer against NULLs)
SELECT e1.employee_id
FROM Employees e1
WHERE e1.salary < 30000
  AND e1.manager_id IS NOT NULL
  AND NOT EXISTS (
    SELECT 1 FROM Employees e2 WHERE e2.employee_id = e1.manager_id
  )
ORDER BY e1.employee_id;
```

`NOT EXISTS` is generally the **safer** choice over `NOT IN` when there's any chance the subquery could return `NULL` values, since `NOT EXISTS` uses row existence logic rather than direct value comparison and isn't affected by `NULL` the same way.

### 🎯 Key Takeaways

- `NOT IN` is dangerous if the subquery can return `NULL` values — it can silently return zero rows for the whole query.
- `NOT EXISTS` is the safer, more predictable alternative for "does not exist in another table" logic.
- Always explicitly filter out `NULL` values in join/filter keys when their presence has a different business meaning (like "never had a manager" vs. "manager left").

---

## 38. Exchange Seats

**Difficulty:** 🟡 Medium
**Category:** CASE / Modulo

---

### 📋 Problem

A `Seat` table has `id` and `student`, ordered by `id`. Swap every pair of adjacent seats (1↔2, 3↔4, and so on). If there's an odd number of seats, the last student keeps their seat.

### 💻 SQL Solution

```sql
SELECT
  CASE
    WHEN id % 2 = 1 AND id = (SELECT MAX(id) FROM Seat) THEN id
    WHEN id % 2 = 0 THEN id - 1
    WHEN id % 2 = 1 THEN id + 1
  END AS id,
  student
FROM Seat
ORDER BY id;
```

### 🔍 Explanation

- `WHEN id % 2 = 1 AND id = (SELECT MAX(id) FROM Seat) THEN id`: Handles the special case of an **odd-numbered last seat** with no pair to swap with — it keeps its own `id` unchanged. The subquery `(SELECT MAX(id) FROM Seat)` finds the highest seat ID to detect this scenario.
- `WHEN id % 2 = 0 THEN id - 1`: For even-numbered seats, subtract 1 to swap into the position of the seat before them.
- `WHEN id % 2 = 1 THEN id + 1`: For all other odd-numbered seats (not the last one), add 1 to swap into the position after them.
- `ORDER BY id`: Sorts the final output by the newly computed `id` values.

### ✅ Why This Solution Works

The `CASE` expression checks conditions **in order**, so the special "last odd seat" case is evaluated first, before the general odd/even swap rules — this ensures it takes priority and isn't accidentally caught by the generic `id % 2 = 1 THEN id + 1` rule. For all other seats, simple arithmetic (`+1` for odd, `-1` for even) correctly implements a pairwise swap of adjacent seat numbers.

### 🧠 SQL Concepts Used

- ✔ CASE (multi-branch)
- ✔ Modulo Operator
- ✔ Scalar Subquery (MAX)
- ✔ ORDER BY

### 💡 Interview Tip

- This tests careful handling of an **edge case within a pattern** — the odd/even swap rule is simple, but the last-seat exception requires spotting it before writing code.
- **Common mistake:** forgetting the "odd count of seats" edge case entirely, which causes the last student to be swapped with a non-existent seat and disappear from a naive implementation (or produce a `NULL` id).
- **Edge case:** always test with both an even and an odd total number of seats — many candidates only test the even case, which passes even with a broken implementation.

### ⏱ Time Complexity

**O(n log n)** due to the final `ORDER BY` sort, or **O(n)** if the seats are already physically ordered by `id` and MySQL can skip an explicit sort.

### 💾 Space Complexity

**O(1)** additional space beyond the output rows themselves.

### 🔄 Alternative Solution

```sql
-- Using LEAD() and LAG() window functions (MySQL 8.0+)
SELECT
  id,
  COALESCE(
    CASE WHEN id % 2 = 1 THEN LEAD(student) OVER (ORDER BY id) END,
    CASE WHEN id % 2 = 0 THEN LAG(student) OVER (ORDER BY id) END,
    student
  ) AS student
FROM Seat
ORDER BY id;
```

This swaps the **student names** while keeping `id` values fixed and in place — a different but equally valid way to represent the same swapped seating, using `LEAD()`/`LAG()` to peek at neighboring rows and `COALESCE` to fall back to the original student if no swap partner exists (the odd-seat-out case).

### 🎯 Key Takeaways

- `CASE` evaluates conditions top-to-bottom — always put special-case exceptions before general rules.
- Modulo (`%`) is a versatile tool for alternating/pairing logic, not just simple odd/even checks.
- Always test boundary conditions (odd vs. even counts) explicitly — they're the most common source of bugs in pairing/swapping logic.

---

## 39. Movie Rating

**Difficulty:** 🟡 Medium
**Category:** UNION / JOIN

---

### 📋 Problem

`Movies` has `movie_id`/`title`, `Users` has `user_id`/`name`, and `MovieRating` logs every rating (`movie_id`, `user_id`, `rating`, `created_at`). Find:
1. The name of the user who has rated the **most** movies (ties broken alphabetically by name).
2. The title of the movie with the **highest average rating** in February 2020 (ties broken alphabetically by title).
Return both as a single column named `results`.

### 💻 SQL Solution

```sql
(SELECT u.name AS results
 FROM MovieRating mr
 JOIN Users u ON mr.user_id = u.user_id
 GROUP BY mr.user_id, u.name
 ORDER BY COUNT(*) DESC, u.name ASC
 LIMIT 1)

UNION ALL

(SELECT m.title AS results
 FROM MovieRating mr
 JOIN Movies m ON mr.movie_id = m.movie_id
 WHERE DATE_FORMAT(mr.created_at, '%Y-%m') = '2020-02'
 GROUP BY mr.movie_id, m.title
 ORDER BY AVG(mr.rating) DESC, m.title ASC
 LIMIT 1);
```

### 🔍 Explanation

- First subquery: Joins ratings to users, groups by user, counts how many ratings each user submitted (`COUNT(*)`), and sorts by that count descending — with `u.name ASC` as a tiebreaker — then takes the top row with `LIMIT 1`.
- Second subquery: Joins ratings to movies, filters to only February 2020 using `DATE_FORMAT()`, groups by movie, computes each movie's `AVG(rating)`, sorts by average descending (tiebreaker: title ascending), and takes the top row.
- `UNION ALL`: Stacks both single-row results into one two-row output. `UNION ALL` (not plain `UNION`) is used here because we specifically want to keep both rows even if, coincidentally, they contained the same text — we're not trying to de-duplicate two logically different answers.

### ✅ Why This Solution Works

The two parts of the question are **completely independent calculations** (most active rater vs. best-rated movie in a specific month) that happen to share the same output column name and type (`results`, a string). Solving them as two separate `GROUP BY` + `ORDER BY` + `LIMIT 1` queries and stacking them with `UNION ALL` is the cleanest way to produce the required two-row report from otherwise unrelated logic.

### 🧠 SQL Concepts Used

- ✔ UNION ALL
- ✔ JOIN
- ✔ GROUP BY
- ✔ COUNT() / AVG()
- ✔ ORDER BY (with tiebreaker) / LIMIT

### 💡 Interview Tip

- This tests whether you can decompose a multi-part question into independent sub-queries and combine them cleanly — a common structure for "top N per category" style business questions.
- **Common mistake:** using `UNION` instead of `UNION ALL` — while it usually doesn't change the result here (the two values are unlikely to be identical strings), `UNION ALL` is the semantically correct choice since we're not trying to de-duplicate, and it also avoids the extra performance cost of `UNION`'s de-duplication step.
- **Edge case:** always include a tiebreaker in the `ORDER BY` (`u.name ASC`, `m.title ASC`) — without one, ties are broken arbitrarily by the database engine, which could produce inconsistent results across runs.

### ⏱ Time Complexity

**O(n log n)** for each subquery's sort step — both subqueries scan and sort independently, so the total cost is roughly the sum of both.

### 💾 Space Complexity

**O(u + m)**, where `u` is the number of users and `m` is the number of movies rated in the target month, for the intermediate grouped results.

### 🔄 Alternative Solution

```sql
-- Using window functions with RANK() to avoid relying on LIMIT 1 (MySQL 8.0+)
(SELECT name AS results FROM (
  SELECT u.name, RANK() OVER (ORDER BY COUNT(*) DESC, u.name ASC) AS rnk
  FROM MovieRating mr JOIN Users u ON mr.user_id = u.user_id
  GROUP BY mr.user_id, u.name
) t WHERE rnk = 1)

UNION ALL

(SELECT title AS results FROM (
  SELECT m.title, RANK() OVER (ORDER BY AVG(mr.rating) DESC, m.title ASC) AS rnk
  FROM MovieRating mr JOIN Movies m ON mr.movie_id = m.movie_id
  WHERE DATE_FORMAT(mr.created_at, '%Y-%m') = '2020-02'
  GROUP BY mr.movie_id, m.title
) t WHERE rnk = 1);
```

Using `RANK()` instead of `ORDER BY ... LIMIT 1` explicitly handles true ties by returning **all** tied top rows, rather than arbitrarily picking just one — useful to discuss with an interviewer if the business rule for ties isn't perfectly clear.

### 🎯 Key Takeaways

- `UNION ALL` is preferred over `UNION` when you don't need (or want) automatic de-duplication.
- Always specify a tiebreaker column in `ORDER BY` when using `LIMIT 1` for "top result" queries.
- `RANK()` can surface all tied top results, while `ORDER BY ... LIMIT 1` silently picks just one.

---

## 40. Restaurant Growth

**Difficulty:** 🟡 Medium
**Category:** Window Function

---

### 📋 Problem

A `Customer` table logs `customer_id`, `name`, `visited_on`, and `amount` per visit. For every date starting from the 7th distinct day onward, compute the **7-day moving sum** and **7-day moving average** of total daily spend, rounded to 2 decimal places.

### 💻 SQL Solution

```sql
SELECT visited_on, amount, average_amount
FROM (
  SELECT
    visited_on,
    SUM(amount) OVER (ORDER BY visited_on ROWS BETWEEN 6 PRECEDING AND CURRENT ROW) AS amount,
    ROUND(AVG(amount) OVER (ORDER BY visited_on ROWS BETWEEN 6 PRECEDING AND CURRENT ROW), 2) AS average_amount,
    ROW_NUMBER() OVER (ORDER BY visited_on) AS rn
  FROM (
    SELECT visited_on, SUM(amount) AS amount
    FROM Customer
    GROUP BY visited_on
  ) daily
) windowed
WHERE rn >= 7
ORDER BY visited_on;
```

### 🔍 Explanation

- Innermost query: `GROUP BY visited_on` first collapses multiple customers' spend on the same day into a single daily total — this is necessary because the moving window should operate on *daily totals*, not individual transactions.
- `SUM(amount) OVER (ORDER BY visited_on ROWS BETWEEN 6 PRECEDING AND CURRENT ROW)`: A window function computing a **moving/rolling sum** — for each day, it sums that day's total plus the 6 days immediately before it (7 days total).
- `AVG(amount) OVER (...)` with the same window frame: Computes the moving average over the same 7-day window.
- `ROW_NUMBER() OVER (ORDER BY visited_on)`: Numbers each distinct day sequentially, so we can identify which days have a full 7-day window available.
- Outer `WHERE rn >= 7`: Excludes the first 6 days, which don't yet have a complete 7-day window behind them.

### ✅ Why This Solution Works

`ROWS BETWEEN 6 PRECEDING AND CURRENT ROW` defines a **sliding window** of exactly 7 rows (the current day plus the 6 before it) for each computation — this is precisely what "7-day moving sum/average" means. Since the first 6 days in the dataset don't have 6 full prior days to include, their windows would be incomplete (partial), so `ROW_NUMBER()` is used to explicitly filter them out, ensuring every reported value truly represents a full 7-day period.

### 🧠 SQL Concepts Used

- ✔ Window Function (SUM/AVG OVER)
- ✔ ROWS BETWEEN (window frame)
- ✔ ROW_NUMBER()
- ✔ GROUP BY (pre-aggregation)
- ✔ ROUND()

### 💡 Interview Tip

- This is one of the best tests of true **window frame** understanding (`ROWS BETWEEN ... PRECEDING AND CURRENT ROW`), which is more advanced than simple `PARTITION BY`/`ORDER BY` window usage.
- **Common mistake:** forgetting to pre-aggregate by `visited_on` first — without collapsing multiple same-day transactions into one row, the window function would operate on individual transactions instead of daily totals, producing incorrect sums.
- **Edge case:** the first 6 distinct days must be excluded from the final output since they don't have a full 7-day trailing window — this is easy to overlook without an explicit `ROW_NUMBER()` filter.

### ⏱ Time Complexity

**O(n log n)** for the initial `GROUP BY` and the window function's implicit sort by `visited_on`.

### 💾 Space Complexity

**O(d)**, where `d` is the number of distinct visit dates, to hold the daily totals and window computations.

### 🔄 Alternative Solution

```sql
-- Using a self-join based date range instead of a window frame (works pre-MySQL 8.0)
SELECT
  d1.visited_on,
  SUM(d2.amount) AS amount,
  ROUND(AVG(d2.amount), 2) AS average_amount
FROM (SELECT visited_on, SUM(amount) AS amount FROM Customer GROUP BY visited_on) d1
JOIN (SELECT visited_on, SUM(amount) AS amount FROM Customer GROUP BY visited_on) d2
  ON d2.visited_on BETWEEN DATE_SUB(d1.visited_on, INTERVAL 6 DAY) AND d1.visited_on
GROUP BY d1.visited_on
HAVING COUNT(*) = 7
ORDER BY d1.visited_on;
```

This achieves the same rolling window using a self-join with a `BETWEEN` date range instead of `ROWS BETWEEN`, useful for MySQL versions prior to 8.0 that lack window function support — `HAVING COUNT(*) = 7` ensures only complete 7-day windows are kept.

### 🎯 Key Takeaways

- `ROWS BETWEEN n PRECEDING AND CURRENT ROW` defines a fixed-size sliding window for moving sums/averages.
- Always pre-aggregate to the correct grain (daily totals, in this case) before applying a window function.
- `ROW_NUMBER()` (or `HAVING COUNT(*) = n` in the self-join version) is essential for excluding incomplete windows at the start of a dataset.

---

## 41. Friend Requests II: Who Has the Most Friends

**Difficulty:** 🟡 Medium
**Category:** UNION ALL / GROUP BY

---

### 📋 Problem

A `RequestAccepted` table logs accepted friend requests via `requester_id` and `accepter_id`. Each accepted request means both people become friends with each other. Find the person with the **most** friends and their friend count. You may assume there is exactly one person with the maximum count.

### 💻 SQL Solution

```sql
SELECT id, COUNT(*) AS num
FROM (
  SELECT requester_id AS id FROM RequestAccepted
  UNION ALL
  SELECT accepter_id AS id FROM RequestAccepted
) all_friends
GROUP BY id
ORDER BY num DESC
LIMIT 1;
```

### 🔍 Explanation

- `SELECT requester_id AS id FROM RequestAccepted UNION ALL SELECT accepter_id AS id FROM RequestAccepted`: Since an accepted friend request creates a mutual friendship, each person's "friend count" needs to include instances where they were **either** the requester **or** the accepter. `UNION ALL` stacks both roles into a single unified list of IDs, one row per friendship-from-that-person's-perspective.
- `GROUP BY id`: Groups the combined list by person, so each person's total appearances (as requester or accepter) can be counted.
- `COUNT(*)`: Counts how many times each person appears across both roles — this equals their total number of friends.
- `ORDER BY num DESC LIMIT 1`: Picks the person with the highest friend count.

### ✅ Why This Solution Works

A friendship is symmetric — if A accepted B's request, both A and B gain one friend. Since each row in `RequestAccepted` only lists the pair once, a person's total friend count requires combining their appearances from **both** columns. `UNION ALL` (not `UNION`) correctly stacks all appearances without removing legitimate duplicates (e.g., if a person is a requester in one row and an accepter in another, both should count separately toward their total).

### 🧠 SQL Concepts Used

- ✔ UNION ALL
- ✔ GROUP BY
- ✔ COUNT()
- ✔ ORDER BY / LIMIT

### 💡 Interview Tip

- This tests whether you understand **symmetric relationships** in relational data — a very common modeling challenge (friendships, mutual follows, bidirectional edges in a graph).
- **Common mistake:** using `UNION` instead of `UNION ALL`, which would incorrectly deduplicate rows and produce inaccurate counts whenever a person's ID happens to repeat identically across the two `SELECT`s in a way that `UNION`'s deduplication logic would collapse.
- **Edge case:** if the same friendship pair somehow appears more than once in `RequestAccepted` (a potential data quality issue), it would be double-counted — worth clarifying whether the source table guarantees unique pairs.

### ⏱ Time Complexity

**O(n log n)** for the `GROUP BY` over the combined `2n`-row unioned set (where `n` is the number of accepted requests).

### 💾 Space Complexity

**O(p)**, where `p` is the number of distinct people, for the grouped friend counts.

### 🔄 Alternative Solution

```sql
-- Using RANK() to handle potential ties explicitly, instead of assuming a single winner
SELECT id, num
FROM (
  SELECT id, COUNT(*) AS num, RANK() OVER (ORDER BY COUNT(*) DESC) AS rnk
  FROM (
    SELECT requester_id AS id FROM RequestAccepted
    UNION ALL
    SELECT accepter_id AS id FROM RequestAccepted
  ) all_friends
  GROUP BY id
) ranked
WHERE rnk = 1;
```

Using `RANK()` instead of `LIMIT 1` explicitly returns **all** people tied for the most friends, rather than silently picking one — a more robust approach if the "exactly one maximum" assumption can't be guaranteed in production data.

### 🎯 Key Takeaways

- `UNION ALL` is essential (not `UNION`) when combining two roles of the same symmetric relationship, since deduplication would corrupt the counts.
- Symmetric/bidirectional relationships often require "flattening" two columns into one before aggregating.
- `RANK()` is safer than `LIMIT 1` whenever ties are a realistic possibility.

---

## 42. Investments in 2016

**Difficulty:** 🟡 Medium
**Category:** Subquery / GROUP BY

---

### 📋 Problem

An `Insurance` table logs `pid`, `tiv_2015`, `tiv_2016`, `lat`, and `lon`. Find the total `tiv_2016` for all policyholders who: (1) had the **same** `tiv_2015` value as at least one other policyholder, **and** (2) do **not** share their exact `(lat, lon)` location with any other policyholder.

### 💻 SQL Solution

```sql
SELECT ROUND(SUM(tiv_2016), 2) AS tiv_2016
FROM Insurance
WHERE tiv_2015 IN (
  SELECT tiv_2015
  FROM Insurance
  GROUP BY tiv_2015
  HAVING COUNT(*) > 1
)
AND (lat, lon) IN (
  SELECT lat, lon
  FROM Insurance
  GROUP BY lat, lon
  HAVING COUNT(*) = 1
);
```

### 🔍 Explanation

- First subquery: `GROUP BY tiv_2015 HAVING COUNT(*) > 1` finds `tiv_2015` values that are **shared** by more than one policyholder — these are the values we want to keep (condition 1).
- Second subquery: `GROUP BY lat, lon HAVING COUNT(*) = 1` finds `(lat, lon)` location pairs that belong to **only one** policyholder — meaning that policyholder's location is unique (condition 2).
- Outer `WHERE tiv_2015 IN (...) AND (lat, lon) IN (...)`: Combines both conditions — a policyholder must satisfy *both* to be included.
- `SUM(tiv_2016)`: Sums the 2016 investment value across all qualifying policyholders.

### ✅ Why This Solution Works

The two conditions are independent group-level facts about the data — "is this `tiv_2015` shared?" and "is this location unique?" — so each is computed separately via its own `GROUP BY`/`HAVING`, then both filters are applied together in the outer query's `WHERE` clause using `AND`. This correctly identifies only the policyholders satisfying both criteria simultaneously before summing their `tiv_2016`.

### 🧠 SQL Concepts Used

- ✔ Subquery (multiple)
- ✔ GROUP BY
- ✔ HAVING
- ✔ Row-value IN comparison
- ✔ SUM()

### 💡 Interview Tip

- This question combines **two opposite group-filtering conditions** (one requiring duplicates, one requiring uniqueness) — testing whether you can keep both requirements straight without confusing `> 1` and `= 1`.
- **Common mistake:** mixing up the `HAVING` thresholds — using `HAVING COUNT(*) > 1` for the location check (which should be `= 1` for uniqueness) or vice versa for the `tiv_2015` check.
- **Edge case:** a policyholder could have a `NULL` `lat`/`lon` — depending on how the row-value comparison handles `NULL`, such rows might be silently excluded; worth clarifying data quality assumptions with an interviewer.

### ⏱ Time Complexity

**O(n log n)** for each of the two `GROUP BY` subqueries, plus **O(n)** for the outer filter — indexes on `tiv_2015` and `(lat, lon)` would speed up both grouping steps.

### 💾 Space Complexity

**O(t + l)**, where `t` is the number of distinct `tiv_2015` values and `l` is the number of distinct `(lat, lon)` pairs, for the intermediate grouped results.

### 🔄 Alternative Solution

```sql
-- Using window functions to compute both counts inline, avoiding separate subqueries (MySQL 8.0+)
WITH Flagged AS (
  SELECT
    tiv_2016,
    COUNT(*) OVER (PARTITION BY tiv_2015) AS tiv_2015_count,
    COUNT(*) OVER (PARTITION BY lat, lon) AS location_count
  FROM Insurance
)
SELECT ROUND(SUM(tiv_2016), 2) AS tiv_2016
FROM Flagged
WHERE tiv_2015_count > 1
  AND location_count = 1;
```

`COUNT(*) OVER (PARTITION BY ...)` computes both group counts in a single pass over the data without separate subqueries, which can be more efficient than two independent `GROUP BY` operations on large tables.

### 🎯 Key Takeaways

- Multiple independent group-level conditions can each be computed in their own subquery, then combined with `AND` in the outer `WHERE`.
- Carefully distinguish `HAVING COUNT(*) > 1` (shared/duplicated) from `HAVING COUNT(*) = 1` (unique) — mixing these up is a common source of bugs.
- Window functions with `PARTITION BY` can sometimes replace multiple separate `GROUP BY` subqueries for better readability and performance.

---

## 43. Department Top Three Salaries

**Difficulty:** 🔴 Hard
**Category:** Window Function (DENSE_RANK)

---

### 📋 Problem

An `Employee` table has `id`, `name`, `salary`, and `departmentId`. A `Department` table has `id` and `name`. For each department, find the employees who are among the **top three highest-paid** in their department (with ties counting as the same rank — e.g., two people tied for 1st still leaves room for a 2nd and 3rd).

### 💻 SQL Solution

```sql
SELECT d.name AS Department, e.name AS Employee, e.salary AS Salary
FROM (
  SELECT
    id, name, salary, departmentId,
    DENSE_RANK() OVER (PARTITION BY departmentId ORDER BY salary DESC) AS rnk
  FROM Employee
) e
JOIN Department d ON e.departmentId = d.id
WHERE e.rnk <= 3;
```

### 🔍 Explanation

- `DENSE_RANK() OVER (PARTITION BY departmentId ORDER BY salary DESC)`: A window function that assigns a rank to each employee **within their own department** (`PARTITION BY departmentId` resets the ranking for each department), ordered from highest to lowest salary. `DENSE_RANK()` specifically means tied salaries receive the **same** rank, and the next distinct salary continues at the very next rank number (no gaps) — unlike plain `RANK()`, which would skip ranks after a tie.
- Inner query computes this rank for every employee.
- `JOIN Department d ON e.departmentId = d.id`: Attaches the human-readable department name.
- `WHERE e.rnk <= 3`: Keeps only employees ranked 1st, 2nd, or 3rd within their department (accounting for ties sharing a rank).

### ✅ Why This Solution Works

"Top three salaries per department" is a **per-group ranking** problem — exactly what `PARTITION BY` was designed for, since it resets the `ORDER BY salary DESC` ranking independently for each department instead of ranking globally across the entire company. `DENSE_RANK()` is specifically chosen (over `RANK()` or `ROW_NUMBER()`) because the problem explicitly states that ties should share a rank without leaving gaps — e.g., two employees tied for 1st should both be included, and the next employee should be ranked 2nd, not 3rd.

### 🧠 SQL Concepts Used

- ✔ Window Function (DENSE_RANK)
- ✔ PARTITION BY
- ✔ JOIN
- ✔ WHERE (post-window filter)

### 💡 Interview Tip

- This is one of the most important window function questions to master — interviewers use it specifically to test whether you know the difference between `ROW_NUMBER()`, `RANK()`, and `DENSE_RANK()`.
- **Common mistake:** using `ROW_NUMBER()` instead of `DENSE_RANK()`, which would arbitrarily break ties and potentially exclude a legitimately tied top-3 employee, or using `RANK()`, which leaves gaps after ties (e.g., two people tied for 1st, then the next person is ranked 3rd, not 2nd) — subtly different from what "top three" should mean here.
- **Edge case:** you **cannot** filter with `WHERE DENSE_RANK() OVER (...) <= 3` directly in the same query level — window functions are computed *after* `WHERE` normally runs, so this logic must be wrapped in a subquery (or CTE) and filtered in an outer layer, as shown in the primary solution.

### ⏱ Time Complexity

**O(n log n)** for the window function's per-department sort — an index on `(departmentId, salary)` can significantly reduce the sorting cost.

### 💾 Space Complexity

**O(n)** — window functions generally require materializing the full partitioned/sorted dataset to assign ranks.

### 🔄 Alternative Solution

```sql
-- Pre-2016 MySQL approach without window functions: correlated subquery counting higher distinct salaries
SELECT d.name AS Department, e1.name AS Employee, e1.salary AS Salary
FROM Employee e1
JOIN Department d ON e1.departmentId = d.id
WHERE (
  SELECT COUNT(DISTINCT e2.salary)
  FROM Employee e2
  WHERE e2.departmentId = e1.departmentId
    AND e2.salary > e1.salary
) < 3;
```

This correlated subquery counts how many **distinct** higher salaries exist in the same department — if fewer than 3 salaries beat this employee's, they're in the top 3. This pattern works on MySQL versions before 8.0 (which lacked window function support), but is significantly less efficient on large tables since the subquery re-evaluates for every row.

### 🎯 Key Takeaways

- `PARTITION BY` resets a window function's calculation independently for each group — essential for "top N per category" problems.
- `DENSE_RANK()` handles ties without gaps; `RANK()` leaves gaps after ties; `ROW_NUMBER()` ignores ties entirely and assigns arbitrary unique numbers.
- Window function results can't be filtered directly in the same `WHERE` clause where they're defined — wrap them in a subquery or CTE first.

---

## 44. Fix Names in a Table

**Difficulty:** 🟢 Easy
**Category:** String Functions

---

### 📋 Problem

A `Users` table has `user_id` and `name`, but names are inconsistently capitalized (e.g., `'aLICE'`, `'John'`). Fix each name so only the first letter is uppercase and the rest are lowercase, sorted by `user_id`.

### 💻 SQL Solution

```sql
SELECT
  user_id,
  CONCAT(UPPER(LEFT(name, 1)), LOWER(SUBSTRING(name, 2))) AS name
FROM Users
ORDER BY user_id;
```

### 🔍 Explanation

- `LEFT(name, 1)`: Extracts just the first character of the name.
- `UPPER(...)`: Converts that first character to uppercase.
- `SUBSTRING(name, 2)`: Extracts every character **from position 2 onward** (i.e., everything except the first letter). SQL string positions are 1-indexed, so position 2 is the second character.
- `LOWER(...)`: Converts that remaining substring to lowercase.
- `CONCAT(..., ...)`: Joins the fixed first letter and the fixed remainder back into a single properly-capitalized name.
- `ORDER BY user_id`: Sorts the final result.

### ✅ Why This Solution Works

Proper capitalization requires treating the first character differently from the rest of the string — so the name is split into two pieces (`LEFT` for the first letter, `SUBSTRING` for the rest), each piece is transformed with the appropriate case function, and `CONCAT` reassembles them into the final corrected name.

### 🧠 SQL Concepts Used

- ✔ String Functions (UPPER, LOWER, LEFT, SUBSTRING, CONCAT)
- ✔ ORDER BY

### 💡 Interview Tip

- Tests basic but essential string manipulation — very common in data-cleaning interview questions.
- **Common mistake:** using `UPPER(name)` or `LOWER(name)` on the *entire* string instead of splitting it, which fixes case consistency but doesn't achieve proper "Title Case" capitalization.
- **Edge case:** what happens with an empty string or a `NULL` name? `LEFT('', 1)` returns an empty string, and `SUBSTRING(NULL, 2)` returns `NULL` — worth testing these boundary cases explicitly if the schema allows them.

### ⏱ Time Complexity

**O(n log n)** due to the final `ORDER BY` sort — the string transformation itself is **O(1)** per row (constant-time string operations), so **O(n)** overall before sorting.

### 💾 Space Complexity

**O(1)** additional space per row for the transformed string.

### 🔄 Alternative Solution

```sql
-- Using CONCAT_WS or INSERT-based manipulation as a stylistic variant
SELECT
  user_id,
  CONCAT(UPPER(SUBSTRING(name, 1, 1)), LOWER(SUBSTRING(name, 2))) AS name
FROM Users
ORDER BY user_id;
```

`SUBSTRING(name, 1, 1)` is functionally identical to `LEFT(name, 1)` — both extract the first character; this alternative is purely a stylistic/consistency choice some teams prefer since it uses `SUBSTRING` throughout instead of mixing `LEFT` and `SUBSTRING`.

### 🎯 Key Takeaways

- String manipulation often requires splitting a string into parts, transforming each part independently, then reassembling with `CONCAT`.
- SQL string positions are 1-indexed, not 0-indexed like many programming languages.
- Always consider empty-string and `NULL` edge cases when writing string transformation logic.

---

## 45. Patients With a Condition

**Difficulty:** 🟢 Easy
**Category:** LIKE

---

### 📋 Problem

A `Patients` table has `patient_id`, `patient_name`, and `conditions` (a space-separated list of medical condition codes). Find all patients who have **Type I Diabetes**, indicated by any code starting with `'DIAB1'` anywhere in the `conditions` field.

### 💻 SQL Solution

```sql
SELECT *
FROM Patients
WHERE conditions LIKE 'DIAB1%'
   OR conditions LIKE '% DIAB1%';
```

### 🔍 Explanation

- `LIKE 'DIAB1%'`: The `%` is a wildcard matching any sequence of characters. This pattern matches conditions where a code starting with `'DIAB1'` appears at the **very beginning** of the string.
- `OR conditions LIKE '% DIAB1%'`: This pattern matches a code starting with `'DIAB1'` appearing **anywhere after the first word**, since it requires a space immediately before `'DIAB1'`.
- Combining both patterns with `OR` correctly catches `'DIAB1'`-prefixed codes whether they're the first condition listed or a later one.

### ✅ Why This Solution Works

Because `conditions` is a space-separated list, a code like `'DIAB100'` could either be the very first entry (no leading space) or a later entry (preceded by a space). Two separate `LIKE` patterns are needed to correctly cover both positions — a single pattern like `'%DIAB1%'` would incorrectly match unrelated codes that merely *contain* the substring `'DIAB1'` in the middle of a different code (e.g., a hypothetical `'XDIAB123'`).

### 🧠 SQL Concepts Used

- ✔ LIKE
- ✔ Wildcard Matching (%)
- ✔ Logical OR

### 💡 Interview Tip

- This tests careful pattern-matching design — specifically, recognizing that a naive `'%DIAB1%'` pattern is **too loose** and could produce false positives.
- **Common mistake:** using just `WHERE conditions LIKE '%DIAB1%'`, which would incorrectly match any code that merely contains the substring `'DIAB1'` anywhere, even in the middle of an unrelated code name.
- **Edge case:** always think about word boundaries when using `LIKE` on space- or comma-separated fields — this is a common data-modeling pitfall (ideally, such multi-value fields would be normalized into a separate table, which is worth mentioning as a best-practice aside in an interview).

### ⏱ Time Complexity

**O(n)** — a leading wildcard-free pattern (`'DIAB1%'`) can potentially use an index, but the second pattern (`'% DIAB1%'`) starts with a wildcard, which generally **prevents** index usage and forces a full table scan.

### 💾 Space Complexity

**O(1)** — no additional storage needed beyond the output.

### 🔄 Alternative Solution

```sql
-- Using REGEXP for more precise word-boundary matching
SELECT *
FROM Patients
WHERE conditions REGEXP '(^|[[:space:]])DIAB1';
```

`REGEXP` with `(^|[[:space:]])` matches `'DIAB1'` only when it's at the very start of the string (`^`) or immediately preceded by whitespace — a more precise, single-expression way to enforce the same "must be a whole condition code" boundary logic as the two `LIKE` patterns combined.

### 🎯 Key Takeaways

- `LIKE` wildcards (`%`, `_`) are powerful but can produce false positives if not anchored carefully.
- Space- or comma-separated multi-value fields often need multiple `LIKE` patterns (or a regex) to correctly enforce word boundaries.
- `REGEXP` can express complex boundary conditions more precisely than chained `LIKE` patterns, at some cost to readability and portability.

---

## 46. Delete Duplicate Emails

**Difficulty:** 🟢 Easy
**Category:** DELETE / Self JOIN

---

### 📋 Problem

A `Person` table has `id` and `email`. Some emails appear more than once. Delete all duplicate rows, keeping only the one with the **smallest** `id` for each email.

### 💻 SQL Solution

```sql
DELETE p1
FROM Person p1
JOIN Person p2
  ON p1.email = p2.email
 AND p1.id > p2.id;
```

### 🔍 Explanation

- `DELETE p1 FROM Person p1 JOIN Person p2 ...`: This is a **multi-table DELETE** — MySQL allows deleting from one table (`p1`) based on a join condition involving another reference to the same table (`p2`).
- `ON p1.email = p2.email`: Matches rows that share the same email address.
- `AND p1.id > p2.id`: For each pair of rows with a matching email, this condition is only true when `p1` has a **larger** ID than `p2` — meaning `p1` represents a "later, duplicate" row that should be deleted, while `p2` (with the smaller ID) is preserved.
- The `DELETE` statement removes every `p1` row that matched this join condition.

### ✅ Why This Solution Works

For any pair of duplicate rows sharing an email, exactly one of them has the smaller `id` and one has the larger `id`. The self-join pairs up every duplicate combination, and the condition `p1.id > p2.id` ensures only the "larger ID" copy of each pair gets targeted by `DELETE p1` — the smallest-ID row for each email is never selected as `p1` in a way that gets deleted, since no other row with an even smaller ID and the same email exists to trigger the condition against it.

### 🧠 SQL Concepts Used

- ✔ DELETE
- ✔ Self JOIN
- ✔ Multi-table DELETE syntax

### 💡 Interview Tip

- This tests whether you know MySQL's multi-table `DELETE` syntax, which differs from standard single-table deletes and trips up many candidates who've only practiced `SELECT` self-joins.
- **Common mistake:** writing `DELETE FROM p1` instead of `DELETE p1 FROM ...` — the table alias to delete from must come immediately after `DELETE`, not after `FROM`.
- **Edge case:** always test this on a copy of the data first — `DELETE` is a destructive, irreversible operation (without a transaction/backup), unlike a `SELECT` query which is safe to experiment with freely.

### ⏱ Time Complexity

Without an index: **O(n²)** for the self-join comparison.
With an index on `email`: closer to **O(n log n)**, since matching duplicate emails becomes much faster.

### 💾 Space Complexity

**O(1)** additional space — `DELETE` operates in place, though the database may use temporary space internally to identify matching rows before removing them.

### 🔄 Alternative Solution

```sql
-- Using a subquery-based DELETE (an alternative syntax some engineers prefer)
DELETE FROM Person
WHERE id NOT IN (
  SELECT MIN(id) FROM Person GROUP BY email
);
```

**Caution:** in MySQL, you generally cannot directly reference the same table being deleted from inside a subquery without wrapping it in an extra derived table (e.g., `SELECT * FROM (SELECT MIN(id) ... ) AS tmp`) due to a restriction on referencing the target table in a subquery — this alternative illustrates the logic, but may require that extra wrapping to actually execute in MySQL.

### 🎯 Key Takeaways

- MySQL's multi-table `DELETE p1 FROM p1 JOIN p2 ...` syntax lets you delete rows based on a self-join condition.
- Always test destructive `DELETE` statements against a backup or in a transaction before running them on production data.
- `GROUP BY` + `MIN(id)` is a common pattern for identifying "the row to keep" among duplicates.

---

## 47. Second Highest Salary

**Difficulty:** 🟢 Easy
**Category:** Subquery / LIMIT OFFSET

---

### 📋 Problem

An `Employee` table has `id` and `salary`. Find the **second highest distinct** salary. If no second-highest salary exists (e.g., only one employee, or all salaries are identical), return `NULL`.

### 💻 SQL Solution

```sql
SELECT
  (SELECT DISTINCT salary
   FROM Employee
   ORDER BY salary DESC
   LIMIT 1 OFFSET 1) AS SecondHighestSalary;
```

### 🔍 Explanation

- `SELECT DISTINCT salary FROM Employee`: Removes duplicate salary values, so tied salaries only count as **one** distinct value (important since "second highest" means second-highest distinct amount, not second row).
- `ORDER BY salary DESC`: Sorts distinct salaries from highest to lowest.
- `LIMIT 1 OFFSET 1`: `OFFSET 1` skips the very first row (the highest salary), and `LIMIT 1` then takes exactly the next row — which is the second-highest distinct salary.
- Wrapping the whole thing in an outer `SELECT (...)  AS SecondHighestSalary`: This scalar-subquery wrapping is what makes the query **always return exactly one row**, even if the inner query finds zero matching rows — in that case, the outer `SELECT` returns a single row with a `NULL` value instead of an empty result set.

### ✅ Why This Solution Works

The `DISTINCT` + `ORDER BY DESC` + `OFFSET 1` combination directly implements "skip the highest, then take the next" — a precise translation of "second highest." Critically, wrapping the subquery as a **scalar subquery** in the outer `SELECT` guarantees `NULL` is returned gracefully when no second value exists, rather than the query returning zero rows entirely (which many interview platforms explicitly penalize, since they expect a row with `NULL`, not an empty result set).

### 🧠 SQL Concepts Used

- ✔ Subquery (Scalar)
- ✔ SELECT DISTINCT
- ✔ ORDER BY
- ✔ LIMIT / OFFSET

### 💡 Interview Tip

- This is one of the most iconic SQL interview questions of all time — interviewers use it to test whether you handle the "no second value exists" edge case gracefully (returning `NULL`) rather than letting the query silently return nothing.
- **Common mistake:** forgetting `DISTINCT`, which would treat two employees tied for the highest salary as occupying both the "1st" and "2nd" positions — incorrectly reporting the tied highest salary as the "second highest" instead of the actual next-lower one.
- **Edge case:** an `Employee` table with only one employee (or one distinct salary) must return `NULL`, not an error or empty result — the scalar-subquery wrapping handles this automatically.

### ⏱ Time Complexity

**O(n log n)** for the `DISTINCT` + `ORDER BY` sort — an index on `salary` can help avoid a full sort by allowing MySQL to read values in already-sorted order.

### 💾 Space Complexity

**O(d)**, where `d` is the number of distinct salary values, needed to de-duplicate before sorting.

### 🔄 Alternative Solution

```sql
-- Using a subquery with MAX() excluding the top salary
SELECT MAX(salary) AS SecondHighestSalary
FROM Employee
WHERE salary < (SELECT MAX(salary) FROM Employee);
```

This finds the highest salary that is strictly *less than* the overall maximum — logically equivalent to "second highest distinct salary," and it also gracefully returns `NULL` if no such salary exists, since `MAX()` over zero rows returns `NULL`.

### 🎯 Key Takeaways

- `LIMIT ... OFFSET ...` is the standard way to skip a fixed number of top/bottom rows after sorting.
- Wrapping a subquery as a scalar value in an outer `SELECT` guarantees a single-row result (with `NULL` if nothing matches), instead of an empty result set.
- Always use `DISTINCT` when "Nth highest" should mean Nth highest *distinct* value, not just the Nth row.

---

## 48. Group Sold Products By The Date

**Difficulty:** 🟡 Medium
**Category:** GROUP_CONCAT

---

### 📋 Problem

An `Activities` table has `sell_date` and `product`. For each date, return the number of **distinct** products sold and a comma-separated, alphabetically sorted list of those distinct product names.

### 💻 SQL Solution

```sql
SELECT
  sell_date,
  COUNT(DISTINCT product) AS num_sold,
  GROUP_CONCAT(DISTINCT product ORDER BY product SEPARATOR ',') AS products
FROM Activities
GROUP BY sell_date
ORDER BY sell_date;
```

### 🔍 Explanation

- `COUNT(DISTINCT product)`: Counts the unique product names sold on each date.
- `GROUP_CONCAT(DISTINCT product ORDER BY product SEPARATOR ',')`: A MySQL-specific aggregate function that combines multiple row values into a **single comma-separated string** per group. `DISTINCT` removes duplicate product names, `ORDER BY product` ensures they appear alphabetically within the string, and `SEPARATOR ','` sets the comma as the joining character.
- `GROUP BY sell_date`: Produces one summary row per distinct sale date.
- `ORDER BY sell_date`: Sorts the final output chronologically.

### ✅ Why This Solution Works

`GROUP_CONCAT()` is purpose-built for exactly this kind of requirement — turning multiple related row values into one readable summary string per group. Combined with `DISTINCT` (to avoid repeating the same product twice on one date) and an internal `ORDER BY` (to guarantee alphabetical ordering within the string itself, independent of the row order MySQL happens to process), it produces exactly the format the question asks for.

### 🧠 SQL Concepts Used

- ✔ GROUP_CONCAT
- ✔ COUNT(DISTINCT)
- ✔ GROUP BY
- ✔ ORDER BY (both outer and inside GROUP_CONCAT)

### 💡 Interview Tip

- This tests knowledge of `GROUP_CONCAT` — a MySQL-specific function that's extremely useful in real-world reporting but isn't part of the standard SQL you'd use in every database engine (PostgreSQL uses `STRING_AGG`, for example).
- **Common mistake:** forgetting the `ORDER BY` **inside** `GROUP_CONCAT()`, which controls the order of items *within* the concatenated string — this is separate from the outer `ORDER BY sell_date`, which only controls the order of the *rows themselves*.
- **Edge case:** `GROUP_CONCAT()` has a default maximum output length (`group_concat_max_len`, often 1024 characters) — for dates with a very large number of distinct products, the string could be silently truncated unless this server setting is increased.

### ⏱ Time Complexity

**O(n log n)** for grouping and internal sorting within `GROUP_CONCAT`.

### 💾 Space Complexity

**O(d)**, where `d` is the number of distinct dates, though each row's storage cost depends on the length of its concatenated product string.

### 🔄 Alternative Solution

```sql
-- Explicitly casting for clarity, and using a shorter separator syntax
SELECT
  sell_date,
  COUNT(DISTINCT product) AS num_sold,
  GROUP_CONCAT(DISTINCT product ORDER BY product ASC) AS products
FROM Activities
GROUP BY sell_date
ORDER BY sell_date;
```

`GROUP_CONCAT`'s default separator is already a comma, so `SEPARATOR ','` can technically be omitted — this alternative is functionally identical but relies on the default rather than specifying it explicitly (many teams prefer being explicit for readability, as in the primary solution).

### 🎯 Key Takeaways

- `GROUP_CONCAT()` is the MySQL-specific tool for combining multiple grouped values into one string.
- `GROUP_CONCAT` supports its own internal `DISTINCT`, `ORDER BY`, and `SEPARATOR` clauses, independent of the outer query's clauses.
- Be aware of `group_concat_max_len` in production systems — long concatenated strings can be silently truncated.

---

## 49. List the Products Ordered in a Period

**Difficulty:** 🟢 Easy
**Category:** JOIN / HAVING

---

### 📋 Problem

A `Products` table has `product_id`, `product_name`, and `product_category`. An `Orders` table has `product_id`, `order_date`, and `unit`. Find the names and total ordered units of all products that had **at least 100 units** ordered during **February 2020**.

### 💻 SQL Solution

```sql
SELECT p.product_name, SUM(o.unit) AS unit
FROM Products p
JOIN Orders o
  ON p.product_id = o.product_id
WHERE o.order_date BETWEEN '2020-02-01' AND '2020-02-29'
GROUP BY p.product_id, p.product_name
HAVING SUM(o.unit) >= 100;
```

### 🔍 Explanation

- `JOIN Orders o ON p.product_id = o.product_id`: Connects each order to its product's name and category.
- `WHERE o.order_date BETWEEN '2020-02-01' AND '2020-02-29'`: Filters orders down to just those placed during February 2020 (2020 was a leap year, so February had 29 days).
- `GROUP BY p.product_id, p.product_name`: Groups the filtered orders by product, so quantities can be summed per product.
- `SUM(o.unit)`: Totals the units ordered for each product within the filtered date range.
- `HAVING SUM(o.unit) >= 100`: Filters out products whose February total didn't reach the 100-unit threshold — a group-level filter, since it depends on the aggregated `SUM()`.

### ✅ Why This Solution Works

The question has three layers: restrict to a specific time period (`WHERE`), total up quantities per product (`GROUP BY` + `SUM`), and then keep only products meeting a quantity threshold (`HAVING`). Applying these in the correct order — filter rows first, then aggregate, then filter the aggregated result — produces exactly the required list of qualifying products and their February totals.

### 🧠 SQL Concepts Used

- ✔ JOIN
- ✔ WHERE (date range filtering)
- ✔ GROUP BY
- ✔ SUM()
- ✔ HAVING

### 💡 Interview Tip

- This question nicely combines all the core filtering/aggregation concepts (`WHERE` vs. `HAVING`, date ranges, joins, grouping) into one query — a great "does the candidate understand the full pipeline" test.
- **Common mistake:** using `WHERE SUM(o.unit) >= 100` instead of `HAVING`, or filtering the date range in `HAVING` instead of `WHERE` — remember: `WHERE` filters rows before aggregation, `HAVING` filters after.
- **Edge case:** always double check leap years when hardcoding February date ranges — using `'2020-02-29'` is correct for 2020, but would need to be `'2020-02-28'` (or better, computed dynamically) for a non-leap year.

### ⏱ Time Complexity

**O(n × m)** for the join without indexes, or **O(n log m)** with an index on `Orders.product_id` — plus **O(n log n)** for the grouping step.

### 💾 Space Complexity

**O(p)**, where `p` is the number of distinct products with qualifying orders.

### 🔄 Alternative Solution

```sql
-- Using DATE_FORMAT for a more explicit month/year match instead of BETWEEN
SELECT p.product_name, SUM(o.unit) AS unit
FROM Products p
JOIN Orders o
  ON p.product_id = o.product_id
WHERE DATE_FORMAT(o.order_date, '%Y-%m') = '2020-02'
GROUP BY p.product_id, p.product_name
HAVING SUM(o.unit) >= 100;
```

Using `DATE_FORMAT()` to match the year-month string avoids needing to know the exact number of days in the target month — a more robust choice when the target period could vary across different months/years.

### 🎯 Key Takeaways

- `WHERE` filters individual rows (like a date range) before aggregation; `HAVING` filters the aggregated groups afterward.
- Always verify calendar details (like leap years) when hardcoding date literals.
- `DATE_FORMAT()` matching is often more robust and readable than manually calculating exact date range boundaries.

---

## 50. Find Users With Valid E-Mails

**Difficulty:** 🟢 Easy
**Category:** REGEXP

---

### 📋 Problem

A `Users` table has `user_id`, `name`, and `mail`. Find all users with a **valid** email address, defined as: starting with a letter, followed by any combination of letters, digits, underscores, periods, or dashes, and ending in exactly `'@leetcode.com'`.

### 💻 SQL Solution

```sql
SELECT *
FROM Users
WHERE mail REGEXP '^[a-zA-Z][a-zA-Z0-9_.-]*@leetcode\\.com$';
```

### 🔍 Explanation

- `REGEXP '...'`: Matches the `mail` column against a **regular expression** pattern, allowing much more precise text validation than `LIKE`.
- `^`: Anchors the match to the **start** of the string — nothing can come before this pattern begins.
- `[a-zA-Z]`: Requires the very first character to be a single letter (upper or lowercase).
- `[a-zA-Z0-9_.-]*`: Matches zero or more of the following characters after the first letter: letters, digits, underscores, periods, or dashes.
- `@leetcode\\.com`: Matches the literal text `@leetcode.com`. The backslash before the period (`\\.`) is required because a plain `.` in regex normally means "any character" — escaping it forces it to match a literal period only.
- `$`: Anchors the match to the **end** of the string — nothing can come after `.com`.

### ✅ Why This Solution Works

Regular expressions excel at validating precise string structure rules like "starts with X, contains only Y characters, and ends with exact text Z." Anchoring the pattern with `^` and `$` ensures the *entire* email must conform to the rule from start to finish — without these anchors, the pattern could match just a substring anywhere inside a longer, invalid string, incorrectly passing malformed emails.

### 🧠 SQL Concepts Used

- ✔ REGEXP
- ✔ Anchors (^, $)
- ✔ Character Classes
- ✔ Escaped Special Characters

### 💡 Interview Tip

- This tests whether you're comfortable writing and reasoning about regular expressions inside SQL — a skill that goes beyond basic `LIKE` pattern matching and is highly valued for data-validation and cleaning tasks.
- **Common mistake:** forgetting to escape the period in `@leetcode.com`, which would technically also match invalid variations like `'@leetcodeXcom'` since an unescaped `.` matches *any* single character, not just a literal period.
- **Edge case:** forgetting the `^` and `$` anchors would allow the pattern to match anywhere *within* a larger string — for example, matching a domain that only *contains* `'@leetcode.com'` as a substring but has extra invalid characters before or after it.

### ⏱ Time Complexity

**O(n)** — regex evaluation must be applied to every row individually; no standard index can accelerate a general regex pattern match.

### 💾 Space Complexity

**O(1)** — no additional storage needed beyond the output rows.

### 🔄 Alternative Solution

```sql
-- Using a combination of LIKE and additional string checks (less precise, but avoids REGEXP)
SELECT *
FROM Users
WHERE mail LIKE '%@leetcode.com'
  AND LEFT(mail, 1) REGEXP '^[a-zA-Z]$'
  AND mail NOT LIKE '%[^a-zA-Z0-9_.-@]%'; -- Note: MySQL's LIKE doesn't support character-class negation like this;
                                          -- true validation of the "only allowed characters" rule generally requires REGEXP.
```

This illustrates why `LIKE` alone is insufficient for full validation — MySQL's `LIKE` operator doesn't support character classes or negated sets the way `REGEXP` does, so a truly robust "only these characters are allowed" check almost always requires `REGEXP` (or an application-layer validation step) rather than `LIKE`.

### 🎯 Key Takeaways

- `REGEXP` enables precise, rule-based string validation that `LIKE` alone cannot express.
- Always anchor patterns with `^` and `$` when the *entire* string must match a rule, not just a portion of it.
- Special regex characters like `.` must be escaped (`\\.`) when you intend to match them literally.

---

## 🧩 Quick Reference: Concepts by Question

| Concept | Questions |
|---|---|
| `SELECT` / `WHERE` basics | 1, 2, 3, 4, 5, 15, 45 |
| `LEFT JOIN` | 6, 8, 11, 12, 16, 34, 37 |
| `INNER JOIN` | 7, 17, 30 |
| Self JOIN | 9, 10, 13, 30, 33 |
| `GROUP BY` / `HAVING` | 13, 19, 20, 23, 26, 27, 28, 29, 36 |
| `CASE` expressions | 14, 19, 20, 32, 36, 38 |
| Subqueries | 13, 18, 21, 22, 25, 28, 29, 34, 37, 42, 47 |
| `UNION` / `UNION ALL` | 31, 36, 39, 41 |
| Window Functions | 21 (alt), 33 (alt), 35, 40, 43 |
| Date Functions | 9, 20, 22, 24, 34, 49 |
| String Functions | 5, 44, 45, 50 |
| `DELETE` | 46 |
| `LIMIT` / `OFFSET` | 35, 39, 47 |
| `GROUP_CONCAT` | 48 |
| `REGEXP` | 45 (alt), 50 |

---

## 🎓 Suggested Learning Path

If you're new to SQL, work through the questions roughly in this order for the smoothest learning curve:

1. **Fundamentals** — Questions 1–5 (SELECT, WHERE, DISTINCT, string basics)
2. **Joining Tables** — Questions 6–12 (LEFT JOIN, INNER JOIN, self-joins)
3. **Grouping & Aggregation** — Questions 13, 16–20, 23, 26–30 (GROUP BY, HAVING, AVG/SUM/COUNT)
4. **Subqueries** — Questions 18, 21, 22, 25, 28, 29, 34, 37, 42, 47
5. **CASE Logic** — Questions 14, 19, 20, 32, 36, 38
6. **Set Operations** — Questions 31, 36, 39, 41 (UNION / UNION ALL)
7. **Window Functions** — Questions 35, 40, 43 (the most advanced topic — save these for last)
8. **String & Regex** — Questions 44, 45, 50

---

## ❓ Frequently Asked Questions

**Q: Do I need to memorize every query?**
No. Focus on recognizing the *pattern* behind each question (e.g., "anti-join," "running total," "top-N per group") — patterns transfer to new problems, memorized queries don't.

**Q: Why MySQL specifically?**
MySQL is one of the most widely used databases in industry and is the standard dialect for the original question set this repository is based on. Most concepts here (joins, `GROUP BY`, window functions) transfer directly to PostgreSQL, SQL Server, and other databases, though some functions (like `GROUP_CONCAT`, `IFNULL`) have different names elsewhere (`STRING_AGG`, `COALESCE`, etc.).

**Q: What MySQL version do I need?**
Window functions (`ROW_NUMBER()`, `RANK()`, `DENSE_RANK()`, `LAG()`, `LEAD()`, `SUM() OVER()`) require **MySQL 8.0+**. Every question that uses them also includes a pre-8.0-compatible alternative solution.

**Q: How should I practice these?**
Try to solve each problem yourself first — using only the "Problem" section — before looking at the solution. Then compare your approach to the one provided and read the "Why This Solution Works" section to understand any gaps in your reasoning.

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve an explanation, add an alternative solution, or fix an error:

1. Fork this repository
2. Create a new branch (`git checkout -b improve-question-14`)
3. Make your changes, following the existing structure for each question
4. Submit a pull request with a clear description of your change

Please keep explanations beginner-friendly and avoid copying problem text directly from any external source — all explanations should be written in original language.

---

## 📄 License

This repository is provided under the [MIT License](https://opensource.org/licenses/MIT). Feel free to use, share, and adapt this content for personal study, teaching, or interview preparation.

---

## ⭐ Final Note

SQL interviews reward **pattern recognition**, not memorization. Every question in this handbook maps to a small number of reusable techniques — anti-joins, running totals, per-group ranking, conditional aggregation, and so on. Once you can spot which pattern a question is really testing, even unfamiliar problems become approachable.

Good luck with your interviews! 🚀
