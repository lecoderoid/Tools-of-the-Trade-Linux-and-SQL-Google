# Join Tables in SQL

**Inner Join** : returns rows matching on a specified column that exists in more than one table

example
```
SELECT username, office, operating_system
FROM employees
INNER JOIN machines ON employees.employee_id=machines.employee_id;
```
