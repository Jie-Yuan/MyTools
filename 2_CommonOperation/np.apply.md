```python
# 类似pandas里的apply
def myfunc(a, b):
    "Return a-b if a>b, otherwise return a+b"
    if a > b:
        return a - b
    else:
        return a + b

vfunc = np.vectorize(myfunc)
vfunc([1, 2, 3, 4], 2)
```
