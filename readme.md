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

### 2.1

```sql
SELECT title
FROM movies
WHERE year
BETWEEN 2000 AND 2010;
```

### 2.1

```sql
SELECT title
FROM movies
WHERE year
NOT BETWEEN 2000 AND 2010;
```

### 2.1

```sql
SELECT title, year
FROM movies
WHERE year
LIMIT 5;
```
