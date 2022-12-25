# Mysql

## Login

Syntax:
```bash
mysql -h <host-ip> -u <username> -p <password>
```

Example (no pw):
```bash
mysql -h 10.129.46.63 -u root
```

## Get all databasees
```sql
SHOW DATABASES
```

## Get all tables in all databases
```sql
SELECT table_name
FROM INFORMATION_SCHEMA.TABLES
WHERE table_type = 'BASE TABLE'
```

## Get all tables in specific database
```sql
SELECT table_name
FROM information_schema.tables
WHERE table_type='BASE TABLE'
      AND table_schema = '<db name>'
```

## Get all values from a table
```sql
SELECT * FROM <db>.<table>
```
