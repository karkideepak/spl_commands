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

### BETWEEN
```
SELECT *
FROM mytable
WHERE mycolumn
BETWEEN 1 AND 5
```
Example: source=mytable 
  mycolumn>=1 mycolumn<=5

### Group By
```
SELECT mycolumn, avg(mycolumn)
FROM mytable
WHERE mycolumn=value
GROUP BY mycolumn
```
Example: source=mytable mycolumn=value
| STATS avg(mycolumn) BY mycolumn
| FIELDS mycolumn, avg(mycolumn)

URL https://help.splunk.com/en/splunk-enterprise/search/spl-search-reference/10.2/quick-reference/splunk-spl-for-sql-users
