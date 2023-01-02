# OFFSET
It refers to the number of pieces of data to be offset, that is the result will skip a specific number of results.
```
SELECT * FROM `new_schema`.`users` LIMIT 3 OFFSET 1;
```
# Multi-column Sorting
In addition to sorting by a single column, the result can also be sorted by multiple columns. When two records have the same value in the first column, they will be sorted according to the values in the second column, for example:
```
SELECT * FROM `new_schema`.`users` ORDER BY age DESC, height DESC;
```
# CONCAT
word combination function that is commonly seen. In SQL, you can use CONCAT() to manipulate the presented data:
```
SELECT CONCAT(`id`, '-', `name`) AS `identification`, `age` FROM `new_schema`.`users`;
```
Result:

|identification	|age

1-John	  40
2-May	  30
3-Tim	  25
4-Jay	  40
