```python
from pymysql import Connection

# 构建mysql链接对象
conn = Connection(
    host="localhost",
    port=3306,
    user="root",
    password="2815834616",
    autocommit=True
)
# 获取游标对象
cursor = conn.cursor()
# 选择数据库
conn.select_db("py_sql")
# 组织sql语句
# 查询数据库中orders表中的全部数据
cursor.execute("select * from orders")
# 获取查询的结果(结果为元组类型)
results: tuple = cursor.fetchall()

with open("销售数据导出.txt", "w", encoding="UTF-8") as f:
    for data in results:
        # 调用元组下标,存储进字典
        data_dict = {
            "data": str(data[0]),
            "order_id": data[1],
            "money": data[2],
            "province": data[3]
        }

        # 将字典转换为字符串类型
        line = str(data_dict)
        f.write(line + "\n")
    # 刷新内容
    f.flush()

# 关闭数据库链接
conn.close()

```

