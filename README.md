# Goddard_Shannon_Pewlett-Hackard-Analysis

#### Table of Contents

[Project Overview](#project-overview)  
[Resources](#resources)  
[Objectives](#objectives)  
[Summary](#summary)  
[Challenge Overview](#challenge-overview)  
[Challenge Summary](#challenge-summary)

## Project Overview
In Pewlett-Hackard-Analysis, we learned about data modeling, engineering, and analysis. Applying our knowledge of DataFrames and tabular data, we created entity relationship diagrams (ERDs), import data into a database, troubleshot common errors, and created queries that use data to answer questions using SQL techniques.

## Resources
The Pewlett-Hackard-Analysis module uses PostgreSQL which required pgAdmin to be installed. Visit the [PostgresSQL download website](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads)
 to initiate your download
  
- **Data Source:** [departments.csv](/Data/departments.csv), [dept_emp.csv](/Data/dept_emp.csv), [dept_manager.csv](/Data/dept_manager.csv), [employees.csv](/Data/employees.csv), [salaries.csv](/Data/salaries.csv), [titles.csv](/Data/titles.csv)
- **Software:** Postgres, pgAdmin  

For more about PostgreSQL, see:  
- The PostgreSQL documentation
 https://www.postgresql.org/docs/manuals/  
- The PostgreSQL tutorial
 https://www.tutorialspoint.com/postgresql/

## Objectives 
- Design an ERD that applies to the data.
- Create and use a SQL database.
- Import and export large CSV datasets into pgAdmin.
- Practice using different joins to create new tables in pgAdmin.
- Write basic- to intermediate-level SQL statements.

## Summary
There are several ways to refer to the map we created. It’s also called a flowchart, an entity relationship diagram, and a schema. We used all of these terms in this module, though “ERD” is the most specific. There are three forms of ERDs: conceptual, logical, and physical. Each one builds upon the other.  

A **conceptual diagram** is an ERD in its simplest form. To create one, we only need two things: a table name and column headers. **Logical diagrams** contain all of the same information that a conceptual diagram does, but the table is updated to include data types and primary keys. **Physical diagrams** portray the physical relationship, or how the data is connected, between each table.  

As we added more information to our tables, such as data types and keys, we advanced through the more complex diagrams.
![EmployeeDB](/CHALLENGE/pics%20of%20output/ERD%20defined.png, "Pewlett-Hackard-Analysis ERD")
<br/>
One benefit to building out each form of the diagram (conceptual, logical, and physical) is that it gives us more exposure to the data and its layout. When writing queries in SQL, data is organized into tables, as shown in the ERD. With the help of the diagram, we know the structure of the table: the amount of columns with their data types. The table can be, already, named. All we need to do is transfer over the same information.

## Challenge Overview
In this challenge, we used advanced queries and joins to create a list of candidates for the mentorship program. To complete this task, we used our knowledge of aliasing, filtering, and creating new tables.

## Objectives
- Use an ERD to understand relationships between SQL tables.
- Create new tables in pgAdmin by using different joins.
- Write basic- to intermediate-level SQL statements.
- Export new tables to a CSV file.

## Challenge Summary  
### Number of [titles] Retiring  
<img src="/CHALLENGE/pics%20of%20code/number_of_titles_retiring.png"
     alt="Home Screen"
     style="float: left; margin-right: 10px;"
     width="310"/> <img src="/CHALLENGE/pics%20of%20output/number_of_titles_excel.png"
     alt="Home Screen"
     style="float: left; margin-right: 40px;"
     width="500"/>  
<br/>    
We were instructed to create a new table using a RIGHT JOIN that contains Employee number, First and last name, Title, from_date, and Salary. Then, export the data as a CSV. To create the new list of potential mentors, we created a query that returns a list of current employees eligible for retirement, as well as their most recent titles.  
<br/>
<br/>
<br/>
### Only the Most Recent Titles
<img src="/CHALLENGE/pics%20of%20code/only_the_most_recent_titles.png"
     alt="Home Screen"
     style="float: left; margin-right: 10px;"
     width="400"/> <img src="/CHALLENGE/pics%20of%20output/only_the_most_recent_excel.png"
     alt="Home Screen"
     style="float: left; margin-right: 40px;"
     width="332"/>    
<br/>    
Here, we were instructed to list the frequency count of emplyee titles in decending order. To get the final list with the recent titles, we partition the data so that each employee is only included on the list once. In addition, we performed a query that shows how many current employees of each title are presently eligible for retirement.    
<br/>     
<br/>
<br/> 
### Who’s Ready for a Mentor?
<img src="/CHALLENGE/pics%20of%20code/whos_ready_for_a_mentor.png"
     alt="Home Screen"
     style="float: left; margin-right: 10px;"
     width="390"/> <img src="/CHALLENGE/pics%20of%20output/whos_ready_for_a_mentor_excel.png"
     alt="Home Screen"
     style="float: left; margin-right: 40px;"
     width="455"/>
<br/>
To find who's ready for a mentor, we created a new table. The birth date was set to be between January 1, 1965 and December 31, 1965. Also, we made sure only current employees were included in this list. The final query returns the potential mentor’s employee number, first and last name, their title, birth date and employment dates.
