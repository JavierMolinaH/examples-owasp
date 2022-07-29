# CWE-73

¿Cuál es la vulnerabilidad?

```java
String rName = request.getParameter("reportName");
File rFile = new File("/usr/local/apfr/reports/" + rName);
...
rFile.delete();
```
