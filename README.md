# Goddard_Shannon_Pewlett-Hackard-Analysis
## Project Overview
In Pewlett-Hackard-Analysis, we learned about data modeling, engineering, and analysis. Applying our knowledge of DataFrames and tabular data, we created entity relationship diagrams (ERDs), import data into a database, troubleshot common errors, and created queries that use data to answer questions using SQL techniques.

### Objectives 
- Design an ERD that applies to the data.
- Create and use a SQL database.
- Import and export large CSV datasets into pgAdmin.
- Practice using different joins to create new tables in pgAdmin.
- Write basic- to intermediate-level SQL statements.

## Resources
- **Data Source:** departments.csv, dept_emp.csv, dept_manager.csv, employees.csv, salaries.csv, titles.csv
- **Software:** Postgres, pgAdmin

## Summary
A **conceptual diagram** is an ERD in its simplest form. To create one, we only need two things: a table name and column headers.

**Logical diagrams** contain all of the same information that a conceptual diagram does, but the table is updated to include data types and primary keys.

**Physical diagrams** portray the physical relationship, or how the data is connected, between each table.
| col 1   | col 2   |
|---------|---------|
| <img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/EmployeeDB.png" width="400"> | <img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20output/ERD%20defined.png" width="200"> |

#<img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/EmployeeDB.png" width="400">
#<img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20output/ERD%20defined.png" width="200">

One benefit to building out each form of the diagram (conceptual, logical, and physical) is that it gives us more exposure to the data and its layout. When writing queries in SQL, data is organized into tables, as shown in the ERD. With the help of the diagram, we know the structure of the table: the amount of columns with their data types. The table can be, already, named. All we need to do is transfer over the same information.

## Challenge Overview
In this challenge, we used advanced queries and joins to create a list of candidates for the mentorship program. To complete this task, we used our knowledge of aliasing, filtering, and creating new tables.

### Objectives
- Use an ERD to understand relationships between SQL tables.
- Create new tables in pgAdmin by using different joins.
- Write basic- to intermediate-level SQL statements.
- Export new tables to a CSV file.

## Challenge Summary
 
<img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20code/number_of_titles_retiring.png"
     alt="Home Screen"
     style="float: left; margin-right: 10px;"
     width="310"/> <img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20output/number_of_titles_excel.png"
     alt="Home Screen"
     style="float: left; margin-right: 40px;"
     width="500"/>
     
**To create the new list of potential mentors, we created a query that returns a list of current employees eligible for retirement, as well as their most recent titles.**  
<br/>
<br/>
<br/>
<img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20code/only_the_most_recent_titles.png"
     alt="Home Screen"
     style="float: left; margin-right: 10px;"
     width="400"/> <img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20output/only_the_most_recent_excel.png"
     alt="Home Screen"
     style="float: left; margin-right: 40px;"
     width="332"/>    
     
**To get the final list with the recent titles, we partition the data so that each employee is only included on the list once. In addition, we performed a query that shows how many current employees of each title are presently eligible for retirement.**     
<br/>     
<br/>
<br/> 
<img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20code/whos_ready_for_a_mentor.png"
     alt="Home Screen"
     style="float: left; margin-right: 10px;"
     width="390"/> <img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20output/whos_ready_for_a_mentor_excel.png"
     alt="Home Screen"
     style="float: left; margin-right: 40px;"
     width="455"/>

**The final query returns the potential mentor’s employee number, first and last name, their title, birth date and employment dates.**
