# FinalDB

## Database Model
![DataBase Model](/images/database.png)

## Tables creation
![Tables](/images/birthdaytable.png)

![Tables](/images/employeestable.png)

## Queries and description

1. select * from employees order by first_name asc;
2. 
*This query will show the data from employees table by first names in ascending order*

2.select * from birthdays order by birthdate asc;

*Will show the birthdates from birthdays table in ascending order*

3.select * from birthdays where age between 23 and 25;

*Will show those whose age is between 23 and 25 from birthdays table*

4.select * from employees where first_name= 'j%';

*Will show those whos name starts with a j from employees table*

5.select * from employees where employee_id= '4' or employee_id= '5';

*Will show employee who is number 4 or 5 on the list in employees table*

6.delete from employees where last_name= 'barron';
select * from employees;

*Deletes a row of data from employees table in this case eduardo barron is deleted*

7.update birthdays set employee_name= 'Marvin' where employee_name= 'eduardo';
select * from birthdays;

*Updates data in a table in this case eduardo will be cahnged into Marvin in the birthdays table*

8.select * from employees where employee_id = (select employee_id from employees where first_name= 'jessica');

*Will get the name jessica from the employees table and show the id of the employee*

9.select count(*) from employees;

*Shows count of how many employees there are in the employees table*

10.select avg(age) from birthdays;

*Shows the average age in the birthdays table, in this case 21*

11.select * from employees left join birthdays on employees.first_name = birthdays.employee_name;

*Joins data from employees and birthdays table where its related*

12.select * from birthdays right join employees on birthdays.birthdate = employees.hire_date;

*returns all records from the right table (birthdays), and the matching records from the left table (employees)*

