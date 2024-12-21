# DataQuery-Hub

## Objective
The DataQuery-Hub project focuses on creating a relational database and simulating real-world data scenarios. It aims to enhance SQL skills by practicing data retrieval, filtering, joining tables, and performing calculations. The project provides hands-on experience in database management and query optimization, preparing participants for real-world data challenges.

## Skills Learned

- Basic SQL: Data retrieval, filtering, sorting, and simple aggregations.
- Filters: Using conditions (AND, OR, NOT, BETWEEN, LIKE).
- Joins: Combining data with INNER JOIN, LEFT JOIN, and more.
- Aggregate Functions: Calculating averages, sums, and counts.
- Problem-Solving: Translating data problems into efficient SQL queries.

## Tools Used

- SQL Database Management System (e.g., MySQL)
- Query editors like MySQL Workbench for database interactions.
- Sample datasets for testing queries and validating results.

## Steps
#### Project Details

#### Tables

Create two tables for this project:

1. **employees**
2. **machines**

#### Schema and Entries

##### employees Table Schema
- **employee_id** (INT, PRIMARY KEY)
- **firstname** (VARCHAR)
- **lastname** (VARCHAR)
- **department** (VARCHAR)
- **hiredate** (DATE)
- **salary** (DECIMAL)
- **device_id** (INT)


**Sample Data for employees:**
| employee_id | firstname | lastname | department | hiredate    | salary   | device_id |
|-------------|-----------|----------|------------|-------------|----------|-----------|
| 1           | John      | Doe      | HR         | 2020-02-01  | 50000.00 | 101       |
| 2           | Jane      | Smith    | IT         | 2021-05-15  | 60000.00 | 102       |
| 3           | Mike      | Brown    | Finance    | 2019-08-20  | 45000.00 | NULL      |
| 4           | Sarah     | Johnson  | Marketing  | 2022-11-30  | 55000.00 | 103       |
| 5           | Alice     | Davis    | IT         | 2020-01-25  | 75000.00 | 102       |
| 6           | Bob       | Wilson   | Finance    | 2021-10-12  | 47000.00 | 104       |
| 7           | Karen     | Miller   | Marketing  | 2020-04-22  | 48000.00 | NULL      |
| 8           | Paul      | Martinez | IT         | 2022-06-10  | 67000.00 | 105       |
| 9           | David     | Lopez    | HR         | 2023-01-15  | 52000.00 | NULL      |
| 10          | Anna      | Taylor   | Finance    | 2018-03-30  | 43000.00 | 106       |
| 11          | Ryan      | White    | IT         | 2022-12-05  | 80000.00 | 102       |
| 12          | Emily     | Thomas   | Marketing  | 2020-08-18  | 57000.00 | 103       |
| 13          | Olivia    | Moore    | HR         | 2021-07-23  | 54000.00 | NULL      |
| 14          | Ethan     | Harris   | IT         | 2022-03-11  | 68000.00 | 107       |
| 15          | Sophia    | Clark    | Finance    | 2020-10-05  | 46000.00 | NULL      |

##### machines Table Schema
- **device_id** (INT, PRIMARY KEY)
- **machine_name** (VARCHAR)
- **status** (VARCHAR)

**Sample Data for machines:**
| device_id | machine_name | status   |
|-----------|--------------|----------|
| 101       | Printer      | Active   |
| 102       | Laptop       | Inactive |
| 103       | Desktop      | Active   |
| 104       | Scanner      | Active   |
| 105       | Router       | Inactive |
| 106       | Switch       | Active   |
| 107       | Firewall     | Active   |
| 108       | Projector    | Active   |
| 109       | NAS          | Inactive |
| 110       | Smartboard   | Active   |
| 111       | Tablet       | Inactive |
| 112       | Smartphone   | Active   |
| 113       | Server       | Active   |
| 114       | Modem        | Inactive |
| 115       | Webcam       | Active   |

---

#### SQL Questions and Instructions

#### Basic-Level Questions

1. **Querying Data:** Write an SQL query to retrieve all columns from the `employees` table sorted in ascending order by the `hiredate`. <br/> <img src="https://github.com/user-attachments/assets/c78333b5-9cbd-4870-9823-b74011667131" /> <img src="https://github.com/user-attachments/assets/49b2ba31-7890-4407-aa98-e7c7423282fa" />
2. **Simple Filter:** Write an SQL query to find all employees in the `employees` table whose `department` is "Finance".<br/> <img src="https://github.com/user-attachments/assets/bffb2632-64a6-4f20-9090-ad535123d0cb" /> <img src="https://github.com/user-attachments/assets/4fca1ef9-ea08-44e7-a75a-6c20a545558a" />
3. **Wildcard Search:** Write an SQL query to find all employees whose `firstname` starts with the letter "J".<br/> <img src="https://github.com/user-attachments/assets/cef28224-b572-4186-a2ef-76802e7e3125" /> <img src="https://github.com/user-attachments/assets/ba9abf89-168a-4ca9-bdbe-696785d4cfc2" />
4. **Sorting by Multiple Columns:** Write an SQL query to retrieve all records from the `employees` table, sorted first by `department` and then by `lastname` in ascending order.<br/> <img src="https://github.com/user-attachments/assets/ab982e01-f2a0-48de-892b-e6395d10b958"/> <img src="https://github.com/user-attachments/assets/dab87655-9cc9-4d7a-8781-fb5881ec3922"/>
5. **Counting Records:** Write an SQL query to count the number of employees in the `employees` table. <br/> <img src="https://github.com/user-attachments/assets/54cf98b2-2acd-41d3-a52d-e56a58c17aa7"/> <img src="https://github.com/user-attachments/assets/ff420a55-1584-4231-b989-c8755127aa08"/>


### Intermediate-Level Questions

1. **Range Filtering:** Write an SQL query to find all employees whose `salary` is between 40,000 and 60,000. <br/> <img src="https://github.com/user-attachments/assets/2f8d13cb-88dc-4045-98bd-e9ca4e83640b" /> <img src="https://github.com/user-attachments/assets/16481d1e-a85a-4880-afb4-775b45c6195d" />
2. 2. **Joining Tables:** Perform a LEFT JOIN between the `employees` and `machines` tables on the `device_id` column. Display all columns from both tables. <br/> <img src="https://github.com/user-attachments/assets/70185424-38a6-4071-a398-115fe69e70b0" /> <img src="https://github.com/user-attachments/assets/d56f99cd-bcf6-45bd-b4ca-780a6a90db51" />
3. **Aggregate Function:** Write an SQL query to calculate the average salary of employees in the `employees` table. <br/> <img src="https://github.com/user-attachments/assets/30ff835f-3f49-4faa-badc-fd9b6c5d6661" /> <img src="https://github.com/user-attachments/assets/794b1b58-f7e1-4023-b630-a18774e1e33b" />
4. **Compound Conditions:** Write an SQL query to find all employees in the `IT` department who were hired after `2021-01-01`. <br/> <img src="https://github.com/user-attachments/assets/5c71086d-88e9-4b82-a1ee-5d07964f0b4f" /> <img src="https://github.com/user-attachments/assets/26a00438-3983-444a-9431-e9d83bbe0042" />
5. **Pattern Matching:** Write an SQL query to find all employees whose `lastname` contains the substring "son" anywhere in the name. <br/> <img src="https://github.com/user-attachments/assets/1fe220dc-2be2-4d6f-8451-bd8e4f779262" /> <img src="https://github.com/user-attachments/assets/f0fd6385-5fcd-417d-be11-5dc6a00f5c09" />

## Conclusion 

This project helps enhance SQL skills through practical queries on employees and machines tables. It covers key concepts like data retrieval, filtering, sorting, joins, aggregations, and pattern matching. By solving real-world data challenges, participants gain hands-on experience in database management, preparing them for advanced data tasks. This project effectively combines theory with practice, making it a valuable tool for developing essential SQL skills for data-related roles.

