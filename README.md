# lambda函数 
匿名函数，不用思考名字。函数的便携式，一行流代码。形式：lambda x(输入数)，可多个 : x*x（返回值且是函数运行模式）。
# 生成器
## 保留函数内的局部变量的数据。yield x。就是保留每次执行x的数据，并且下次调用函数从他的下一句代码开始。x不会被重置。
```
def counter():
    i=0
    while i <= 5:
    yield i
    i+=1
for i in counter():
    print(i)
```
## 生成器第二个方法，循环语句加括号赋值，得到生成器对象，叫生成器表达式
```
t = (i**2 for i in range(10))
for i in t:
  print(i)
```

