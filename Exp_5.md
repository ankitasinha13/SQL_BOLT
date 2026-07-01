### <center>Experiment 5</center>
### 1.List all the Canadian cities and their populations
~~~sql
SELECT  city, Population FROM north_american_cities
WHERE country like 'canada';
~~~

### 2.Order all the cities in the United States by their latitude from north to south
~~~sql
SELECT city, latitude FROM north_american_cities
WHERE country = "United States"
ORDER BY latitude DESC;
~~~

### 3.List all the cities west of Chicago, ordered from west to east
~~~sql
SELECT city, longitude FROM north_american_cities
WHERE longitude < -87.629798
ORDER BY longitude ASC;
~~~

### 4.List the two largest cities in Mexico (by population)
~~~sql
SELECT city, population FROM north_american_cities
WHERE country LIKE "Mexico"
ORDER BY population DESC
LIMIT 2;
~~~

### 5.List the third and fourth largest cities (by population) in the United States and their population
~~~sql
SELECT city, population FROM north_american_cities
WHERE country LIKE 'United States'
ORDER BY population DESC
LIMIT 2 OFFSET 2;
~~~