
List all table from dataset
```sql
SELECT *
FROM {your_dataset}.INFORMATION_SCHEMA.TABLES
ORDER BY table_name;
```


List columns name 
```sql
SELECT 
    *
FROM {your_dataset}.INFORMATION_SCHEMA.COLUMNS
WHERE table_name = {table_name}
```
