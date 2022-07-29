# CWE-89

¿Cuál es la vulnerabilidad?

```python
@app.route('/user')
def downloadFile (username: str) -> Dict[str, object]:
    query = f'SELECT * FROM items WHERE owner = {userName}'
    response = SqlDataAdapter(query, conn)
    return ok_response(response)
```
