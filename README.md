Data Analysis, Data Science, Machine Learning

Data Analysis, Data Science, Machine Learning
General videos
General books
Data Analysis
Data Analysis general (how to learn, advices etc.)
Data Analysis courses
Alex The Analyst (playlist) - Data Analyst Bootcamp - course + my notes
Data Analysis projects
Data Analysis books
Data Analysts - what do they do?
Data Science
Data Science general (roadmaps, how to learn, advices etc.)
Data Science courses
Data Science projects
Data Science mathematics
Data Science books
Data Scientists - what do they do?
Machine Learning
Machine learning general (how to learn, advices etc.)
Machine learning projects
Diffusion models
Machine Learning basics
Machine learning courses
Premium (Udemy, Coursera etc.)
Free
Machine learning books
Deep Learning
Tutorials
Artificial intelligence
Artificial intelligence general (how to learn, advices etc.)
Tutorials
Fine-tuning
Fine-tuning projects
Mathematics for AI
Artificial intelligence articles
Artificial intelligence books
Mathematics courses (with my notes)
Databases
Interactive SQL tutorials
Platforms for learning
Talks
Interviews
YouTube channels
Other links and playlists
Interesting videos involving AI
General videos
 IBM Technology - AI, Machine Learning, Deep Learning and Generative AI Explained
General books
 Engineering with Utsav - Books Every Software Engineer Should Read in 2025
 PythonProgrammer - I've read 57 Books on AI and Data Science - these are the best (for 2025)
Data Analysis
Data Analysis general (how to learn, advices etc.)
 Alex The Analyst - How I Would Become a Data Analyst if I had to Start Over in 2024 | 6 Month Plan
Learn: SQL, Excel, Tableau
Projects:
2 SQL projects,
1 Excel project,
1-2 Tableau project
BUT create something in connection with the field you want to work in (e.g., healthcare, finance, marketing etc.)
Make a good resume
Apply for jobs, but not directly - work with multiple recruiters
Be good at an interview :) (research a company, the position and questions they might ask you)
If you have more time, learn some cloud tools (e.g., AWS, GCP, Azure) and Python
 Alex The Analyst - How to Become a Data Analyst in 2023 (Completely FREE!)
 Agatha - How I'd Become a Data Analyst (if i had to start over) in 2024
 Agatha - I analyzed data for 4 hours everyday and it changed my life
 Stefanovic - FASTEST Way to Become a Data Analyst and ACTUALLY Get a Job
 Luke Barousse - How I'd Learn to be a Data Analyst in 2024
 Luke Barousse - How I Would Learn to be a Data Analyst (2 years ago)
 Luke Barousse - Top Courses to Become a Data Analyst
 Josh Brindley - FASTEST Way to become a Data Analyst and ACTUALLY get a job [2023]
 Learn with Lucas - Data Analyst Roadmap - FASTEST Way To a Data Analyst Job
Data Analysis courses
 Shashank Kalanithi - Day in the Life of a Data Analyst (playlist)

 Data Analyst - Python PCA Application w/ Streamlit (29K views, 2 years ago, 1:11:54)
 Day in the Life of a Data Analyst - SurveyMonkey Data Transformation (3M views, 2 years ago, 1:17:14)
 Day in the Life of a Data Analyst - Bing Maps API (20K views, 2 years ago, 29:00)
 Day in the Life of a Data Analyst - SurveyMonkey Data Transformation (Using R) (18K views, 2 years ago, 41:55)
 Data Analyst - PyCaret to Enhance Your Machine Learning (4K views, 2 years ago, 31:04)
 Day in the Life of a Data Analyst - Google Data Studio (28K views, 2 years ago, 31:33)
 Making Money (as a data analyst) - Webscraping with ScraperAPI (20K views, 2 years ago, 57:13)
 Data Cleaning CHALLENGE (can you think of a better solution?) (131K views, 2 years ago, 22:41)
Shashank Kalanithi - A Data Crash Course | 100+ Key Data Concepts

Alex The Analyst (playlist) - Data Analyst Bootcamp - course + my notes
Link to a course on YouTube

 1. FREE Data Analyst Bootcamp!! (497K views, 6 months ago, 6:52)

 2. How to Become a Data Analyst in 2023 (Completely FREE!) (638K views, 7 months ago, 13:59)

 3. SQL Basics Tutorial For Beginners | Installing SQL Server Management Studio and Create Tables | 1/4 (893K views, 3 years ago, 9:37)

 4. SQL Basics Tutorial For Beginners | Select + From Statements | 2/4 (299K views, 3 years ago, 6:14)

<> is the not equal operator.

My comment: SELECT is a projection operation. It selects the columns that we want to see in the result.

 5. SQL Basics Tutorial For Beginners | Where Statement | 3/4 (204K views, 3 years ago, 7:58)

 6. SQL Basics Tutorial For Beginners | Group By + Order By Statements | 4/4 (194K views, 3 years ago, 8:09)

COUNT() is not a (regular) column (from a table). It's a derived column/field (and an aggregate function BTW). That's why we don't need to include it in the GROUP BY clause.

ORDER BY can be used not just on one column, but on multiple columns as well. In that case, the order of columns in the ORDER BY clause matters.

 7. Intermediate SQL Tutorial | Inner/Outer Joins | Use Cases (315K views, 3 years ago, 15:53)

For inner join, it's not important which ID column we use in the SELECT clause, because they are the same. But for outer join, it's important to use the ID column from the table that we want to keep all the rows from.

Left join keeps all the rows from the left table, and right join keeps all the rows from the right table.

My comment (about the syntax of JOIN; BTW the word "INNER" is optional):

SELECT * FROM EmployeeDemographics ed
INNER JOIN EmployeeSalary es
ON ed.EmployeeID = es.EmployeeID
is the same as:

SELECT * FROM EmployeeDemographics
INNER JOIN EmployeeSalary
ON EmployeeDemographics.EmployeeID = EmployeeSalary.EmployeeID
My comment (about for example LEFT (OUTER) JOIN):

SELECT *
FROM EmployeeDemographics
LEFT OUTER JOIN EmployeeSalary ON EmployeeDemographics.EmployeeID = EmployeeSalary.EmployeeID
This takes everything from the "left" table (EmployeeDemographics) and matches it with the "right" table (EmployeeSalary). If there is no match, it will still take the row from the "left" table, but it will fill the columns from the "right" table with NULLs.

My comment (about emulating FULL OUTER JOIN in MySQL)

SELECT *
FROM EmployeeDemographics
LEFT JOIN EmployeeSalary ON EmployeeDemographics.EmployeeID = EmployeeSalary.EmployeeID

UNION

SELECT *
FROM EmployeeDemographics
RIGHT JOIN EmployeeSalary ON EmployeeDemographics.EmployeeID = EmployeeSalary.EmployeeID;
 8. Intermediate SQL Tutorial | Unions | Union Operator (156K views, 3 years ago, 5:25)

Check out the previous example for FULL OUTER JOIN emulation in MySQL.

JOIN combines both tables based on common column(s) (in our last video that column was the EmployeeID which we had in both tables), while UNION combines both tables based on common rows.

My comments:

JOIN combines both tables horizontally, while UNION combines both tables vertically. In other words, JOIN puts both tables side by side, while UNION puts both tables on top of each other (below each other).
Also, UNION removes the duplicates, while UNION ALL keeps the duplicates.
My comment (about UNION and UNION ALL):

SELECT *
FROM EmployeeDemographics
UNION
SELECT *
FROM EmployeeSalary;

SELECT *
FROM EmployeeDemographics
UNION ALL
SELECT *
FROM EmployeeSalary;
The first query will return 5 rows, while the second query will return 6 rows (because there is one duplicate row in the EmployeeSalary table).

My comment (about the example in the previous video, about FULL JOIN done using UNION):

Even though it looks as though the results is horizontal, it's actually vertical. How? The first query returns 5 rows, while the second query returns 4 rows. So the result of the UNION is 9 rows (4 rows are placed below first 5 rows and then), which is the same as the result of the FULL JOIN.

My comment (about selecting columns in UNION):

SELECT EmployeeID, FirstName, Age
FROM EmployeeDemographics
UNION
SELECT EmployeeID, JobTitle, Salary
FROM EmployeeSalary
If we select columns like this, we will not get the desired result. Why? Because the columns in the first query are different than the columns in the second query. So we need to select the same number of columns in both queries, and the columns need to be of the same type (or at least compatible types).

 9. Intermediate SQL Tutorial | Case Statement | Use Cases (185K views, 3 years ago, 7:26)

Case statement allows us to specify a condition and then also specify what we want returned (a result) if that condition is met. (Case statement allows us to create a new column based on the values of other columns.)

We can put multiple WHEN statements in the CASE statement. Example:

SELECT FirstName, LastName, Age,
CASE
WHEN Age < 18 THEN 'Minor'
WHEN Age >= 18 AND Age <= 65 THEN 'Adult'
ELSE 'Senior'
END AS 'AgeGroup'
FROM EmployeeDemographics;
Something to note is that the CASE statement is evaluated in order. So if the first WHEN statement is true, then it will return that result and not check the other WHEN statements.

My comment:

So if we have multiple WHEN statements, we need to make sure that the most specific WHEN statement is first, and the most general WHEN statement is last. Example:

SELECT FirstName, LastName, Age,
CASE
	WHEN Age > 30 THEN 'Old'
	WHEN Age = 38 THEN 'Stanley' # Previous WHEN statement is true, so this one is not checked. So this one is never true.
	ELSE 'Baby'                  # Solution: change the order of WHEN statements.
END
FROM EmployeeDemographics
WHERE Age is NOT NULL
ORDER BY Age
Another example (about using CASE statement with JOIN):

SELECT *,
CASE
	WHEN JobTitle = 'Salesman' THEN Salary + (Salary * .10)
	WHEN JobTitle = 'Accountant' THEN Salary + (Salary * .05)
	WHEN JobTitle = 'HR' THEN Salary + (Salary * .000001)
END AS 'Salary after raise'
FROM EmployeeDemographics ed
JOIN EmployeeSalary es
ON ed.EmployeeID = es.EmployeeID
 10. Intermediate SQL Tutorial | Having Clause (102K views, 3 years ago, 3:31)

The HAVING clause is used to filter the results of an aggregate function. Example:

SELECT JobTitle, COUNT(JobTitle)
FROM EmployeeDemographics ed
JOIN EmployeeSalary es
ON ed.EmployeeID = es.EmployeeID
GROUP BY JobTitle
HAVING COUNT(JobTitle) > 1 # This cannot be placed above GROUP BY.
                           # It has to be placed below GROUP BY because it's an aggregate function.
The SQL query components need to be in a specific order due to the way SQL engines parse and execute queries. The SQL standard defines a particular sequence in which the clauses should appear in a SELECT statement. Here is the typical order:

Why does HAVING clause have to go below GROUP BY clause?

The SQL query components need to be in a specific order due to the way SQL engines parse and execute queries. The SQL standard defines a particular sequence in which the clauses should appear in a SELECT statement. Here is the typical order:

1. SELECT
2. FROM
3. JOIN
4. WHERE
5. GROUP BY
6. HAVING
7. ORDER BY
Here's why each step comes where it does:

1. SELECT: Specifies the columns you want.
2. FROM: Specifies the tables from which to select or delete or the tables to update.
3. JOIN: Combines rows from two or more tables based on a related column between them.
4. WHERE: Filters records before any groupings are made.
5. GROUP BY: Groups records after the WHERE clause has been applied. The grouping is done on the basis of columns. Aggregate functions (like COUNT, AVG, MAX, etc.) then operate on these groups.
6. HAVING: Filters records after the GROUP BY clause has been applied.
7. ORDER BY: Sorts the records, but does this last, after all filtering and grouping have been done.
My comment (a quick recap) of the difference between WHERE and HAVING:

WHERE filters records before any groupings are made.
HAVING filters records after the GROUP BY clause has been applied.
My comment about aggregate functions vs. GROUP BY:

Aggregate functions (e.g., COUNT, SUM, AVG, MIN, MAX): Perform calculations on a set of values and return a single value.
GROUP BY clause: Groups rows that have the same values in specified columns into summary rows.
 11. Intermediate SQL Tutorial | Updating/Deleting Data (86K views, 3 years ago, 4:37)

The difference between INSERT and UPDATE is that INSERT adds a new row to a table, while UPDATE modifies existing rows in a table.

Example:

UPDATE EmployeeDemographics
SET Age = 31, Gender = 'Female'
WHERE EmployeeID = 1012
Good practice, before DELETE, is to use SELECT to see what we are going to delete.

SELECT * FROM EmployeeDemographics
WHERE EmployeeID  = 1005
DELETE statement is used to delete rows from a table. Example:

DELETE FROM EmployeeDemographics
WHERE EmployeeID  = 1005
 12. Intermediate SQL Tutorial | Aliasing (85K views, 3 years ago, 6:12)

Useful hint for writing SQL statements:
When writing the SQL statement, first write the FROM clause with an alias. Then, when writing the SELECT statement, use the alias to refer to the table - which will give us a dropdown list of all the columns in that table.```
Now, continuing with the lecture...

Aliasing is used to give a table, or a column in a table, a temporary name.

My example:

SELECT ed.EmployeeID, ed.FirstName, ed.LastName, es.Salary
FROM EmployeeDemographics ed
JOIN EmployeeSalary es
ON ed.EmployeeID = es.EmployeeID
Another example:

SELECT FirstName AS fn
FROM EmployeeDemographics AS ed
is the same as:

SELECT FirstName fn
FROM EmployeeDemographics
Another example:

SELECT CONCAT(FirstName, ' ', LastName) AS 'Full Name'
FROM EmployeeDemographics
Another time we'll use aliasing in the SELECT statement is when we want to use an aggregate function. Example:

SELECT AVG(Age) AS 'Average Age'
FROM EmployeeDemographics
Untill now, we used aliasing for column names. But we can also use aliasing for table names. Example:

SELECT Demographics.EmployeeID
FROM EmployeeDemographics Demographics
 13. Intermediate SQL Tutorial | Partition By (163K views, 2 years ago, 4:14)

PARTITION BY statement is often compared to GROUP BY statement. But they are not the same. The GROUP BY statement is going to reduce the number of rows in our result set by actually "rolling them up" (by calculating the sum, or averages for each group), while the PARTITION BY statement is going to divide the result set into partitions (and change how the window function is calculated) without reducing the number of rows in our result set.

SELECT ed.FirstName, ed.LastName, ed.Gender, es.Salary, COUNT(Gender) OVER (PARTITION BY Gender) as TotalGender FROM EmployeeDemographics ed JOIN EmployeeSalary es ON ed.EmployeeID = es.EmployeeID

What is a "window function"? A window function is a function that can be applied to a partition of rows. It is also called an "analytic function". Another way to think about it is that a window function is a function that can be applied to a group of rows that are related to the current row.

ChatGPT's answer:

A window function in SQL allows you to perform calculations across a set of table rows that are related to the current row, almost like a sliding "window" over the data. This is analogous to the way a window in a GUI application displays a subportion of the overall data. What makes window functions unique is that they provide access to more than just the current row of the query result.

Unlike aggregate functions, which return a single result value based on a group of rows, window functions return a single value for each row from the underlying query result based on a window of rows related to that row.

Key components of window functions:

1. OVER() Clause: This defines the window of rows for the function to operate on. You can specify ordering and partitioning within this clause.
2. PARTITION BY: This divides the result set into partitions to which the window function is applied. For instance, if you want to operate on groups of rows having the same value in a certain column (e.g., date or category), you'd use PARTITION BY.
3. ORDER BY: Within the OVER() clause, this determines the order in which rows will be processed by the window function.
4. ROWS/RANGE: Specifies which rows are included in the frame. The frame is a subset of the current partition and is used for calculation in functions like running totals.

Examples of window functions:

- Ranking functions: ROW_NUMBER(), RANK(), DENSE_RANK(), NTILE().
- Analytic functions: LEAD(), LAG(), FIRST_VALUE(), LAST_VALUE().
- Aggregate functions: SUM(), AVG(), MIN(), MAX(). These can be used as window functions when combined with the OVER() clause.

Using our earlier example, COUNT(Gender) OVER (PARTITION BY Gender) is a window function. For each row in the dataset, it counts the number of rows with the same Gender value.

In essence, window functions let you perform calculations that require considering a range or "window" of rows relative to the current row, without collapsing all those rows into a single output row.
Aditional explanation Colt Steele - SQL Window Functions in 10 Minutes

Several things to note:

Window functions perform aggregate operations on group of rows but they produce a result FOR EACH ROW. So we have individual row data alongside aggregated data.
The OVER() clause constructs a window. When it's empty, the window will include all records.
Use ORDER BY inside of the OVER() clause to re-order rows within each window.
The PARTITION BY clause divides the window into smaller sets or partitions. The window function is applied to each partition separately and computation restarts for each partition. (Copilot suggestion)
 14. Advanced SQL Tutorial | CTE (Common Table Expression) (214K views, 2 years ago, 3:44)

CTE is a common table expression and it's a named temporary result set which is used to manipulate (Copilot suggestion: the data in the result set further) the complex sub-queries data. This only exists within the scope of the statement that we're about to write. Once we cancel out of this query it's like it never existed. A CTE is also only created in memory rather than a tempdb file like a temp table would be, but in general a CTE acts very much like a subquery and so if we know how to write subqueries we can easily learn how to write CTEs.

CTEs are sometimes called "WITH" queries because we use the WITH keyword to create them. The syntax is as follows:

WITH CTE_Employee as
(SELECT ed.FirstName, ed.LastName, ed.Gender, es.Salary,
COUNT(Gender) OVER (PARTITION BY Gender) as TotalGender,
AVG(Salary) OVER (PARTITION BY Gender) AS AvgSalary
FROM EmployeeDemographics ed
JOIN EmployeeSalary es
ON ed.EmployeeID = es.EmployeeID
WHERE Salary > '45000')

SELECT *
FROM CTE_Employee
Explanation suggested by the Copilot: CTE is a temporary result set that we can reference within another SQL statement. It's similar to a subquery, but it's more readable and easier to maintain.

Example:

WITH EmployeeCTE AS (
	SELECT *
	FROM EmployeeDemographics
	WHERE Age > 30
)

SELECT *
FROM EmployeeCTE
Aditional explanation (check out LearnatKnowstar - SQL | Subquery or CTE - Which one to choose? Difference between Subquery and CTE):

Excerpt:
CTEs are named queries (suggested by Copilot: temporary result sets) that you can reference (multiple times if needed) within another SQL statement. They are similar to subqueries, but they are more readable and easier to maintain. They are also more flexible than subqueries. For example, you can reference a CTE multiple times in the same SELECT statement, while you can only reference a subquery once. In terms of performance and in terms of how the logic is executed, they are similar to subqueries (no difference as far as I can see at the moment).

There are scenarios where we we can use only a CTE or only a subquery:

CTE can be recursive, while subquery cannot be recursive:
Recursive CTEs can reference themselves in a query. (Suggested by Copilot: This is useful for querying hierarchical data (like a tree structure) or data that has a parent-child relationship.)
Corelated subqueries can reference outer table from the subquery, while CTE cannot reference outer table from the CTE.
Suggested by Copilot: there are also scenarios where we can use both. In those cases, we should use a CTE because it's more readable and easier to maintain.

 15. Advanced SQL Tutorial | Temp Tables (158K views, 2 years ago, 10:19)

Suggested by Copilot: Temp tables are like regular tables, but they are only available to the current session. They are also stored in tempdb, which is a system database. Temp tables are automatically deleted when the session that created them is closed.

We can hit off of this temp table multiple times which we cannot do with something like CTE or subquery, where we can only use it one time or with the subquery where we need to write it multiple times within the query. (TODO: check this)
Example:

CREATE TEMPORARY TABLE temp_Employee (
EmployeeID int,
JobTitle varchar(100),
Salary int
)

SELECT *
FROM temp_Employee
Maybe the best way to work with temp tables is to take a subset of data from a (much) larger table, put it into a temp table, and then work with that temp table.
Example:

INSERT INTO temp_Employee
SELECT *
FROM EmployeeSalary AS es
WHERE es.Salary > '40000'
Realistic example: We have a table with 100 million rows. We want to do some analysis on that table, but we don't want to do it on the entire table. So we can create a temp table with a subset of data from that table, and then do the analysis on that temp table. (Suggested by Copilot)

CREATE TEMPORARY TABLE temp_Employee2
SELECT JobTitle, Count(JobTitle), Avg(Age), Avg(Salary)
FROM EmployeeDemographics AS ed
JOIN EmployeeSalary AS es
ON ed.EmployeeID = es.EmployeeID
GROUP BY JobTitle
Useful for later: A lot of times these temp tables are used in stored procedures. (we'll need to remove the temp table before we can create it again)
Example:

DROP TABLE IF EXISTS temp_Employee
CREATE TEMPORARY TABLE temp_Employee (
...
)

INSERT INTO temp_Employee
SELECT *
FROM ...

SELECT *
FROM temp_Employee
 16. Advanced SQL Tutorial | String Functions + Use Cases (105K views, 2 years ago, 13:49)

 17. Advanced SQL Tutorial | Stored Procedures + Use Cases (244K views, 2 years ago, 6:15)

 18. Advanced SQL Tutorial | Subqueries (233K views, 2 years ago, 8:37)

 19. Data Analyst Portfolio Project | SQL Data Exploration | Project 1/4 (1.3M views, 2 years ago, 1:17:09)

 20. Data Analyst Portfolio Project | Data Cleaning in SQL | Project 3/4 (281K views, 2 years ago, 54:44)

 21. Pivot Tables in Excel | Excel Tutorials for Beginners (333K views, 1 year ago, 17:35)

 22. Formulas in Excel | Excel Tutorials for Beginners (160K views, 1 year ago, 33:54)

 23. XLOOKUP in Excel | Excel Tutorials for Beginners (98K views, 1 year ago, 18:47)

 24. Conditional Formatting in Excel | Excel Tutorials for Beginners (81K views, 1 year ago, 20:59)

 25. Charts in Excel | Excel Tutorials for Beginners (60K views, 1 year ago, 15:11)

 26. Cleaning Data in Excel | Excel Tutorials for Beginners (280K views, 1 year ago, 21:04)

 27. Full Project in Excel | Excel Tutorials for Beginners (417K views, 1 year ago, 40:50)

 28. How to Install Tableau and Create First Visualization | Tableau Tutorials for Beginners (402K views, 1 year ago, 17:04)

 29. How to use Calculated Fields and Bins in Tableau | Tableau Tutorials for Beginners (118K views, 1 year ago, 6:25)

 30. How to Create Visualizations in Tableau | Tableau Tutorials for Beginners (95K views, 1 year ago, 14:05)

 31. How to use Joins in Tableau | Tableau Tutorials for Beginners (69K views, 1 year ago, 14:29)

 32. Full Beginner Project in Tableau | Tableau Tutorials for Beginners (154K views, 1 year ago, 44:18)

 33. How to Install Power BI | Building First Visualization | Microsoft Power BI for Beginners (155K views, 1 year ago, 12:50)

 34. How to use Power Query in Power BI | Microsoft Power BI for Beginners (107K views, 1 year ago, 13:07)

 35. How to Create and Manage Relationships in Power BI | Microsoft Power BI for Beginners (74K views, 1 year ago, 8:36)

 36. How to use DAX in Power BI | Microsoft Power BI for Beginners (62K views, 1 year ago, 15:44)

 37. How to use Drill Down in Power BI | Microsoft Power BI for Beginners (61K views, 1 year ago, 6:02)

 38. How to use Conditional Formatting in Power BI | Microsoft Power BI for Beginners (49K views, 1 year ago, 9:53)

 39. How to use Bins and Lists in Power BI | Microsoft Power BI for Beginners (32K views, 11 months ago, 9:31)

 40. Popular Visualizations in Power BI | Microsoft Power BI for Beginners (35K views, 11 months ago, 14:14)

 41. Full Power BI Guided Project | Microsoft Power BI for Beginners (186K views, 11 months ago, 42:37)

 42. Installing Jupyter Notebooks/Anaconda | Python for Beginners (105K views, 10 months ago, 10:03)

 43. Variables in Python | Python for Beginners (36K views, 10 months ago, 13:17)

 44. Data Types in Python | Python for Beginners (33K views, 9 months ago, 21:58)

 45. Comparison, Logical, and Membership Operators in Python | Python for Beginners (17K views, 9 months ago, 7:15)

 46. If Else Statements in Python | Python for Beginners (16K views, 9 months ago, 6:40)

 47. For Loops in Python | Python for Beginners (18K views, 9 months ago, 9:17)

 48. While Loops in Python | Python for Beginners (15K views, 9 months ago, 5:40)

 49. Functions in Python | Python for Beginners (18K views, 8 months ago, 12:44)

 50. Converting Data Types in Python | Python for Beginners (15K views, 8 months ago, 6:36)

 51. Building a BMI Calculator with Python | Python Projects for Beginners (29K views, 7 months ago, 14:23)

 52. Building an Automated File Sorter in File Explorer using Python | Python Projects for Beginners (22K views, 6 months ago, 16:51)

 53. Inspecting Web Pages with HTML | Web Scraping in Python (13K views, 2 months ago, 5:55)

 54. BeautifulSoup + Requests | Web Scraping in Python (14K views, 2 months ago, 6:58)

 55. Find and Find_All | Web Scraping in Python (9K views, 1 month ago, 12:10)

 56. Scraping Data from a Real Website | Web Scraping in Python (42K views, 1 month ago, 25:23)

 57. Reading in Files in Pandas | Python Pandas Tutorials (31K views, 6 months ago, 19:17)

 58. Filtering Columns and Rows in Pandas | Python Pandas Tutorials (20K views, 5 months ago, 11:49)

 59. Indexes in Pandas | Python Pandas Tutorials (13K views, 5 months ago, 11:22)

 60. Group By and Aggregate Functions in Pandas | Python Pandas Tutorials (14K views, 4 months ago, 11:05)

 61. Merging DataFrames in Pandas | Python Pandas Tutorials (18K views, 3 months ago, 22:09)

 62. Creating Visualizations using Pandas Library | Python Pandas Tutorials (18K views, 3 months ago, 16:50)

 63. Data Cleaning in Pandas | Python Pandas Tutorials (49K views, 3 months ago, 38:37)

 64. Exploratory Data Analysis in Pandas | Python Pandas Tutorials (28K views, 2 months ago, 32:13)

 65. Amazon Web Scraping Using Python | Data Analyst Portfolio Project (177K views, 2 years ago, 47:14)

 66. Automating Crypto Website API Pull Using Python | Data Analyst Project (35K views, 1 year ago, 51:14)

 67. How to Create a Portfolio Website for FREE (322K views, 2 years ago, 35:29)

 68. Create the Perfect Data Analyst Resume | Free Templates! (78K views, 5 months ago, 17:37)

 69. Top 3 Tips on Using LinkedIn to Land a Job (198K views, 2 years ago, 6:50)

 70. How To Download Your Data Analyst Bootcamp Certification (Congrats!!) (25K views, 7 months ago, 1:41)

Data Analysis projects
 Learn with Lucas - Data Analyst Portfolios Are Dead??
 Learn with Lucas - Top 5 Data Analyst Portfolios
 Learn with Lucas - The ONLY Data Analytics Portfolio You Need (GUARANTEED Job)
 Mér Winter - Data Analyst Portfolio Projects for 2024 | 3 projects to include in your resume
 Tech With Tim - Data Collection Project Ideas & Demos
Data Analysis books
Python for Data Analysis: Data Wrangling with pandas, NumPy, and Jupyter - Wes McKinney (2022, 3rd edition, 579 pages, O'Reilly Media, 5.4 stars from 241 ratings on Amazon)
Data Analysts - what do they do?
Agatha - What I actually do as a Data Analyst | salary, job, harsh reality
Data Science
Data Science general (roadmaps, how to learn, advices etc.)
Gregg Hogg - Data Science Has Changed - Here's What to Do
Sundas Khalid - How to Become a Data Scientist in 2024? (complete roadmap)
Tani Tech - HOW To BECOME A DATA SCIENTIST In 2024
Power Couple - FASTEST Way to Learn Data Science and ACTUALLY Get a Job
Thu Vu data analytics - 👩🏻‍💻 How to learn Data Science FASTER
DataNash - How I'd Learn Data Science In 2023 (If I Could Restart) | A Beginner's Roadmap
DataNash - How I'd Learn Data Science In 2024 (If I Could Restart) - The Ultimate Roadmap
Data Appreciation Society - How To Get a Job in MACHINE LEARNING without a DEGREE | 7 Best Tips (the following URL's are mostly generated using the Copilot, but comments are added by me based on the info from this video)
Learn Data Exploration (data preprocessing, data cleaning, data visualization)
Article on data pre-processing/data exploration
Another article explaining why it is so important to know for data scientists and machine learning engineers
Learn Pandas, SciKit-Learn, NumPy (also Matplotlib, Seaborn)
Pandas
SciKit-Learn
NumPy
Matplotlib
Seaborn
DataCamp - Pandas Cheat Sheet
DataCamp - NumPy Cheat Sheet
DataCamp - Matplotlib Cheat Sheet
DataCamp - Seaborn Cheat Sheet
DataCamp - SciKit-Learn Cheat Sheet
DataCamp - SciPy Cheat Sheet
SQL ("you only need basic SQL" hmmm)
DataCamp - SQL Cheat Sheet
DataCamp - SQL Tutorial
DataCamp - SQL Tutorial: How To Write Better Queries
Recommended in video - W3School
Start with startups
AngelList
Crunchbase
LinkedIn
Glassdoor
Indeed
Hired
Triplebyte
DataJobs
Data Science Jobs
Data Science Central
Data Elixir
Data Science Weekly
Data Science Report
Data Science 101
Data Science Central
Data Science Central - Jobs
Look for a mentor
Data Science Mentors
Follow on LinkedIn: Kate Strachnyi, Cassie Kozyrkov, Andrew Ng, Jason Brownlee, Elena Tej Grewal, Vin Vashishta, Kevin Gray
Personal projects
DataCamp - 5 Data Science Projects That Will Get You Hired in 2021
Data Science courses
Udemy - Jose Portilla - Python for Data Science and Machine Learning Bootcamp (Rating: 4.6 out of 5 (133,378 ratings) 654,156 students, 25h, Last updated 5/2022)
freeCodeCamp - Santiago Basulto from RMOTR - Data Analysis with Python - Full Course for Beginners (Numpy, Pandas, Matplotlib, Seaborn)
freeCodeCamp - Learn Data Science Tutorial - Full Course for Beginners
freeCodeCamp (playlist) - Data Science
20 videos 651,868 views Last updated on 16 Apr 2023

 [In progress] Learn Data Science Tutorial - Full Course for Beginners (2.8M views, 4 years ago, ~6h)
 Statistics - A Full University Course on Data Science Basics (2.4M views, 4 years ago, ~8.2h)
 Python for Data Science - Course for Beginners (Learn Python, Pandas, NumPy, Matplotlib) (3.1M views, 3 years ago, ~12.2h)
 Data Analysis with Python Course - Numpy, Pandas, Data Visualization (2M views, 2 years ago, ~10h)
 [In progress] Data Analysis with Python - Full Course for Beginners (Numpy, Pandas, Matplotlib, Seaborn) (2.7M views, 3 years ago, ~4.5h)
 Build 12 Data Science Apps with Python and Streamlit - Full Course (1.1M views, 2 years ago, ~3.2h)
 Data Science Hands-On Crash Course (96K views, 2 years ago, ~2.5h)
 Data Visualization with D3.js - Full Tutorial Course (1.1M views, 4 years ago, ~13h)
 R Shiny for Data Science Tutorial – Build Interactive Data-Driven Web Apps (127K views, 1 year ago, ~1.5h)
 R Programming Tutorial - Learn the Basics of Statistical Computing (3.6M views, 4 years ago, ~2.2h)
 Python for Bioinformatics - Drug Discovery Using Machine Learning and Data Analysis (478K views, 2 years ago, ~2h)
 Intro to Data Science - Crash Course for Beginners (382K views, 4 years ago, ~2h)
 Applied Deep Learning with PyTorch - Full Course (151K views, 4 years ago, ~6h)
 Tableau for Data Science and Data Visualization - Crash Course Tutorial (769K views, 4 years ago, ~0.5h)
 jamovi for Data Analysis - Full Tutorial (119K views, 3 years ago, ~5h)
 Data Analysis with Python: Part 1 of 6 (Live Course) (526K views, Streamed 2 years ago, ~1.1h)
 [In progress] Data Analytics Crash Course: Teach Yourself in 30 Days (237K views, 2 years ago, ~0.9h)
 Data Analysis with Python for Excel Users - Full Course (1.1M views, 1 year ago, ~4h)
 Data Visualization with D3 – Full Course for Beginners [2022] (233K views, 1 year ago, ~20h)
 Data Science Job Interview – Full Mock Interview (248K views, 4 months ago, ~1.5h)
 Thu Vu data analytics - Top Courses to Learn Data Science Skills FAST!
Keith Galli (playlist) - Data Science
 1. Comprehensive Python Beautiful Soup Web Scraping Tutorial! (find/find_all, css select, scrape table) (276K views, 3 years ago, 1:13:03)
 2. Complete Python Pandas Data Science Tutorial! (Reading CSV/Excel files, Sorting, Filtering, Groupby) (2.8M views, 4 years ago, 1:00:27)
 3. Solving Real-World Data Science Interview Questions! (with Python Pandas) (75K views, 1 year ago, 1:47:50)
 4. 5 Jupyter Notebook Tips & Tricks to Improve your Data Science Workflow! (42K views, 1 year ago, 23:17)
 5. Intro to Data Visualization in Python with Matplotlib! (line graph, bar chart, title, labels, size) (215K views, 4 years ago, 32:33)
 6. Python Plotting Tutorial w/ Matplotlib & Pandas (Line Graph, Histogram, Pie Chart, Box & Whiskers) (285K views, 4 years ago, 1:01:30)
 7. Real-World Python Machine Learning Tutorial w/ Scikit Learn (sklearn basics, NLP, classifiers, etc) (220K views, 3 years ago, 1:40:49)
 8. Solving real world data science tasks with Python Beautiful Soup! (movie dataset creation) (270K views, 2 years ago, 3:24:18)
 9. Complete Python NumPy Tutorial (Creating Arrays, Indexing, Math, Statistics, Reshaping) (734K views, 4 years ago, 58:41)
 10. Solving real world data science tasks with Python Pandas! (1.3M views, 3 years ago, 1:26:07)
 11. Generating Mock Data with Python! (NumPy, Pandas, & Datetime Libraries) (25K views, 3 years ago, 1:00:26)
 12. Python Data Science Project Ideas! (for all skill levels) (68K views, 3 years ago, 15:45)
 13. Complete Natural Language Processing (NLP) Tutorial in Python! (with examples) (94K views, 1 year ago, 1:37:46)
 14. Complete Regular Expressions Tutorial! (with exercises for practice) (5.4K views, 4 months ago, 1:19:21)
 15. Introduction to Neural Networks in Python (what you need to know) | Tensorflow/Keras (81K views, 3 years ago, 1:00:37)
 16. Real-World Python Neural Nets Tutorial (Image Classification w/ CNN) | Tensorflow & Keras (78K views, 3 years ago, 1:01:14)
 17. Solving real world data science problems with Python! (computer vision edition) (36K views, 1 year ago, 1:21:38)
 18. How to Generate an Analytics Report (pdf) in Python! (136K views, 2 years ago, 49:15)
 19. How to Schedule & Automatically Run Python Code! (116K views, 2 years ago, 1:20:23)
 20. Solving real-world data analysis problems with Python Pandas! (Lego dataset analysis) (72K views, 1 year ago, 43:37)
 21. Full Data Science Mock Interview! (featuring Kylie Ying) (9.8K views, 7 months ago, 1:27:34)
Data Science projects
 Ken Jee - 5 Impactful Data Science Projects For Your Portfolio
 NASA
Datasets for NASA missions, research, activities, and more
Life science data (from NASA)
Data Science mathematics
Derek Banas - Probability for Data Science & Machine Learning
Derek Banas - Statistics for Data Science & Machine Learning
Data Nash - How Much Math Is REALLY In Data Science | What Math Do You Need For Data Science
 Data Nash - Every Data Scientist Should Read This Book
Brian Godsey - Think Like a Data Scientist: Tackle the data science process step-by-step
metacodeM - Statistics
 1. Basic Statistics 1 by Data Scientist [2-hour Full Course] (1.6K views, 10 days ago, 2:12:09)
 2. Statistics for Data Science Course [Part 1: Categorical and Quantitative Data] (1.6K views, 4 weeks ago, 13:27)
 3. Statistics for Data Science Course [Part 2: Mean, Median, and Mode] (298 views, 3 weeks ago, 17:57)
 4. Statistics for Data Science Course [Part 3: Variance and Standard Deviation] (392 views, 3 weeks ago, 11:19)
 5. Statistics for Data Science Course [Part 4 : Shape and Correlation] (345 views, 3 weeks ago, 15:17)
 6. Basic Statistics by Data Scientist [Part 5 : Probability] (466 views, 2 weeks ago, 14:57)
 7. Basic Statistics by Data Scientist [Part 6 : Conditional Probability] (357 views, 2 weeks ago, 17:25)
 8. Basic Statistics by Data Scientist [Part 7 : Bayes' Theorem] (1.2K views, 2 weeks ago, 16:29)
 9. Basic Statistics by Data Scientist [Part 8 : Random Variables] (458 views, 13 days ago, 11:52)
 10. Basic Statistics by Data Scientist [Part 9 : Probability Density Function] (253 views, 11 days ago, 13:31)
Data Science books
Essential Math for Data Science: Take Control of Your Data with Fundamental Linear Algebra, Probability, and Statistics - Thomas Nield (2022, 1st edition, 347 pages, O'Reilly Media, 4.5 stars from 231 ratings on Amazon)
Practical Statistics for Data Scientists: 50+ Essential Concepts Using R and Python - Andrew Bruce, Peter Bruce (2020, 2nd edition, 360 pages, O'Reilly Media, 4.6 stars from 793 ratings on Amazon)
Becoming a Data Head: How to Think, Speak, and Understand Data Science, Statistics, and Machine Learning - Alex J. Gutman, Jordan Goldmeier (2021, 1st edition, 272 pages, Wiley, 4.6 stars from 311 ratings on Amazon)
The Art of Statistics: How to Learn from Data - David Spiegelhalter (2021, 1st edition, 448 pages, Basic Books, 4.6 stars from 3,508 ratings on Amazon)
Data Science from Scratch: First Principles with Python - Joel Grus (2019, 2nd edition, 403 pages, O'Reilly Media, 4.4 stars from 700 ratings on Amazon)
Think Like a Data Scientist: Tackle the data science process step-by-step - Brian Godsey (2017, 1st edition, 328 pages, Manning, 4.5 stars from 40 ratings on Amazon)
Data Scientists - what do they do?
Tani Tech - https://www.youtube.com/watch?v=iymwofogLCs
Machine Learning
Machine learning general (how to learn, advices etc.)
 Boris Meinardus - How I'd learn ML in 2025 (if I could start over)
 Aleksa Gordić - The AI Epiphany - How I Got a Job at DeepMind as a Research Engineer (without a Machine Learning Degree!)
 Aleksa Gordić - How to get started with Machine Learning
Step 1: Learn to code in Python
 Go through the course Python - Learn Python - Full Course for Beginners [Tutorial]
 Go through the book "Automate the Boring Stuff with Python" by Al Sweigart
 If you don't want to read the book, you can watch the Automate the Boring Stuff with Python Programming Course
If you still feel your Python coding skills are weak go through the first 8 chapters of the book
If you feel comfortable with Python coding, skip the first 8 chapters and go through the rest of the book
That's all you need to know about Python. If you need something else, learn it on the fly by just Googling it!
Step 2: Get a high-level understanding of what Machine Learning is (NOTE: Aleksa mentioned that he took 2.5 months, while working, to go through these 2 courses)
 Course 1: Machine Learning by Andrew Ng
 Course 2: Deep Learning Specialization by Andrew Ng
Start working on projects and put them on GitHub + write a blog!
Kaggle
Step 3 (more practical):
 Course 1: Deep Learning for Coders with fastai and PyTorch
 Course 2: Deep Learning from the Foundations
Start focusing on one Deep Learning Framework; Aleksa recommends PyTorch
NOTE: The previous 3 steps can take up to 6 months if we're a beginner
Step 4: Start reading research papers and implement a single paper
List of places to find research papers (NOTE: Everything but the first link was added by the Copilot):
Arxiv - a good place to start
OpenAI
DeepMind
Google AI
Facebook AI
Twitter AI
LinkedIn AI
Microsoft Research
Apple AI
Amazon AI
Baidu AI
Alibaba AI
Tencent AI
Huawei AI
NVIDIA AI
Intel AI
IBM Research
MIT AI
Stanford AI
Berkeley AI
CMU AI
Oxford AI
NOTE: We're going to feel so dumb (I'm sure I will). Read the paper from start to end. It's OK if we don't understand everything on the first pass while reading the paper. Aleksa read about 20ish papers in Neural style transfer. We should read at least a couple of papers on a particular subject and then implement the paper.
Step 5: Mathematics
Resources:
Mathematics for Machine Learning by Marc Peter Deisenroth, A. Aldo Faisal, Cheng Soon Ong (NOTE: It took Aleksa about 3-4 months to go through this book but he supplemented it with the resources below)
3Blue1Brown (playlist) - Essence of Linear Algebra
3Blue1Brown (playlist) - Essence of Calculus
Jake VanderPlas - Python Data Science Handbook
We should go through the 5th chapter of the book - it's about Machine Learning
Ian Goodfellow, Yoshua Bengio, Aaron Courville - Deep Learning, and https://github.com/janishar/mit-deep-learning-book-pdf
NOTE: Maybe check the new book by Simon Prince called "Understanding Deep Learning". Check out this video Machine Learning Street Talk - Deep Learning is a strange beast.
BONUS TIPS:
Coursera - Barbara Oakley - Learning how to Learn
Don't learn tools for the sake of tooling. Learn them when you need them.
Aleksa doesn't even use Pandas because he doesn't work with structured data but with imagery because he works in computer vision. He uses PyTorch and NumPy (this short sentence is added by the Copilot)
Build your own stuff after going through the theory. Set the project goal - that's the "What" and a lot of "Hows" will follow up. If you need for example Pandas, to acomplish the project - learn it on the fly.
FOCUS, FOCUS, FOCUS. In the beginning, focus on the single deep learning framework (use PyTorch). Focus on the single application area (computer vision, NLP or something else).
Follow people on Twitter/X:
Yann LeCun
Geoffrey Hinton
Yoshua Bengio
Ian Goodfellow
Andrej Karpathy
Andrew Ng
François Chollet
Pieter Abbeel
Jeremy Howard
Rachel Thomas
Sebastian Ruder
Sylvain Gugger
Thomas Wolf
Hugging Face
OpenAI
DeepMind
Google AI
Facebook AI
Twitter AI
LinkedIn AI
Microsoft Research
Apple AI
Amazon AI
Baidu AI
Alibaba AI
Tencent AI
Huawei AI
NVIDIA AI
Intel AI
IBM Research
MIT AI
Stanford AI
Berkeley AI
CMU AI
Oxford AI
Data Science Central
Data Elixir
Data Science Weekly
Data Science Report
Data Science 101
Data Science Central
Data Science Central - Jobs
DataCamp
DataCamp - Pandas Cheat Sheet
etc.
Watch Lex Friedman's podcast
 Boris Meinardus - How I’d learn ML in 2024 (if I could start over)
 1. Learn Python
 2. Learn mathematics (high-school or entry-level college math; what's a derivate and how to compute it; what's a matrix and how the dot product works)
 (for example) edX: HarvardX: Introduction to Probability
 (for example) edX: UTAustinX: Linear Algebra - Foundations to Frontiers
 (for example) Coursera: Matrix Algebra for Engineers
 Khan Academy (probably the best option for learning math; it's free and it's very well structured)
 Brilliant
 College (no way)
 learn the basics; later, if you need something just Google it or similar (this!)
 3. ML developer stack
 Jupyter notebooks
 Pandas (tool for dealing with data in tabular format)
 NumPy (library for doing maths with matrices or arrays; can be used to implement mathematics we've learned previously, like doing the dot product between two matrices easily etc.)
 matplotlib (tool for visualizing data and graphs)
 4. ML Courses (which will give me practical experience with ML concepts)
 Machine learning specialization by Andrew Ng
 SciKit learn, Tensorflow (but learn PyTorch instead)
 Andrej Karpathy's "Neural Networks: Zero to Hero"
 Implementing an NLP model, from the ground up
 Goes all the way up to a Transformer model
 Also, goes through all the mathematics of backpropagation etc.
 Deep learning specialization
 Focuses on implementing and training Neural networks
 Includes Hugging Face - Hugging Face has an NLP course on their website, with even more advanced concepts in NLP (if we're interested in NLP that is)
 5. Projects
 Kaggle (work on challenges)
 start with simpler challenges
 eventually move to working on more complex projects (they also come with prize money; they require a lot of compute)
 Reimplementing a paper and recreating the results
 Boris Meinardus - 7 Mistakes Beginner ML Students Make Every Year
 Boris Meinardus - This Simple RESUME got me 5 Machine Learning Interviews
 Boris Meinardus - What Is Self-Supervised Learning and Why Care?
 Thu Vu data analytics - How I'd Learn AI (If I Had to Start Over)
 Dave Ebbelaar - How I'd Learn AI in 2023 (if I could start over)
 Sahil & Sarra (former "The Power Couple") - How to learn AI and get RICH in the AI revolution
 LunarTech - Machine Learning Roadmap 2024 | How I'd Learn Machine Learning in 2024 (If I could start over)
 Amazon Web Services - How I Started a Career in Machine Learning - No PHD Required
 Kylie Ying - How to learn Machine Learning (ML/AI Roadmap 2024)
Machine learning projects
 Smitha Kolan - Machine Learning Engineer - ABSOLUTE BEGINNER Machine Learning NLP Project (Tutorial)
 Boris Meinardus - How To Build A Machine Learning Portfolio in 2024
 Boris Meinardus - This ML Project Gives You an Unfair Advantage
Reimplementing a paper and recreating it's results
Step 1: Read the paper
Methodology: Use colored markers to highlight the important parts
Color no. 1 (General understanding): We want to highlight the parts that are important for understanding the paper
Color no. 2 (Implementation details): Actively highlight the parts relevant for the implementation.
This includes things like used loss loss functions, used activation functions, used architectures, used datasets, used hyperparameters etc. When highlighting these parts, we can already start envisioning how we would start to implement the architecture and which other repositories we alredy know that have similar implementations that we can use for our own new implementation. Or we write down a list of common modules we need to look up existing implementations for. The idea is not to not to reinvent the wheel, but to use existing implementations and to understand how they work and how they can be adapted to our own needs.
Color no. 3 (Datasets): Since we are not only reimplement the paper but also recreate results to actually verify whether we implemented the paper successfully, we need to train on the same datasets and evaluate on the same ones. Highlighting those should not too difficult, since the paper should already mention the datasets used and the evaluation metrics used.
It might also be important to look for details about the compute that the authors used. If they used expensive compute, we might need to look for alternatives or we might need to look for ways to reduce the compute needed. This might be important for us, since we might not have access to the same compute as the authors of the paper.
Tackle the datasets. That means - find the datasets used in the paper and download them.
Step 2: Implementing the dataset and data loader classes (PyTorch).
Data loader is used to provide data in a preprocessed format. That way we can very consistently get a batch of data and just focus on the training logic. When implementing the dataset and data loader classes he recomments to use Jupyter Notebooks. That makes it very easy to save certain variables (like the path to the dataset) and visualize everything we need.
One final thing is if we are working on a reinforcement learning paper, the equivalent to implementing the dataset classes is setting up the gym environment.
Step 3: Start coding
(NOTE: Perhaps our paper focuses more on a new training technique rather a new architecture).
Since we've highlighted the novel elements of the architecture and found existing implementations of modules we might need, his recommendation is to just start coding(!!!). Don't think too much about making it right the first time. Start writing our torch.nn.module class and initialize all layers we might need. If they are larger, more complex models, we can directly start writing a function for those. [TODO: Check the mentioned example].
Use "Weights and Biases" to track our experiments. It's a tool that allows us to track our experiments and visualize them. It's a very powerful tool and it's free to use. (added by the Copilot)
 Algorithmic Simplicity - Deriving the Transformer Neural Network from Scratch #SoME3
Diffusion models
 DeepFindr - Diffusion models from scratch in PyTorch
Machine Learning basics
David MacKay - Information Theory, Inference, and Learning Algorithms

Produced by: David MacKay (University of Cambridge) Author: David MacKay, University of Cambridge

A series of sixteen lectures covering the core of the book "Information Theory, Inference, and Learning Algorithms" (Cambridge University Press, 2003, http://www.inference.eng.cam.ac.uk/mackay/itila/) which can be bought at Amazon (http://www.amazon.co.uk/exec/obidos/ASIN/0521642981/davidmackay0f-21), and is available free online (http://www.inference.eng.cam.ac.uk/mackay/itila/).

A subset of these lectures used to constitute a Part III Physics course at the University of Cambridge. The high-resolution videos and all other course material can be downloaded from the Cambridge course website (http://www.inference.eng.cam.ac.uk/mackay/itprnn/).

Snapshots of the lecture can be found here: http://www.inference.eng.cam.ac.uk/itprnn_lectures/

These lectures are also available at http://videolectures.net/course_information_theory_pattern_recognition/ (synchronized with snapshots and slides)

Lecture 1: Introduction to Information Theory (329K views, 9 years ago, 1:01:51)
Lecture 2: Entropy and Data Compression (I): Introduction to Compression, Inf.Theory and Entropy (90K views, 9 years ago,51:09)
Lecture 3: Entropy and Data Compression (II): Shannon's Source Coding Theorem, The Bent Coin Lottery (55K views, 9 years ago, 51:01)
Lecture 4: Entropy and Data Compression (III): Shannon's Source Coding Theorem, Symbol Codes (40K views, 9 years ago, 56:58)
Lecture 5: Entropy and Data Compression (IV): Shannon's Source Coding Theorem, Symbol Codes (33K views, 9 years ago, 1:02:48)
Lecture 6: Noisy Channel Coding (I): Inference and Information Measures for Noisy Channels (27K views, 9 years ago, 54:42)
Lecture 7: Noisy Channel Coding (II): The Capacity of a Noisy Channel (26K views, 9 years ago, 46:54)
Lecture 8: Noisy Channel Coding (III): The Noisy-Channel Coding Theorem (23K views, 9 years ago, 1:08:59)
Lecture 9: A Noisy Channel Coding Gem, And An Introduction To Bayesian Inference (I) (15K views, 9 years ago, 48:36)
Lecture 10: An Introduction To Bayesian Inference (II): Inference Of Parameters And Models (19K views, 9 years ago, 1:15:53)
Lecture 11: Approximating Probability Distributions (I): Clustering As An Example Inference Problem (15K views, 9 years ago, 56:56)
Lecture 12: Approximating Probability Distributions (II): Monte Carlo Methods (I) (22K views, 9 years ago, 1:23:48)
Lecture 13: Approximating Probability Distributions (III): Monte Carlo Methods (II): Slice Sampling (14K views, 9 years ago, 1:47:57)
Lecture 14: Approximating Probability Distributions (IV): Variational Methods (18K views, 9 years ago, 46:35)
Lecture 15: Data Modelling With Neural Networks (I): Feedforward Networks: The Capacity Of A Neuron (14K views, 9 years ago, 1:27:16)
Lecture 16: Data Modelling With Neural Networks (II): Content-Addressable Memories And State (10K views, 9 years ago, 1:36:33)
r2d3 - A visual introduction to machine learning (text)

Part 1 - A Decision Tree (text)
Part 2 - Model Tuning and the Bias-Variance Tradeoff (text)
Machine learning courses
Premium (Udemy, Coursera etc.)
Udemy - ZTM, Andrei Neagoie, Daniel Bourke - Complete Machine Learning & Data Science Bootcamp 2023 (Rating: 4.6 out of 5 (17,179 ratings) 99,450 students), 43.5h, Last updated 6/2023
Udemy - Jose Portilla - Python for Machine Learning & Data Science Masterclass (4.7 out of 5 (12,599 ratings) 91,232 students, 44h, Last updated 9/2021)
Free
 Jeremy Howard - A Hackers' Guide to Language Models
 Programming with Mosh - Python Machine Learning Tutorial (Data Science)
 Eye On AI - Why Attention is Crucial in AI
 freeCodeCamp - Machine Learning with Python and Scikit-Learn – Full Course
 freeCodeCamp (playlist) - Machine Learning
 1. Machine Learning for Everybody – Full Course (1.7M views, 10 months ago, 3:53:53)
NOTE: The course is using TensorFlow
 2. TensorFlow 2.0 Complete Course - Python Neural Networks for Beginners Tutorial (2.7M views, 3 years ago, 6:52:08)
 3. Self-Driving Car with JavaScript Course – Neural Networks and Machine Learning (1.9M views, 1 year ago, 2:32:40)
 4. No Black Box Machine Learning Course – Learn Without Libraries (280K views, 4 months ago, 3:51:31)
 5. PyTorch for Deep Learning & Machine Learning – Full Course (797K views, 10 months ago, 25:37:26)
 6. Practical Deep Learning for Coders - Full Course from fast.ai and Jeremy Howard (333K views, 2 years ago, 11:12:32)
 7. Deep Learning Crash Course for Beginners (580K views, 3 years ago, 1:25:39)
 8. Python TensorFlow for Machine Learning – Neural Network Text Classification Tutorial (218K views, 1 year ago, 1:54:11)
 9. Keras with TensorFlow Course - Python Deep Learning and Neural Networks for Beginners Tutorial (784K views, 3 years ago, 2:47:55)
 10. OpenCV Course - Full Tutorial with Python (2.5M views, 2 years ago, 3:41:42)
 11. How Deep Neural Networks Work - Full Course for Beginners (1.4M views, 4 years ago, 3:50:57)
 12. TensorFlow 2.0 Crash Course (497K views, 3 years ago, 2:13:17)
 13. Scikit-Learn Course - Machine Learning in Python Tutorial (399K views, 3 years ago, 2:54:25)
 14. Scikit-learn Crash Course - Machine Learning Library for Python (231K views, 2 years ago, 2:09:22)
 15. Machine Learning Course for Beginners (1.3M views, 1 year ago, 9:52:19)
 16. AlphaZero from Scratch – Machine Learning Tutorial (95K views, 5 months ago, 4:07:54)
 17. Computer Vision and Perception for Self-Driving Cars (Deep Learning Course) (225K views, 1 year ago, 1:59:38)
 Assembly AI (playlist) - Machine Learning From Scratch Full course
 1. Machine Learning From Scratch Full course (50K views, 2 years ago, 1:05)
 2. How to implement KNN from scratch with Python (88K views, 2 years ago, 9:24)
 3. How to implement Linear Regression from scratch with Python (54K views, 2 years ago, 17:03)
 4. How to implement Logistic Regression from scratch with Python (68K views, 2 years ago, 14:04)
 5. How to implement Decision Trees from scratch with Python (65K views, 2 years ago, 37:24)
 6. How to implement Random Forest from scratch with Python (26K views, 2 years ago, 13:31)
 7. How to implement Naive Bayes from scratch with Python (28K views, 2 years ago, 14:37)
 8. How to implement PCA (Principal Component Analysis) from scratch with Python (16K views, 2 years ago, 12:16)
 9. How to implement Perceptron from scratch with Python (34K views, 2 years ago, 13:46)
 10. How to implement SVM (Support Vector Machine) from scratch with Python (28K views, 2 years ago, 14:45)
 11. How to implement K-Means from scratch with Python (15K views, 2 years ago, 23:42)
Machine learning books
Machine Learning with Python Cookbook: Practical Solutions from Preprocessing to Deep Learning - Chris Albon (2023, 2nd edition, 413 pages, O'Reilly Media)
Machine Learning with PyTorch and Scikit-Learn: Develop machine learning and deep learning models with Python - Sebastian Raschka, Yuxi (Hayden) Liu (2022, 1st edition, 774 pages, Packt Publishing)
Introduction to Machine Learning with Python: A Guide for Data Scientists - Andreas C. Müller, Sarah Guido (2016, 1st edition, 398 pages, O'Reilly Media)
Deep Learning
Tutorials
 Alexander Amini (playlist) - MIT 6.S191: Introduction to Deep Learning
Course lectures for MIT Introduction to Deep Learning.

http://introtodeeplearning.com

69 videos 3,149,217 views Updated today

 1. MIT Introduction to Deep Learning | 6.S191 (210K views, 1 month ago, 1:09:58)
 2. MIT 6.S191: Recurrent Neural Networks, Transformers, and Attention (63K views, 3 weeks ago, 1:01:31)
 3. MIT 6.S191: Convolutional Neural Networks (24K views, 2 weeks ago, 1:07:58)
 4. MIT 6.S191: Deep Generative Modeling (20K views, 13 days ago, 56:19)
 5. MIT 6.S191: Reinforcement Learning (16K views, 6 days ago, 1:00:19)
 6. 6.S191: Language Models and New Frontiers (4 waiting (Premieres 03/06/2024, 16:00, UPCOMING MIT )
 7. MIT Introduction to Deep Learning (2023) | 6.S191 (1.9M views, 1 year ago, 58:12)
 8. MIT 6.S191 (2023): Recurrent Neural Networks, Transformers, and Attention (650K views, 1 year ago, 1:02:50)
 9. MIT 6.S191 (2023): Convolutional Neural Networks (242K views, 1 year ago, 55:15)
 10. MIT 6.S191 (2023): Deep Generative Modeling (295K views, 1 year ago, 59:52)
 11. MIT 6.S191 (2023): Robust and Trustworthy Deep Learning (85K views, 1 year ago, 53:50)
 12. MIT 6.S191 (2023): Reinforcement Learning (121K views, 1 year ago, 57:33)
 13. MIT 6.S191 (2023): Deep Learning New Frontiers (80K views, 1 year ago, 1:08:47)
 14. MIT 6.S191 (2023): Text-to-Image Generation (44K views, 1 year ago, 44:36)
 15. MIT 6.S191 (2023): The Modern Era of Statistics (78K views, 1 year ago, 53:10)
 16. MIT 6.S191 (2023): The Future of Robot Learning (43K views, 1 year ago, 1:02:42)
 17. MIT Introduction to Deep Learning (2022) | 6.S191 (615K views, 2 years ago, 49:01)
 18. MIT 6.S191 (2022): Recurrent Neural Networks and Transformers (252K views, 2 years ago, 58:18)
 19. MIT 6.S191 (2022): Convolutional Neural Networks (119K views, 2 years ago, 49:23)
 20. MIT 6.S191 (2022): Deep Generative Modeling (79K views, 2 years ago, 54:46)
 21. MIT 6.S191 (2022): Reinforcement Learning (82K views, 2 years ago, 54:53)
 22. MIT 6.S191 (2022): Deep Learning New Frontiers (36K views, 2 years ago, 53:29)
 23. MIT 6.S191: LiDAR for Autonomous Driving (29K views, 2 years ago, 49:04)
 24. MIT 6.S191: Automatic Speech Recognition (28K views, 2 years ago, 41:44)
 25. MIT 6.S191: AI for Science (35K views, 2 years ago, 44:43)
 26. MIT 6.S191: Uncertainty in Deep Learning (30K views, 2 years ago, 50:08)
 27. MIT 6.S191 (2021): Introduction to Deep Learning (556K views, 3 years ago, 56:36)
 28. MIT 6.S191 (2021): Recurrent Neural Networks (296K views, 3 years ago, 1:00:31)
 29. MIT 6.S191 (2021): Convolutional Neural Networks (160K views, 3 years ago, 55:57)
 30. MIT 6.S191 (2021): Deep Generative Modeling (106K views, 3 years ago, 1:01:54)
 31. MIT 6.S191 (2021): Reinforcement Learning (102K views, 3 years ago, 57:08)
 32. MIT 6.S191 (2021): Deep Learning New Frontiers (62K views, 3 years ago, 50:46)
 33. MIT 6.S191: Evidential Deep Learning and Uncertainty (57K views, 3 years ago, 48:52)
 34. MIT 6.S191: AI Bias and Fairness (46K views, 3 years ago, 43:22)
 35. MIT 6.S191: Deep CPCFG for Information Extraction (20K views, 3 years ago, 40:58)
 36. MIT 6.S191: Taming Dataset Bias via Domain Adaptation (22K views, 3 years ago, 42:51)
 37. MIT 6.S191: Towards AI for 3D Content Creation (20K views, 3 years ago, 47:59)
 38. MIT 6.S191: AI in Healthcare (31K views, 3 years ago, 33:31)
 39. MIT 6.S191 (2020): Introduction to Deep Learning (1.2M views, 4 years ago, 52:52)
 40. MIT 6.S191 (2020): Recurrent Neural Networks (392K views, 4 years ago, 45:28)
 41. MIT 6.S191 (2020): Convolutional Neural Networks (306K views, 4 years ago, 37:20)
 42. MIT 6.S191 (2020): Deep Generative Modeling (174K views, 4 years ago, 40:40)
 43. MIT 6.S191 (2020): Reinforcement Learning (107K views, 4 years ago, 44:11)
 44. MIT 6.S191 (2020): Deep Learning New Frontiers (118K views, 4 years ago, 38:10)
 45. MIT 6.S191 (2020): Neurosymbolic AI (72K views, 4 years ago, 41:10)
 46. MIT 6.S191 (2020): Generalizable Autonomy for Robot Manipulation (34K views, 4 years ago, 47:00)
 47. MIT 6.S191 (2020): Neural Rendering (31K views, 4 years ago, 36:44)
 48. MIT 6.S191 (2020): Machine Learning for Scent (40K views, 4 years ago, 38:52)
 49. Barack Obama: Intro to Deep Learning | MIT 6.S191 (609K views, 4 years ago, 1:50)
 50. MIT 6.S191 (2019): Introduction to Deep Learning (230K views, 5 years ago, 45:28)
 51. MIT 6.S191 (2019): Recurrent Neural Networks (117K views, 5 years ago, 36:31)
 52. MIT 6.S191 (2019): Convolutional Neural Networks (145K views, 5 years ago, 41:17)
 53. MIT 6.S191 (2019): Deep Generative Modeling (61K views, 5 years ago, 43:44)
 54. MIT 6.S191 (2019): Deep Reinforcement Learning (104K views, 5 years ago, 44:53)
 55. MIT 6.S191 (2019): Deep Learning Limitations and New Frontiers (33K views, 5 years ago, 36:21)
 56. MIT 6.S191 (2019): Visualization for Machine Learning (Google Brain) (64K views, 5 years ago, 37:40)
 57. MIT 6.S191 (2019): Biologically Inspired Neural Networks (IBM) (33K views, 5 years ago, 31:30)
 58. MIT 6.S191 (2019): Image Domain Transfer (NVIDIA) (21K views, 5 years ago, 46:33)
 59. MIT 6.S191 (2018): Introduction to Deep Learning (523K views, 6 years ago, 42:40)
 60. MIT 6.S191 (2018): Sequence Modeling with Neural Networks (83K views, 6 years ago, 27:13)
 61. MIT 6.S191 (2018): Convolutional Neural Networks (61K views, 6 years ago, 35:10)
 62. MIT 6.S191 (2018): Deep Generative Modeling (30K views, 6 years ago, 44:07)
 63. MIT 6.S191 (2018): Deep Reinforcement Learning (25K views, 6 years ago, 32:49)
 64. MIT 6.S191 (2018): Deep Learning Limitations and New Frontiers (18K views, 6 years ago, 31:37)
 65. MIT 6.S191 (2018): Issues in Image Classification (15K views, 6 years ago, 17:18)
 66. MIT 6.S191 (2018): Faster ML Development with TensorFlow (22K views, 6 years ago, 19:20)
 67. MIT 6.S191 (2018): Deep Learning - A Personal Perspective (17K views, 6 years ago, 32:56)
 68. MIT 6.S191 (2018): Beyond Deep Learning: Learning+Reasoning (27K views, 6 years ago, 32:21)
 69. MIT 6.S191 (2018): Computer Vision Meets Social Networks (24K views, 6 years a 33:58go,)
 ACMSIGGRAPH - Deep Learning: A Crash Course (2018) | SIGGRAPH Courses
 metacodeM (playlist) - Deep Learning
 1. What are ML and DL?ㅣChapter 1. Deep learning (809 views, 7 days ago, 16:28)
 2. Differences between ML and DLㅣChapter 2. Deep learning (7.8K views, 5 days ago, 17:43)
Artificial intelligence
Artificial intelligence general (how to learn, advices etc.)
 freeCodeCamp.org (LunarTech) - AI Engineer Roadmap – How to Learn AI in 2025
 David Bombal - You need to learn AI in 2024! (And here is your roadmap)
 Machine Learning Street Talk - Deep Learning is a strange beast.
 Jay Shah - Best resources to remain updated to Machine Learning Research | Siddha Ganju, @NVIDIA
 deeplizard - CUDA Explained - Why Deep Learning uses GPUs
 Thu Vu data science - How I'd Learn AI (If I Had to Start Over)
Tutorials
 freeCodeCamp - Harvard CS50’s Artificial Intelligence with Python – Full University Course
 Wes Roth - AI Tutorials
 1. Install Open Interpreter in 2 min | The free, open source CODE INTERPRETER! (24K views, 2 months ago, 8:31)
 2. AutoGen Tutorial 🔥 How to Build POWERFUL AI Agents (90K views, 1 month ago, 30:43)
 3. AI Plays Pokemon with Reinforcement Learning (14K views, 1 month ago, 14:25)
 4. OpenAI Playground Assistant is POWERFUL! Here's how to BUILD one... (45K views, 12 days ago, 8:42)
 5. Create Custom GPTs | No code AI automation | OpenAI App Store | Complete Guide (189K views, 11 days ago, 26:59)
 6. Zapier AI Actions & GPTs | Tutorial, Examples and Automation Ideas 🔥 (50K views, 10 days ago, 30:52)
 7. OpenAI Assistants API to Build AI Agent SWARMS. Better than AutoGen? (30K views, 6 days ago, 34:52)
 Samson Zhang - Building a neural network FROM SCRATCH (no Tensorflow/Pytorch, just numpy & math)
 Akhil Sharma - LLM Concepts
 1. What Are Transformers - LLM Concepts ( EP 1 ) #llm #ai #ml #transformers #gpt #gpt4 #gpt3 (750 views • 1 month ago, 12:49)
 2. What is Parameter Offloading? - LLM Concepts ( EP 2 ) #llm #ai #artificialintelligence (483 views • 1 month ago, 6:42)
 3. What is Quantization? - LLM Concepts ( EP - 3 ) #quantization #llm #ml #ai #artificialintelligence (298 views • 1 month ago, 6:28)
 4. What is Post Training Quantization - GGUF, AWQ, GPTQ - LLM Concepts ( EP - 4 ) #ai #llm #genai #ml (360 views • 1 month ago, 6:35)
 5. What is LLM Sharding - LLM Concepts ( EP - 5 ) #llm #artificialintelligence #largelanguagemodels (676 views • 1 month ago, 6:00)
 6. What is Attention? - LLM Concepts ( EP - 6 ) #llm #largelanguagemodels #generativeai #genai #ai #ml (365 views • 1 month ago, 5:00)
 7. What Is Finetuning? - LLM Concepts ( EP - 7 ) #llm #largelanguagemodels #artificialintelligence (286 views • 8 days ago, 9:41)
Fine-tuning
 Hamel Husain - Why Fine Tuning is Dead w/Emmanuel Ameisen
 Hamel Husain - Deploying Fine-Tuned Models
 Prompt Engineering - LLAMA-3.1: EASIET WAY To FINE-TUNE ON YOUR DATA
 Entry Point AI - LoRA & QLoRA Fine-tuning Explained In-Depth
Fine-tuning projects
https://www.mlexpert.io/bootcamp
 Hugging Face - Fine-tuning a model on a text classification task
 Venelin Valkov - Fine-tuning Tiny LLM on Your Data | Sentiment Analysis with TinyLlama and LoRA on a Single GPU
 Venelin Valkov - Fine-Tuning Llama 3 on a Custom Dataset: Training LLM for a RAG Q&A Use Case on a Single GPU
 https://www.mlexpert.io/bootcamp/fine-tuning-llama-3-llm-for-rag
 Shaw Talebi - QLoRA—How to Fine-tune an LLM on a Single GPU (w/ Python Code)
https://platform.openai.com/docs/guides/fine-tuning/preparing-your-dataset
https://hn.algolia.com/?q=fine+tuning
Mathematics for AI
 metacodeM - Linear Algebra
 1. Linear Algebra Tutorial by PhD in AIㅣ2-hour Full Course(74K views, 4 weeks ago, 2:07:26)
 2. Linear Algebra Tutorial for AI [ Part 1: Dimensions ](1.7K views, 1 month ago, 16:19)
 3. Linear Algebra Tutorial for AI [ Part 2: Linear Independence and Rank ](375 views, 1 month ago, 15:27)
 4. Linear Algebra Tutorial for AI [ Part 3: Matrix as Linear Operator ](317 views, 1 month ago, 16:06)
 5. Linear Algebra Tutorial for AI [ Part 4: Application in Neural Networks ](696 views, 1 month ago, 12:39)
 6. Linear Algebra Tutorial for AI [ Part 5: Determinant of a Matrix ](212 views, 1 month ago, 13:33)
 7. Inverse Matrix and Dot ProductㅣLinear Algebra for AI [ Part 6 ](264 views, 1 month ago, 15:31)
 8. Eigenvectors and Eigenvalues IㅣLinear Algebra for AI [ Part 7 ](446 views, 1 month ago, 10:12)
 9. Eigenvectors and Eigenvalues II [ Linear Algebra for AI - Part 8 ](537 views, 1 month ago, 13:15)
 10. Principal Component Analysis (PCA) [ Linear Algebra for AI - Part 9 ](277 views, 1 month ago, 14:30)
 11. Linear Algebra Review in 10-min (feat. PhD in AI)(328 views, 3 days ago, 10:35)
Artificial intelligence articles
WaitButWhy - The AI Revolution: The Road to Superintelligence
Artificial intelligence books
Deep Learning for Coders with Fastai and PyTorch: AI Applications Without a PhD - Jeremy Howard, Sylvain Gugger (2020, 1st edition, 621 pages, O'Reilly Media, 4.7 stars from 500 reviews on Amazon)
Inside Deep Learning: Math, Algorithms, Models - Edward Raff (2022, Annotated edition, 600 pages, Manning, 4.7 stars from 24 reviews on Amazon)
Deep Learning with Python, Second Edition - François Chollet (2021, 2nd edition, 504 pages, Manning, 4.7 stars from 345 reviews on Amazon)
Deep Learning with PyTorch: Build, train, and tune neural networks using Python tools - Eli Stevens, Luca Antiga, Thomas Viehmann (2020, 1st edition, 520 pages, Manning, 4.4 stars from 119 reviews on Amazon)
Mathematics courses (with my notes)
 Khan Academy - Statistics and Probability
 Unit 1: Analyzing categorical data

 Lesson 1: Analyzing one categorical variable
Median - is the middle value in a set of data. Example, 100 is median in this array of data: 75, 80, 100 (this is median), 100, 100.
Midrange - is the mean of the highest and lowest values in a set of data.
Example: for the array of data 75, 80, 100, 100, 100 the midrange is (75+100)/2=87.5
Mean - is the average value in a set of data. Example, 100 is mean in this array of data
Average - is the average value in a set of data.
NOTE: If someone says "average" without giving more information they're probably thinking about the arithmetic mean.
Example: for the array of data 75, 80, 100, 100, 100 the average is (75+80+100+100+100)/5=91
Mode - is the most commommon score. In 75, 80, 100, 100, 100, the mode is 100 because it appears 3 times.
Range - is the difference between the highest and lowest values in a set of data. Example: for the array of data 75, 80, 100, 100, 100 the range is 100-75=25
Lesson 2: Two-way tables
Example of a table with two variables

Preference	Male	Female
Prefers dogs	36	22
Prefers cats	8	26
No preference	2	6
Notice that there are two variables - gender and preference - this is where the two in two-way frequency table comes from.
The cells tell us the number (or frequency) of students. For example, the 36 is in the male column and the prefers dogs row. This tells us that there are 36 male students who prefer dogs.

 Unit 2: Displaying and comparing quantitative data

Dot plots - are used to show individual data points (bad if we have a lot of data).
Bar graphs - are used to show groups of data (good if we have a lot of data).
Histograms - displays ranges of data (good if we have a lot of data). Example: 0-10, 11-20, 21-30, etc.
Databases
 Nerd's Lesson - Meta - Database Engineering Complete Course | DBMS Complete Course*

 BroCode - MySQL: JOINS are easy (INNER, LEFT, RIGHT)

 JomaClass - SQL Joins: Difference Between Inner/Left/Right/Outer Joins

 Learn at Knowstar (playlist) - SQL Concepts

 1. SQL101 - DDL statements - Create, Alter, Drop (8.9K views, 4 years ago, 10:10)
 2. SQL DML Statements | Select | Update | Insert | Delete (8K views, 3 years ago, 19:36)
 3. SQL tutorial | Where Clause with Options (2K views, 3 years ago, 14:58)
 4. SQL Tutorial : Order By Clause (1K views, 3 years ago, 6:07)
 5. SQL Query | How to check for Alphanumeric values | Like | Wildcards (14K views, 2 years ago, 10:37)
 6. SQL Concepts | Types of Joins | SQL Tutorial (1.6K views, 2 years ago, 27:57)
 7. How to install SQL Server database | SQL Server Management Studio | Sample database | Free editions (2.8K views, 2 years ago, 15:28)
 8. SQL Query | Order of Execution (4.5K views, 1 year ago, 8:37)
 9. SQL | Recursive CTE | Practical Examples and 5 Use Cases | Sequences | Hierarchies (6.5K views, 1 year ago, 26:34)
 10. SQL Index explained in 5 minutes| What, Why & How they improve performance| Clustered |Non Clustered (5K views, 11 months ago, 5:54)
 11. SQL | Dynamic Data Masking | How to mask sensitive data | MS SQL (7.3K views, 10 months ago, 16:47)
 12. SQL | CharIndex or PatIndex | Difference #shorts (14K views, 10 months ago, 1:00)
 13. SQL | How to perform conditional / dynamic joins on multiple tables based on column value (5.7K views, 10 months ago, 8:52)
 14. SQL | Cross Apply | When to Use | Difference between Cross Apply and Inner Join (3.6K views, 8 months ago, 13:50)
 15. SQL | NOT IN Vs NOT EXISTS (Which one to use?) (5.9K views, 7 months ago, 10:03)
 16. SQL | How to add a column if it already does not exist | Error handling (3K views, 7 months ago, 5:16)
 17. SQL tutorial | Date Functions | Difference between DATEDIFF and DATEADD (4.5K views, 5 months ago, 19:25)
 18. SQL | Constraints in SQL (1.5K views, 5 months ago, 0:37)
 19. 8 Tips & Pointers to solve SQL Complex Queries ! (BONUS Tip Included !) (4.3K views, 5 months ago, 13:19)
 20. SQL | Subquery or CTE - Which one to choose? Difference between Subquery and CTE (3.5K views, 4 months ago, 11:01)
 21. SQL CTE | Follow these 5 Rules while Creating a CTE (Avoid these mistakes !) (2K views, 4 months ago, 7:33)
 22. SQL Tutorial | How to Avoid a Divide By Zero Error in SQL | NULLIF (1.6K views, 4 months ago, 5:49)
 23. SQL | IIF Function | Learn a Shorthand for CASE #shorts (8.4K views, 3 months ago, 0:55)
 24. SQL Interview Question - Difference between Count(*), Count(1), Count(colname) | Which is fastest (148K views, 2 years ago, 7:39)
 25. SQL Order Of Execution | In which order does the clauses in a SQL Query execute? (1.7K views, 3 months ago, 0:17)
 26. SQL Quiz | SQL Order By will put NULLs at top or bottom? (2.4K views, 3 months ago, 0:19)
 27. SQL | Windows Vs Aggregate Functions (12K views, 3 months ago, 0:37)
 28. SQL | How to Upload / Restore a Database in SQL Server? (6K views, 3 months ago, 0:30)
 29. SQL | Difference Between Union Vs Union ALL | Delete Vs Truncate | SQL Interview Questions (1.2K views, 1 month ago, 4:32)
Interactive SQL tutorials
SQLBolt
SQLZOO
Spathon - Visual JOIN - Understand how joins work by interacting and see it visually
Platforms for learning
Elements of AI - free course on AI
Talks
TEDxTalks - Neuroscience and Artificial Intelligence Need Each Other | Marvin Chun | TEDxKFAS
WeAreDevelopers - Deep Learning for Mobile devices—Siddha Ganju
Interviews
Edan Meyer - I Talked with Rich Sutton
Aleksa Gordić - The AI Epiphany - Tanishq Abraham (PhD at 19) - MedARC
Jeremy Howard - Tanishq Mathew Abraham - Their Life and Work Eps 1
Weights & Biases - Scaling LLMs and Accelerating Adoption: Interview with Aidan Gomez
Lex Fridman - Charles Isbell and Michael Littman: Machine Learning and Education | Lex Fridman Podcast #148
IBE Munich - Traditional Statistics vs Machine Learning
Jay Shah - Algorithmic Reasoning, Graph Neural Nets, AGI and Tips to researchers | Petar Veličković
Jay Shah - Siddha Ganju, Self-Driving Architect @NVIDIA | @ForbesBreakingNews
SparX by Mukesh Bansal - Why Machines Learn: The Elegant Math Behind AI with Anil Ananthaswamy | SparX by Mukesh Bansal
Breaking Math - Why Machines Learn: The Math Behind AI
YouTube channels
metacodeM - Machine Learning, Data Science, Python, and more
Whether you're exploring the realms of AI, data science, machine learning, deep learning, LLM, or statistics, our expert instructors, who are either actively working in tech fields or hold Ph.D.s in their domains, are here to guide you for free.

Our goal is to empower you with the knowledge and skills needed to thrive in the dynamic world of rapidly evolving technologies.

Additionally, we're excited to announce the upcoming launch of our community website, where you can engage with fellow learners, stay updated on industry trends, and access exclusive resources related to Industry 4.0.

We’ll also offer comprehensive courses designed to provide you with in-depth learning experiences. Upon completion, you'll have the opportunity to earn certificates, validating your expertise.

deeplizard - ML + DL + AI tutorials, AI art tutorials, NLP tutorials etc.
Machine Learning Street Talk
DeepFindr - Machine Learning / Data Science topics
Make Data Useful - Data science and analytics channel with a nice mix of Python tutorials and analysis.
codebasics - Data Analytics, Data Science and Machine Learning tutorials
Other links and playlists
https://ainowinstitute.org/publication/policy/compute-and-ai

Institute of Computing for Climate Science (ICCS) - ICCS Summer School 2023

Recordings from ICCS's second annual summer school in July 2023.

Recordings from ICCS's second annual summer school in July 2023.

 1. Day 1 - Welcome to ICCS Summer School - Emily Shuckburgh, Colm-cille Caulfield, Marla Fuchs (180 views, 6 months ago, 14:32)
 2. Day 2 - Using GitHub effectively for collaborative development (114 views, 6 months ago, 1:23:40)
 3. Introduction to the 2023 ICCS Summer School Hackathon (66 views, 7 months ago, 4:15)
 4. Day 1 - Keynote - Machine Learning for Climate Change and Environmental Sustainability (182 views, 6 months ago, 1:09:58)
 5. Day 1 - David Kamm - 10 minute quick fire science talk (17 views, 6 months ago, 7:14)
 6. Day 1 - Keren Jakhar - 10 minute quick fire science talk (31 views, 6 months ago, 9:14)
 7. Day 1 - Simon Driscoll - 10 minute quick fire science talk (45 views, 6 months ago, 8:18)
 8. Day 2 - Introduction to GPU Programming Teaching - Paul Richmond (3.1K views, 6 months ago, 1:26:05)
 9. Day 2 - Keynote - Reproducibility and open software practises in climate research (335 views, 6 months ago, 51:48)
 10. Day 2 - Panel on the importance of software engineering goodpractices in climate science (457 views, 6 months ago, 1:27:57)
 11. Day 3 - Ivo Pasmans - 10 minute quick fire science talk (146 views, 6 months ago, 9:49)
 12. Day 3 - Levin Rug - 10 minute quick fire science talk (109 views, 6 months ago, 8:44)
 13. Day 3 - Introduction to Machine Learning with Pytorch Teaching - Part 1 of 2 - ANNs and exercises (174 views, 6 months ago, 2:01:15)
 14. Day 3 - Probabilistic Machine Learning From Bayesian Linear Regression to Gaussian Processes (143 views, 6 months ago, 42:31)
 15. Day 4 - Ira Shokar - 10 minute quick fire science talk (69 views, 6 months ago, 9:26)
 16. Day 4 - Renato Barghiere - 10 minute quick fire science talk (81 views, 6 months ago, 7:44)
 17. Day 4 - Advanced GPU programming optimisation - Paul Richmond (456 views, 6 months ago, 1:04:35)
 18. Day 4 - Introduction to Machine Learning with Pytorch Teaching - Part 2 of 2 - CNNs, exercises, ... (262 views, 6 months ago, 2:24:27)
 19. Day 4 - Communicating Science: You Can’t Win, But You’ve Got To Play - Joe Palca (111 views, 6 months ago, 33:30)
 20. Day 4 - Hugging Face platform - Ben Orchard (272 views, 6 months ago, 1:25:24)
 21. Day 4 - Kazem Ardaneh - 10 minute quick fire science talk (103 views, 6 months ago, 8:00)
Interesting videos involving AI
Jon Oleksiuk - Does God Exist? AI debates Atheist vs. Believer
