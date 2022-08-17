# Pewlett-Hackard-Analysis
With a database of six human resources csv files, we create an ERD as a reference to better understand the relationships within our data. We created different tables to narrow the employee data and be able to get the number of employees per department that are retiring according to certain parameters. Additionally, we created another table with the potential mentors of new hires. 

### Folders/Files

Queries folder - "Employee_Database_challenge.sql"

Data folder - "retirement_titles.csv", "unique_titles.csv","retiring_titles.csv","mentorship_eligibility.csv"

## Results

Three tables and csv files were created for getting the needed data. 

### The retirement titles table

For getting the retiring titles table we created two previous tables: "retirement titles" and "unique titles". In the first one, we joined the employees with the titles data. We filtered by the birthday column between 1952-01-01 and 1955-12-31, and at the end, we ordered in ascending order by the emp_no. In the unique table, we took the data from the retirement titles table and we filtered the data to get only the active employees. 

Finally, we created the retiring_titles file grouping by title and counted the number of employees in the unique_titles table. This summary table allows us to understand the number of new hires that are going to be needed and to show the importance of the mentoring program before people start to retire. 

!["retiring_titles"](https://github.com/DylanMontemayor/Pewlett-Hackard-Analysis/blob/main/Resources/retiring_titles.png)

### The mentorship eligibility table

For this table, we joined three files, we filtered the data by birth date and ordered by the employee number. This table will allow us to ask these employees if they want to be part of the mentoring program for new hires before retiring. 

!["mentorship"](https://github.com/DylanMontemayor/Pewlett-Hackard-Analysis/blob/main/Resources/mentorship.png)

## Summary

In this project, we were able to create and use a schema as a reference for our data base. Then, we create new csv files and tables using SQL in postgreSQL that we joined and narrowed to get the data we needed. As a result, we have the necessary information to present the new hires that will be required and get the people that is retiring so we can ask them if they want to join the mentoring program.
