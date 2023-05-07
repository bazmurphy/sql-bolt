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

## 3. Queries with constraints (Pt.1)

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
