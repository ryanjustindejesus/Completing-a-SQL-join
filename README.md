<h1>Completing a SQL join </h1>



<h2>Description</h2>
In this lab, I used INNER JOIN, LEFT JOIN, and RIGHT JOIN in SQL to retrieve information from two different tables. I used these different types of SQL joins to join data from separate machines, employees, and login attempts tables. I will be using the MariaDB shell to run SQL queries.
<br />


<h2>Practical experience gained in this Lab</h2>

- <b>INNER JOIN</b> 
- <b>LEFT JOIN</b>
- <b>RIGHT JOIN</b> 


<h2>Environments Used </h2>

- <b>Qwiklabs</b> 

<h2>Lab walk-through:</h2>

<h2>Task 1: Match employees to their machines </h2>
In thi task, I identified which employees are using which machines. The data is located in the machines and employees tables.
 <br/> <br />
(1) I used the command "SELECT * FROM machines INNER JOIN employees ON machines.device_id = emplyoees.device_id;" to perform an inner join between the machines and employees tables on the device.id column. 
<br/> <br/> <p align="center">
<img src="https://imgur.com/E7ivK9Y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 2: Return more data </h2>
In this task, I returned the information on all machines and the employees who have machines. Next, I reversed and retrieved the information of all employees and any machines that are assigned to them.
<br/> <br />
(1) First, I used the command "SELCT * FROM machines LEFT JOIN employees ON machines.device_id = employees.device_id;" to connect the machines and employees tables through a left join.
<br /> <br /> <p align="center">
<img src="https://imgur.com/F2wjsQ2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />
(2) Finally, I used the command "SELECT *FROM machines RIGHT JOIN employees ON machines.device_id = employees.device_id;" to connect the machines and employees tables through a right join.
<br /> <br /> <p align="center">
<img src="https://imgur.com/6zwmDUH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 3: Retrieve login attempt </h2>
In this task, I retrieved the information on all employees who have made login attempts. 
 <br/> <br/>
(1) I used the command "SELECT * FROM employees INNER JOIN log_in_attempts ON employees.username = log_in_attempts.username;" to perform an inner join on the employees and log_in_attempts tables.
<br/> <br/> <p align="center">
<img src="https://imgur.com/9jyhEP3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />
