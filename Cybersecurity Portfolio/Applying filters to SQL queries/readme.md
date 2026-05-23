# Project Overview

As a security professional at a large organization. Part of my job is to investigate security issues to help keep the system secure. recently I discovere some potential security issues that involve login attempts and employee machines.

My task is to examine the organization’s data in their employees and **log_in_attempts** tables. I need to use SQL filters to retrieve records from different datasets and investigate the potential security issues.

### Procedures followed
in this project i used SQL filters to retrieve records from different datasets and investigate the potential security issues.**using the following steps:**

**1. Retrieve after hours failed login attempts**

To investigate this, I query the **log_in_attempts** table and review after hours login activity. I use filters in SQL to create a query that identifies all failed login attempts that occurred after 18:00   .The **success** column contains a value of 0 when a login attempt failedI I use a value **FALSE** in my query to identify failed login attempts.

```
SELECT *
FROM log_in_attempts
WHERE login_time > '18:00' AND success = FALSE;
```
 **2. Retrieve login attempts on specific dates**

A suspicious event occurred on 2022-05-09.To investigate this event, I review all login attempts which occurred on this day and the day before. I use filters in SQL to create a query that identifies all login attempts that occurred on 2022-05-09 or 2022-05-08 from **login_date** column.

```
WHERE login_date = '2022-05-09' OR login_date = '2022-05-08';
```

**3. Retrieve login attempts that occurred outside of Mexico**

To investigate login attempts that occurred outside of Mexico. I  use filters in SQL to create a query that identifies all login attempts that occurred outside of Mexico.
When referring to Mexico, the country column contains values of both MEX and MEXICO,I use the **LIKE** keyword with **%** to make sure my query reflects this.
```
WHERE NOT country LIKE 'MEX%';
 ```
**4. Retrieve employees in Marketing**

The team wants to perform security updates on specific employee machines in the Marketing department. my responsiblity is getting information on these employee machines and I query the employees table. I use filters in SQL to create a query that identifies all employees in the Marketing department for all offices in the East building.I use the **LIKE** keyword with **%** to filter for the East building

```
WHERE department = 'Marketing' AND office LIKE 'East%';
```

**5.  Retrieve employees in Finance or Sales**

My team now needs to perform a different security update on machines for **employees** in the Sales and Finance departments. I use filters in SQL to create a query that identifies all employees in the Sales or Finance departments in the **employees** table. 
```
SELECT *
FROM employees
WHERE department = 'Finance' OR department = 'Sales'; 
```
