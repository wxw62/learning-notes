# Python 学习笔记

## 常用内建函数

| 函数 | 用途 |
|------|------|
| `enumerate(iterable, start=0)` | 遍历时同时拿到索引 |
| `zip(*iterables)` | 并行遍历多个可迭代对象 |
| `map(fn, iterable)` | 对每个元素应用函数 |
| `filter(pred, iterable)` | 按谓词过滤 |
| `functools.reduce(fn, iterable)` | 累积归约 |

## 小技巧

- 解包：`a, *rest = [1, 2, 3, 4]`
- 字典合并：`d = {**d1, **d2}`（Python 3.5+）
- 类型注解：`def f(x: int) -> str: ...`
- 列表推导带条件：`[x*2 for x in range(10) if x % 2 == 0]`

## 文件操作

```python
with open("data.txt", "r", encoding="utf-8") as f:
    for line in f:
        print(line.strip())
```
