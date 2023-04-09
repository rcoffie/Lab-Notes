
# PostgreSQL

## SQL 
Structured Query Language, abbreviated as SQL, is a domain-specific language used in programming and designed for managing data held in a relational database management system

## PostgreSQL
PostgreSQL, also known as Postgres, is a free and open-source relational database management system emphasizing extensibility and SQL compliance.

### How to start a postgresql on ubuntu 
sudo service postgresql start 

```postgresql
  sudo service postgresql start 
```
    

### How to log on to psql using command line 

```postgresql
  sudo -u postgresql psql 
```

### How to connect to dataase 

```postgresql
  \c databasename 
```
### Connecting to database with a specific user 

```postgresql
  psql -h localhost -p 5432 -U bobby posts
```

### Command to get help 

```postgresql
  \?
```
### Command to list all the database in the system 

```postgresql
  \l
```

### Connecting to database from the command line 

```postgresql
  \c database_name
```

### Deleting database 

```postgresql
  DROP DATABASE database_name
```

### Creating table with Potgres 

```postgresql
  CREATE TABLE table_name (Column_name + data_type + contstraint if any )
```
### Example of creating table 

```postgresql
  CREATE TABLE person(
      id, int, 
      first_name VARCHAR(50),
      last_name VARCHAR(50),
      gender VARCHAR(50),
      date_of_birth TIMESTAMP,
  )
```
### Listing all tables in database 

```postgresql
  \d 
```
#### Describing table 

```postgresql
  \d table_name
```

### Inserting records into a table 
```postgresql
  INSERT INTO person(
      first_name, 
      last_name,
      gender,
      date_of_birth
  )VALUES 
  ('Anne', 'Smith','Female', DATE'1993-01-09', 'man@man.com');
```

### Switching user account 

```postgresql
  \c db_name user_name
```

### Using Select in POSTGRES 

### Getting all records from the table 
```postgresql
  SELECT * FROM table_name
```

### SELECT ACCORDING A SPECIFIC COLUMN 

```postgresql
  SELECT column_name FROM table_name;
```

### SELECTING MULTIPLE COLUMNS 

```postgresql
  SELECT * column1, column2, column3 FROM table_name;
```

### USING ORDER BY 

```postgresql
  SELECT * FROM table_name ORDER BY column_name;
```

Notes.
note this statemnet will be sorted by ascending  order 
you can also specify the order either by using ascending or decending order. 
you can also combine multiple columns when using ORDER BY

### Where clause and AND 

where clause allow us to filter the table base on conditions 

```postgresql
  SELECT * FROM table_name WHERE gender = "female";
```

### Adding and condition to the where cluase 

```postgresql
  SELECT * FROM table_name WHERE gender = "female" and country_of_birth = "china";
```

### USING OR statment in where cluase 

```postgresql
  SELECT * FROM table_name WHERE gender = 'female' AND (country_of_birth = 'china' OR country_of_birth='Poland' )
```