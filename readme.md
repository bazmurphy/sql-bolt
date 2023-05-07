# SQL Bolt

https://sqlbolt.com/

## 1. SELECT queries 101

### 1.1

```sql
SELECT title FROM movies;
```

### 1.2

```sql
SELECT director FROM movies;
```

### 1.3

```sql
SELECT title, director FROM movies;
```

### 1.4

```sql
SELECT title, year FROM movies;
```

### 1.5

```sql
SELECT * FROM movies;
```

## 2. Queries with constraints (Pt.1)

### 2.1

```sql
SELECT title
FROM movies
WHERE id = 6;
```

### 2.2

```sql
SELECT title
FROM movies
WHERE year
BETWEEN 2000 AND 2010;
```

### 2.3

```sql
SELECT title
FROM movies
WHERE year
NOT BETWEEN 2000 AND 2010;
```

### 2.4

```sql
SELECT title, year
FROM movies
WHERE year
LIMIT 5;
```

## 3. Queries with constraints (Pt.2)

### 3.1

```sql
SELECT title
FROM movies
WHERE title
LIKE "Toy Story%";
```

### 3.2

```sql
SELECT title
FROM movies
WHERE director
LIKE "John Lasseter";
```

### 3.3

```sql
SELECT title
FROM movies
WHERE director
NOT LIKE "John Lasseter";
```

### 3.4

```sql
SELECT title
FROM movies
WHERE title
LIKE "WALL-%";
```

## 4. Filtering and sorting Query results

### 4.1

```sql
SELECT DISTINCT director
FROM movies
ORDER BY director ASC;
```

### 4.2

```sql
SELECT title, year
FROM movies
ORDER BY year DESC
LIMIT 4;
```

### 4.3

```sql
SELECT title, year
FROM movies
ORDER BY title ASC, year ASC
LIMIT 5;
```

### 4.4

```sql
SELECT title, year
FROM movies
ORDER BY title ASC, year ASC
LIMIT 5 OFFSET 5;
```

## 5. Review: Simple SELECT Queries

### 5.1

```sql
SELECT city, country, population
FROM north_american_cities
WHERE country = 'Canada';
```

### 5.2

```sql
SELECT city, country, latitude
FROM north_american_cities
WHERE country = 'United States'
ORDER BY latitude DESC;
```

### 5.3

```sql
SELECT city, country, longitude
FROM north_american_cities
WHERE longitude < -87.629798
ORDER BY longitude ASC;
```

### 5.4

```sql
SELECT city, country, population
FROM north_american_cities
WHERE country = 'Mexico'
ORDER BY population DESC
LIMIT 2;
```

### 5.5

```sql
SELECT city, country, population
FROM north_american_cities
WHERE country = 'United States'
ORDER BY population DESC
LIMIT 2 OFFSET 2;
```
