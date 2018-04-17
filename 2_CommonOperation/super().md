## [super(): 用于调用父类(超类)的一个方法][1]

```python
class Base(object):
    def __init__(self):
        print 'Base create'
 
class childA(Base):
    def __init__(self):
        print 'creat A ',
        Base.__init__(self)
 
# 使用super()继承时不用显式引用基类
class childB(Base):
    def __init__(self):
        print 'creat B ',
        super(childB, self).__init__()
```

---
[1]: http://www.runoob.com/python/python-func-super.html
