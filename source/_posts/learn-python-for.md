---
title: '学习 Python 的 for 循环'
date: 2021-02-19 21:30:09
tags: ['python', 'for']
---

今天复习了 Python 的 `for` 循环，第一个例子是**遍历列表**：

```py
majicians = ['alice', 'david', 'carolina']
for majician in majicians:
    print(f'{majician.title()}, that was a greate trick!')
    print(f"I can't wait to see your next trick, {majician.title()}\n")
```

运行结果：

```
Alice, that was a greate trick!
I can't wait to see your next trick, Alice

David, that was a greate trick!
I can't wait to see your next trick, David

Carolina, that was a greate trick!
I can't wait to see your next trick, Carolina

```

第二个例子是在**创建数值列表**：

```py
squares = []
for i in range(1, 6):
    squares.append(i ** 2)
print(squares)
```

运行结果：

```
[1, 4, 9, 16, 25]
```

第三个例子是**列表解析**（将 `for` 循环和创建新元素的代码合并成一行，并自动附加新元素）：

```py
# [1, 2, 3, 4, 5] -> [1, 4, 9, 16, 25]
squares = [i ** 2 for i in range(1, 6)] # [1, 2, 3, 4, 5]
print(squares)
```

运行结果：

```
[1, 4, 9, 16, 25]
```

第四个例子是**切片**：

```py
a = [3, 6, 8, 1, 7, 2, 4, 9]
b = a[2:5] # [8, 1, 7, 2]
for i in b:
    print(i)
```

运行结果：

```
8
1
7
2
```

![learn-python-for](2021/02/19/learn-python-for/learn-python-for.jpg)