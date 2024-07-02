# Compare types of Joins

## Inner Joins
INNER JOIN returns rows matching on a specified column that exists in more than one table.

It only returns the rows where there is a match, but like other types of joins, it returns all specified columns from all joined tables. For example, if the query joins two tables with SELECT *, all columns in both of the tables are returned.

```
SELECT *

FROM employees

INNER JOIN machines ON employees.device_id = machines.device_id;
```
