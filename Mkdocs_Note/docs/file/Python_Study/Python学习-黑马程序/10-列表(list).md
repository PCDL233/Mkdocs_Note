#### 1. 列表(list)



- 以 **` [ ] `** 作为标识
- 列表内每一个元素之间，用逗号隔开

##### 基本语法：

```python
# 字面量
[元素1,元素2,元素3......]

#定义变量
变量名称 = [元素1,元素2,元素3......]

# 定义空列表
变量名称 = []
变量名称 = list()
```

##### 示例：

```python
# 列表内全部是字符串
name_list = ['itheima', 'itcast', 'python']
print(name_list)

# 列表内每一个元素是不同的数据类型
my_list = ['itcast', 666, True]
print(my_list)

# 列表嵌套
num_list = [[1, 2], [3, 4], [9, 10]]
print(num_list)
```

##### 列表下标（索引）—正向

&emsp; 下标索引从 0  开始，依次递增。

```python
# 列表下标索引
# 语法：列表[标号]
name_list = ['itheima', 'itcast', 'python']
for x in range(3):
    print(x, name_list[x])
"""
输出：
0 itheima
1 itcast
2 python
"""
```

##### 列表下标（索引）—反向

&emsp; 反向索引，从 -1 开始，依次递减。

```python
# 语法：列表[标号]
name_list = ['itheima', 'itcast', 'python']
i = -1
while i > -4:
    print(i, name_list[i])
    i -= 1
"""
输出：
-1 python
-2 itcast
-3 itheima
"""
```

##### 嵌套列表的下标（索引)

```python
num_list = [[1, 2], [3, 4], [9, 10]]
print(num_list[0][0])
print(num_list[0][1])
print(num_list[1][0])
print(num_list[1][1])
"""
输出：
1
2
3
4
"""
```



****



#### 1.1 列表常用操作（方法)

- 插入元素
- 删除元素
- 清空列表
- 修改元素
- 统计元素个数

##### 1.1.1 查询

&emsp; 查找指定元素在 列表的下标，如果找不到，报错：ValueError 。

​	**语法：**

```python
列表.index(元素)
```

​	**示例：**

```python
name_list = ['itheima', 'itcast', 'python']
index = name_list.index("python")
print(index)
# 输出：2
```

##### 1.1.2 修改

​	**语法：**

```python
# 修改特定位置(索引)的元素值：
# 语法：
列表[下标] = 值
```

​	**示例：**

```python
name_list = ['itheima', 'itcast', 'python']
name_list[0] = "chen"
print(name_list[0])
# 输出：chen
```

##### 1.1.3 插入

​	**语法：**

```python
# 在指定的下标位置,插入指定的元素
# 语法：
列表.insert(下标,元素)
```

​	**示例：**

```python
my_list = [1, 2, 3, 4, 5]
my_list.insert(1, "chen")
for x in range(6):
    print(x, my_list[x])
"""
输出：
0 1
1 chen
2 2
3 3
4 4
5 5
"""
```

##### 1.1.4 追加单个元素

​	**语法：**

```python
# 将指定元素,追加到列表的尾部
# 语法：
列表.append(元素)
```

​	**示例：**

```python
my_list = [1, 2, 3, 4, 5]
my_list.append("python")
print(my_list)
# 输出：[1, 2, 3, 4, 5, 'python']
```

##### 1.1.5 追加多个元素

​	**语法：**

```python
# 将其他数据容器的内容取出,依次追加到列表的尾部
# 语法：
列表.extend(其他数据容器)
```

​	**示例：**

```python
my_list1 = [1, 2, 3]
my_list2 = [3, 4, 5]

my_list1.extend(my_list2)
print(my_list1)
# 输出：[1, 2, 3, 3, 4, 5]
```

##### 1.1.6 删除

​	**语法：**

```python
# 语法1：
del 列表[下标]

# 语法2：
列表.pop(下标)

# 语法3：
# 删除某元素在列表中的第一匹配项
列表.remove(元素)
```

​	**示例：**

```python
name_list = ['itheima', 'itcast', 'python']
del name_list[2]
print(name_list)
# 输出：['itheima', 'itcast']

name_list.pop(1)
print(name_list)
# 输出：['itheima']

num_list = [1, 2, 2, 3, 4]
num_list.remove(2)
print(num_list)
# 输出：[1, 2, 3, 4]
```

##### 1.1.7 清空

​	**语法：**

```python
# 清空列表内容
# 语法：
列表.clear()
```

​	**示例：**

```python
num_list = [1, 2, 3, 4]
num_list.clear()
print(num_list)
# 输出：[]
```

##### 1.1.8 统计

​	**语法：**

```python
# 统计某元素在列表内的数量
# 语法：
列表.count(元素)
```

​	**示例：**

```python
num_list = [1, 1, 1, 3, 4]
temp = num_list.count(1)
print(temp)
# 输出：3
```



##### 1.1.9 统计列表内，一共有多少元素

​	**语法：**

```python
len(列表)
```

​	**示例：**

```python
num_list = [1, 1, 1, 3, 4]
print(len(num_list))
# 输出：5
```



****



#### 2. 列表（list）的循环遍历



```python
def list_while_func():
    my_list = ["黑马程序员", "传智教育", "Python"]
    index = 0
    while index < len(my_list):
        element = my_list[index]
        print(f"列表的元素：{element}")
        index += 1


list_while_func()


def list_for_func():
    my_list = [1, 2, 3, 4, 5]
    for element in my_list:
        print(f"列表的元素：{element}")


list_for_func()

```