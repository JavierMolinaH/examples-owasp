
# CWE-23

Dadas las siguientes url's

* http://example.com.br/get-files.jsp?file=report.pdf
* http://example.com.br/get-page.php?home=aaa.html
* http://example.com.br/some-page.asp?page=index.html

Si se hace una petición agregando el siguiente texto en el valor del query param

```txt
/etc/passwd
```

```python

@app.route('/download')
def downloadFile (path: str) -> Dict[str, object]:
    return send_file(path, as_attachment=True)

```
