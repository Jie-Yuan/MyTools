<h1 align = "center">:rocket: 常用操作 :facepunch:</h1>

---
改善 Python 程序的 91 个建议
https://zhuanlan.zhihu.com/p/26155739
---
- 取整数各位置数
```python
f = lambda x: np.floor(x / np.array([10**i for i in range(len(str(x)))])) % 10
f(123456789)

array([ 9.,  8.,  7.,  6.,  5.,  4.,  3.,  2.,  1.])
```
- exec 被当成一个函数 ，可以通过以下的方法来进行将字符串变成变量的名字进行赋值
```python
x='myVar'
exec("%s = %s" % (x, [1,2,3]))
print(myVar)

[1, 2, 3]
```

- print(value, ..., sep=' ', end='\n', file=sys.stdout)
    - file默认打印到终端
    ```python
    print(*range(10), sep=' ', end='\n', file=sys.stdout)
    
    0 1 2 3 4 5 6 7 8 9
    ```
    - file打印到指定文件
    ```python
    f = open('log.txt', 'w')
    print(*range(10), sep=' ', end='\n', file=f)
    f.close()
    ```
    - shell
    ```
    python test.py > log.txt # 覆盖
    python test.py >> log.txt # 追加
    ```

---

- df.pipe

- df.groupby('x')['xx'].shift(1): x组内xx下滑Lag一位
- pd.crosstab(data.Pclass,data.Survived,margins=True).style.background_gradient(cmap='summer_r')
- str.isdigit
```python
str.isdigit('1')
str.isdigit('1s')
```
- func2str
```
#获取函数名
ls = ['a', max, 'b']
list(map(lambda x: x.__name__ if type(x) != str else x, ls))

['a', 'max', 'b']
```

- coalesce: 返回第一个非空的值
```
df['c'] = np.where(df["a"].isnull, df["b"], df["a"] )
df['c'] = df.a.combine_first(df.b)
```
