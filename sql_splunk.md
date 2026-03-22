### SELECT *
```
SELECT *
FROM mytable
```
example: source=mytable

### WHERE
```
SELECT *
FROM mytable
WHERE mycolumn=5
```
Example: source=mytable mycolumn=5

### AND/OR	

```
SELECT *
FROM mytable
WHERE (mycolumn1="true" 
  OR mycolumn2="red") 
AND mycolumn3="blue"
```
Example:
source=mytable
AND (mycolumn1="true" 
  OR mycolumn2="red")
AND mycolumn3="blue"

