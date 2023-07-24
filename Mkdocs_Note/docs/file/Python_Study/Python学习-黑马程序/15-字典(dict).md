#### 字典（dict)

- 使用字典，实现 **key** 取出 **Value** 的操作。
- 字典的定义，使用 **`{ }`** ，不过存储的元素是一个个的：**键值对** 。
- 不允许 重复的数据	( **新的会覆盖老的** )
- 不可以使用下标索引，只有通过 **`key`** 值来取得对应的 **`value`**
- 字典的key和value可以是任意的数据类型，（key不可为字典）
- 字典可以嵌套

##### 语法：

```python
# 定义字典字面量
{key: value,key: value,key: value ......}

# 定义字典变量
my_dict = {key: value,key: value,key: value ......}

# 定义空字典
my_dict = {}
my_dict = dict()
```

##### 示例：

```python
# 定义字典
my_dict = {"张三": 99, "李四": 88, "王二": 77}
# 定义字典
my_dict1 = {}
my_dict2 = dict()
print(f"my_dict:{my_dict},类型：{type(my_dict)}")
print(f"my_dict1:{my_dict1},类型：{type(my_dict)}")
print(f"my_dict2:{my_dict2},类型：{type(my_dict)}")

"""
输出：
my_dict:{'张三': 99, '李四': 88, '王二': 77},类型：<class 'dict'>
my_dict1:{},类型：<class 'dict'>
my_dict2:{},类型：<class 'dict'>
"""
```



**通过Key来获取value：**

```python
my_dict = {"张三": 99, "李四": 88, "王二": 77}
score = my_dict["张三"]
print(score)

# 输出：99
```



**字典嵌套：**

```python
my_dict4 = {
    "张三": {"语文": 77, "数学": 66, "英语": 33},
    "李四": {"语文": 88, "数学": 86, "英语": 55},
    "王二": {"语文": 99, "数学": 96, "英语": 65},
}
print(f"学生成绩信息：{my_dict4}")
score = my_dict4["张三"]["语文"]
print(f"张三语文成绩：{score}")
```



****



#### 字典常用操作

| 编号 | 语法              | 作用                                                    |
| :--: | :---------------- | :------------------------------------------------------ |
|  1   | 字典[key] = value | 新增元素、更新元素                                      |
|  2   | 字典.pop(key)     | 获得指定key的value，同时字典被修改，指定key的数据被删除 |
|  3   | 字典.clear()      | 字典被修改，元素被清空                                  |
|  4   | 字典.keys()       | 获取字典全部的key                                       |
|  5   | len(字典)         | 计算字典内的元素数量                                    |



#### 字典遍历

- 不支持 while 循环遍历
- 可以使用 for 循环遍历

```python
#字典定义
my_dict = {"张三": 99, "李四": 88, "王二": 77}

# 新增元素
my_dict["陈一"] = 33
# 更新元素
my_dict["王二"] = 44
print(my_dict)

# 获取字典全部key
keys = my_dict.keys()
print(keys)

# 遍历字典
# 方式1：通过获取全部的key来完成
for key in keys:
    print(f"key：{key}")
    print(f"value：{my_dict[key]}")

# 方式2：直接对字典进行for循环，每一次循环都是直接得到key
for key in my_dict:
    print(f"key：{key}")
    print(f"value：{my_dict[key]}")
```

