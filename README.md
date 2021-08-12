# 9 SQL Homework


## Rice University Data Analytics and Visualization Boot Camp 2020


This repository contains the following scenario:

## Employee Database: A Mystery in Two Parts

In this repository, the major task is a research project on employees of a corporation from the 1980s and 1990s. All that remain of the database of employees from that period are six CSV files.

We will design the tables to hold data in the CSVs, import the CSVs into a SQL database (Postgres), and answer questions about the data. The two major tasks are:

1. Data Engineering / Data Modeling

3. Data Analysis

#### Data Modeling

Inspect the CSVs and sketch out an ERD of the tables. We use the [Quick Database Diagrams](https://app.quickdatabasediagrams.com/#/).

![ERD.png](EmployeeSQL/ERD.png)

#### Data Engineering

* Create a table schema for each of the six CSV files.

  * For the primary keys check to see if the column is unique, otherwise create a composite key. Which takes to primary keys in order to uniquely identify a row.
  * Create tables in the correct order to handle foreign keys.

* Import each CSV file into the corresponding SQL table. **Note** be sure to import the data in the same order that the tables were created and account for the headers when importing to avoid errors.

#### Data Analysis

1. List the following details of each employee: employee number, last name, first name, sex, and salary. 
![query_1.png](EmployeeSQL/query_1.png)

2. List first name, last name, and hire date for employees who were hired in 1986. 

![query_2.png](EmployeeSQL/query_2.png)

3. List the manager of each department with the following information: department number, department name, the manager's employee number, last name, first name. 

![query_3.png](EmployeeSQL/query_3.png)

4. List the department of each employee with the following information: employee number, last name, first name, and department name. 

![query_4.png](EmployeeSQL/query_4.png)

5. List first name, last name, and sex for employees whose first name is "Hercules" and last names begin with "B." 

![query_5.png](EmployeeSQL/query_5.png)

6. List all employees in the Sales department, including their employee number, last name, first name, and department name. 

![query_6.png](EmployeeSQL/query_6.png)

7. List all employees in the Sales and Development departments, including their employee number, last name, first name, and department name. 

![query_7.png](EmployeeSQL/query_7.png)

8. In descending order, list the frequency count of employee last names, i.e., how many employees share each last name. 

![query_8.png](EmployeeSQL/query_8.png)

## Bonus

As you examine the data, you are overcome with a creeping suspicion that the dataset is fake. You surmise that your boss handed you spurious data in order to test the data engineering skills of a new employee. To confirm your hunch, you decide to take the following steps to generate a visualization of the data, with which you will confront your boss:

1. Import the SQL database into Pandas.

2. Create a [histogram](EmployeeSQL/Salary_Distribution.png) to visualize the most common salary ranges for employees.

![Salary_Distribution.png](EmployeeSQL/Salary_Distribution.png)

3. Create a [bar chart](EmployeeSQL/Average_Salary_Title.png) of average salary by title.

![Average_Salary_Title.png](EmployeeSQL/Average_Salary_Title.png)

## Epilogue

Evidence in hand, you march into your boss's office and present the visualization. With a sly grin, your boss thanks you for your work. On your way out of the office, you hear the words, "Search your ID number." You look down at your badge to see that your employee ID number is 499942.

## Submission

* [Create an image file of your ERD](EmployeeSQL/ERD.png)

* [Create a `.sql` file of your table schemata.](EmployeeSQL/schema.sql)

* [Create a `.sql` file of your queries.](EmployeeSQL/query.sql)

* [Create a Jupyter Notebook of the bonus analysis.](EmployeeSQL/SQL_Bonus.ipynb)