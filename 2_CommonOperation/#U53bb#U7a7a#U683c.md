- 字符串去空格
    - 去左右空格
    ```
    a = ' hello world '
    a.strip()
    a.lstrip()
    a.rstrip()
    ```
    - 替换法
    ```
    a.replace(' ', '')
    ```
    - 重组法
    ```
    ''.join(a.split())
    ```
    - 正则法
    ```
    re.sub(' ', '', a)
    re.compile(' ').sub('', a)
    ```
---

- 元组/列表去空格
```
filter(lambda x: x!=' ', ['a', ' ', 'b'])
```
