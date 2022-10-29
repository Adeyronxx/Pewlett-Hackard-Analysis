# Pewlett-Hackard-Analysis
The goal of this project is;
1. To Identify employees eligible for participation in the Pewlett Hackard's Mentorship Program and,
2. To Identify the number of retiring employees for each Job Title.

# Resources
PostgreSQL, pgAdmin 4, Quick DBD
6 CSV files (Employees, Departments, Department managers, Salaries, Department Employees and Titles)

#ERD

![EmployeeDB](https://user-images.githubusercontent.com/109445468/198850777-bcceadad-c5fa-44e5-8361-e43d393a7d66.png)

This relational diagram shows the relationships betwwen our individial tables and helps us create a strong database.

# Analysis Results
  # Retiring Employees
To identify retiring employees we first had to create a new table with information from both the Employees and Job title tables, order by birth dates to get employees born within a certain period.

<img width="780" alt="Retiring employees" src="https://user-images.githubusercontent.com/109445468/198851387-3d83b7c7-650d-41e0-af45-fe4185863628.png">

We then filtered our results to show only employees who are currently employed only

![unique titles](https://user-images.githubusercontent.com/109445468/198851461-86207724-8bbb-4fc8-ac4b-33b440ddeafb.png)

Lastly, we used the count() function to determine the total number of employees that will retire for each job title

![retirees by job title](https://user-images.githubusercontent.com/109445468/198851515-0825193b-a87e-451e-92c9-020e4bddfc38.png)

From our analysis we can detrmine 2 details;

1. A total of 90,398 employees will retire.
2. Of the total employees retiring 57, 668 are senior positions.

  # Employees Eligible for the Mentorship Program 
  
To get the total number of eligible employees, we retrieved information from 3 of our datasets (Employees, Department Employees and Title). from this we were able to filter or results by employees born in the year 1965 to determine employees who qualify for Pewlett hackards Mentorship. These employees will retire partly into part-time roles and help mentor newly hired employees to fill the retired roles.

from our analysis we can determine;
1. A total number of 1,549 employees qualify for mentorship.
2. Comparing the number of employees that qualify for mentorship and employees retiring, we see a huge margin between both,

# SUMMARY
We are able to detrmine from our analysis that Pewlett Hackard will need more employees in their mentorship program to prepare the newly employed to fill senior positions in the company.
