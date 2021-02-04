
Convert string datetime to UNIX timestamp
````python
from datetime import datetime 

last_execution_date = "2020-01-01 00:00:00"
int(datetime.strptime(last_execution_date, "%Y-%m-%d %H:%M:%S").timestamp()*1e3)
````


Convert UNIX timestamp to datetime
````python
from datetime import datetime 

unix_timestamp = 1577833200000
datetime.fromtimestamp((last_execution_date_sec-1)/1e3)
````