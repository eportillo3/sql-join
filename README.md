<h1>Complete a SQL join</h1>


<h2>Description</h2>
In this lab activity, you’ll use SQL joins to connect separate tables and retrieve needed information.

<h2>Environments Used </h2>

- <b>MariaDB shell</b>

<h2>Scenario:</h2>

In this scenario, you’ll investigate a recent security incident that compromised some machines.

You are responsible for getting the required information from the database for the investigation.

Here’s how you’ll do this task: 

- First, you’ll use an inner join to identify which employees are using which machines.

- Second, you’ll use left and right joins to find machines that do not belong to any specific user and users who do not have any specific machine assigned to them.

- Finally, you’ll use an inner join to list all login attempts made by all employees.

<h2>Tutorial walk-through:</h2>

<h3>Task 1. Match employees to their machines</h3>

First, you must identify which employees are using which machines. The data is located in the machines and employees tables.

You must use a SQL inner join to return the records you need based on a connecting column. In the scenario, both tables include the device_id column, which you’ll use to perform the join.

1. Run the following query to retrieve all records from the machines table:

<img src="https://i.imgur.com/GFbyBzg.png" height="80%" width="80%"/>

You’ll note that this query is not sufficient to perform the join and retrieve the information you need.

2. Complete the query to perform an inner join between the machines and employees tables on the device_id column. Replace X and Y with this column name:

<img src="https://i.imgur.com/2DQgKF4.png" height="80%" width="80%"/>


<h3>Task 2. Return more data</h3>

You now must return the information on all machines and the employees who have machines. Next, you must do the reverse and retrieve the information of all employees and any machines that are assigned to them.

To achieve this, you’ll complete a left join and a right join on the employees and machines tables. The results will include all records from one or the other table. You must link these tables using the common device_id column.

1. Run the following SQL query to connect the machines and employees tables through a left join. You must replace the keyword X in the query:

<img src="https://i.imgur.com/IEgvNBt.png" height="80%" width="80%"/>

2. Run the following SQL query to connect the machines and employees tables through a right join. You must replace the keyword X in the query to solve the problem:

<img src="https://i.imgur.com/N7SIJB7.png" height="80%" width="80%"/>


<h3>Task 3. Retrieve login attempt data</h3>

To continue investigating the security incident, you must retrieve the information on all employees who have made login attempts. To achieve this, you’ll perform an inner join on the employees and log_in_attempts tables, linking them on the common username column.

- Run the following SQL query to perform an inner join on the employees and log_in_attempts tables. Replace X with the name of the right table. Then replace Y and Z with the name of the column that connects the two tables:

<img src="https://i.imgur.com/sjT1nJX.png" height="80%" width="80%"/>



<h2>Conclusion</h2>

You have completed this activity and should be able to use joins to combine data from multiple tables in a database.

You now have practical experience in using

- INNER JOIN
- LEFT JOIN
- RIGHT JOIN

  
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
