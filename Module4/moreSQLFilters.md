# More SQL Queries

## Common Data Types
- **String** : data consisting of an ordered sequence of characters
- **Numeric** : data consisting of numbers
- **Date and time** : data representing data and/or time

    example: 
    ```
    SELECT * 
    FROM login_attempts
    WHERE time > '18:00';
    ```
## Operators
- **BETWEEN** : an operator that filters for numbers and or dates within a range
    example:
    ```
    SELECT *
    FROM machines
    WHERE OS_patch_date 
    BETWEEN '2021-03-01' AND '2021-09-01';
    ```
