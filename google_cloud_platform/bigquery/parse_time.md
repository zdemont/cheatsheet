
parse with timezone `YYYY-MM-DDTHH:MM:SS+HH:MM` like `2021-02-01T12:08:18+00:00`

```sql
SELECT
PARSE_TIMESTAMP('%Y-%m-%dT%H:%M:%S%Ez', '2021-02-01T12:08:18+00:00', 'Europe/Paris') AS report_provider_id, 

```


parse with fractional precision `YYYY-MM-DDTHH:MM:SS.NNNN` like `2021-02-01T12:08:18.5355435`

```sql
SELECT
PARSE_TIMESTAMP('%Y-%m-%dT%H:%M:%E*S', '2021-02-01T12:08:18.106298', 'Europe/Paris') AS report_provider_id, 

```

parse with fractional precision and timezone `YYYY-MM-DD HH:MM:SS.NNNN+00:00` like `2021-02-01 09:31:18.648752+00:00`

```sql
SELECT
PARSE_TIMESTAMP('%Y-%m-%d %H:%M:%E*S%Z', '2021-02-01 09:31:18.648752+00:00', 'Europe/Paris') AS report_provider_id, 

```