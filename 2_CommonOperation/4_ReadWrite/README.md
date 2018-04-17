- all
```python
def read(file):
    with open(file) as f:
        return f.read()

def write(text, file, overwrite=True):
    if overwrite:
        with open(file, 'w') as f:
            f.write(text)
    else:
        with open(file, 'a') as f:
            f.write(text)
```

- by line
```python
```
