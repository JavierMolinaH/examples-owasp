# CWE-74

¿En dónde está la vulnerabilidad?

```php
$userName = $_POST["user"];
$command = 'ls -l /home/' . $userName;
system($command);
```
