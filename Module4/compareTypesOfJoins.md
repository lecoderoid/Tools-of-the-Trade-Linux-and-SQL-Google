# Compare types of Joins

## Inner Joins
INNER JOIN returns rows matching on a specified column that exists in more than one table.

It only returns the rows where there is a match, but like other types of joins, it returns all specified columns from all joined tables. For example, if the query joins two tables with SELECT *, all columns in both of the tables are returned.

```
SELECT *

FROM employees

INNER JOIN machines ON employees.device_id = machines.device_id;
```

## Outer joins
Outer joins expand what is returned from a join. Each type of outer join returns all rows from either one table or both tables.

### Left Joins 
When joining two tables, LEFT JOIN returns all the records of the first table, but only returns rows of the second table that match on a specified column.

```
SELECT *

FROM employees

LEFT JOIN machines ON employees.device_id = machines.device_id;
```

### Right Joins
When joining two tables, RIGHT JOIN returns all of the records of the second table, but only returns rows from the first table that match on a specified column.

```
SELECT *

FROM employees

RIGHT JOIN machines ON employees.device_id = machines.device_id;

```
Note:  You can use LEFT JOIN and RIGHT JOIN and return the exact same results if you use the tables in reverse order. The following RIGHT JOIN query returns the exact same result as the LEFT JOIN query demonstrated in the previous section:

```
SELECT *

FROM machines

RIGHT JOIN employees ON employees.device_id = machines.device_id;
```

### Full Outer Joins

FULL OUTER JOIN returns all records from both tables. You can think of it as a way of completely merging two tables.

```
SELECT *

FROM employees

FULL OUTER JOIN machines ON employees.device_id = machines.device_id;
```
