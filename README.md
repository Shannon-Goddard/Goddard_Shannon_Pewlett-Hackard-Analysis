# Goddard_Shannon_Pewlett-Hackard-Analysis
## Project Overview
In Pewlett-Hackard-Analysis, we learned about data modeling, engineering, and analysis. Applying our knowledge of DataFrames and tabular data, we created entity relationship diagrams (ERDs), import data into a database, troubleshot common errors, and created queries that use data to answer questions using SQL techniques.

## Resources
- **Data Source:** departments.csv, dept_emp.csv, dept_manager.csv, employees.csv, salaries.csv, titles.csv
- **Software:** Postgres, pgAdmin

## Summary
In this module, we: 
- Designed an ERD that applied to the data.
- Created and used a SQL database.
- Imported and exported large CSV datasets into pgAdmin.
- Practiced using different joins to create new tables in pgAdmin.
- Wrote basic- to intermediate-level SQL statements.

## Challenge Overview
In this challenge, we used advanced queries and joins to create a list of candidates for the mentorship program. To complete this task, we used our knowledge of aliasing, filtering, and creating new tables.

### Objectives
- Use an ERD to understand relationships between SQL tables.
- Create new tables in pgAdmin by using different joins.
- Write basic- to intermediate-level SQL statements.
- Export new tables to a CSV file.

## Challenge Summary
To create the new list of potential mentors, we created a query that returns a list of current employees eligible for retirement, as well as their most recent titles. To get the final list with the recent titles, we partition the data so that each employee is only included on the list once. In addition, we performed a query that shows how many current employees of each title are presently eligible for retirement. The final query returns the potential mentor’s employee number, first and last name, their title, birth date and employment dates.

<img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20code/number_of_titles_retiring.png"
     alt="Home Screen"
     style="float: left; margin-right: 10px;"
     width="300"/> <img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20output/number_of_titles_excel.png"
     alt="Home Screen"
     style="float: left; margin-right: 40px;"
     width="500"/>
     
     
     
 <img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20code/only_the_most_recent_titles.png"
     alt="Home Screen"
     style="float: left; margin-right: 10px;"
     width="300"/> <img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20output/only_the_most_recent_excel.png"
     alt="Home Screen"
     style="float: left; margin-right: 40px;"
     width="500"/>    
     
     
     

 <img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20code/whos_ready_for_a_mentor.png"
     alt="Home Screen"
     style="float: left; margin-right: 10px;"
     width="300"/> <img src="https://github.com/Shannon-Goddard/Goddard_Shannon_Pewlett-Hackard-Analysis/blob/master/CHALLENGE/pics%20of%20output/whos_ready_for_a_mentor_excel.png"
     alt="Home Screen"
     style="float: left; margin-right: 40px;"
     width="500"/>




