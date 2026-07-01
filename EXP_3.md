### <center>Exercise 3</center>

### 1.Find all the Toy Story movies
~~~sql
SELECT * FROM movies
WHERE title like "toy story%";
~~~

### 2.Find all the movies directed by John Lasseter
~~~sql
SELECT * FROM movies
WHERE director like "john lasseter";
~~~

### 3.Find all the movies (and director) not directed by John Lasseter
~~~sql
SELECT * FROM movies
WHERE director not like "john lasseter";
~~~
### 4.Find all the WALL-* movies
~~~sql
SELECT * FROM movies
WHERE title like "wall%";
~~~