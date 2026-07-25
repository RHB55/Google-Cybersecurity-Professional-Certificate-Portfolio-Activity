# Project Overview

As a security professional at a large organization. Part of my job is to investigate security issues to help keep the system secure. Recently I discovered some potential security issues that involve login attempts and employee machines.
My task is to examine the organization’s data in their employees and **log_in_attempts** tables. I need to use SQL filters to retrieve records from different datasets and investigate the potential security issues.

### Project Scope
in this project, I used SQL filters to retrieve records from different datasets and investigate the potential security issues, using the following steps:

**1. Retrieve after hours failed login attempts**

To investigate this, I queried the **log_in_attempts** table and reviewed after hours' login activity. I use filters in SQL to create a query that identifies all failed login attempts that occurred after 18:00 .The **success** column contains a value of 0 when a login attempt failedI I use a value **FALSE** in my query to identify failed login attempts.

```
SELECT *
FROM log_in_attempts
WHERE login_time > '18:00' AND success = FALSE;
```

**2. Retrieve login attempts on specific dates**

A suspicious event occurred on 2022-05-09.To investigate this event, I review all login attempts that occurred on this day and the day before. I use filters in SQL to create a query that identifies all login attempts that occurred on 2022-05-09 or 2022-05-08 from the **login_date** column.

```
WHERE login_date = '2022-05-09' OR login_date = '2022-05-08';
```

**3. Retrieve login attempts that occurred outside of Mexico**

To investigate login attempts that occurred outside of Mexico. I  use filters in SQL to create a query that identifies all login attempts that occurred outside of Mexico.
When referring to Mexico, the country column contains values of both MEX and Mexico;I use the **LIKE** keyword with **%** to make sure my query reflects this.

```
WHERE NOT country LIKE 'MEX%';
 ```
**4. Retrieve employees in Marketing**

The team wants to perform security updates on specific employee machines in the Marketing department. My responsibility is getting information on these employee machines and I queried the employees table. I use filters in SQL to create a query that identifies all employees in the Marketing department for all offices in the East building.I use the **LIKE** keyword with **%** to filter for the East building

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

**6. Retrieve all employees not in IT**

The employees who are in the Information Technology department already had this update, but employees in all other departments need it. In this case, I use filters in SQL to create a query which identifies all employees not in the IT department. 

```
WHERE NOT department = 'Information Technology';
```

### Summary

To investigate security issues related to login attempts to help keep the system secure. I used filters to SQL queries  for different tables. I used ```SELECT``` and ```FROM``` to create a query to  retrieve records from different datasets. Also, I used ```AND```, ```OR```, and ```NOT``` operators to filter for the specific information needed for each task. I also used ```LIKE``` and the percentage sign ```%``` wildcard to filter for patterns.

### Project Impact

This project enhances the organization’s security posture by enabling early detection of suspicious login activity, improving incident response, reducing breach risk, and providing data‑driven insights that strengthen authentication and access control policies.



> You will find the full project supported with screenshots in the in the **Applying filters to SQL queries** file inside the **Apply filters to SQL queries** folder.
