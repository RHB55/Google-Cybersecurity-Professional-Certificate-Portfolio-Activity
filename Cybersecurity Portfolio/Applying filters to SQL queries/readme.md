# Project Overview

As a security professional at a large organization. Part of my job is to investigate security issues to help keep the system secure. recently I discovere some potential security issues that involve login attempts and employee machines.

My task is to examine the organization’s data in their employees and log_in_attempts tables. I need to use SQL filters to retrieve records from different datasets and investigate the potential security issues.

### Procedures followed
in this project i used SQL filters to retrieve records from different datasets and investigate the potential security issues.**using the following steps:**

**1. Retrieve after hours failed login attempts**

 To investigate this, I query the log_in_attempts table and review after hours login activity. I use filters in SQL to create a query that identifies all failed login attempts that occurred after 18:00.  The success I use a value FALSE in my query to identify failed login attempts.

 **2. Retrieve login attempts on specific dates**

A suspicious event occurred on 2022-05-09.To investigate this event, I review all login attempts which occurred on this day and the day before. I use filters in SQL to create a query that identifies all login attempts that occurred on 2022-05-09 or 2022-05-08 from **login_date column**
 

