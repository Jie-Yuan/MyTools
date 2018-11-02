#`%[(name)][flags][width].[precision]`

## 1. 字符串格式化
```python
'%.2f' % 0.11111
'{:.2f}'.format(0.11111)
```

## 2. Decimal
  - 1. 可以传递给Decimal整型或者字符串参数，但不能是浮点数据，因为浮点数据本身就不准确。

  - 2. Decimal还可以用来限定数据的总位数。
```python
from decimal import Decimal
Decimal('5.123').quantize(Decimal('0.00'))
```

## 3. np.set_printoptions(3)


---
http://www.runoob.com/python/att-string-format.html
