```python
from Data_define import Record
from File_define import TextFileReader, JsonFileReader
from pymysql import Connection

# 读取数据
text_FileReader = TextFileReader("2011年1月销售数据.txt")
json_FileReader = JsonFileReader("2011年2月销售数据JSON.txt")

data1: list[Record] = text_FileReader.read_data()
data2: list[Record] = json_FileReader.read_data()

# 将两个月的数据合并成一个list
all_data: list[Record] = data2 + data1

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
for record in all_data:
    if record.data is None:
        continue
    else:
        sql = f"insert into orders(order_data,order_id,money,province)" \
              f"values('{record.data}','{record.order_id}',{record.money},'{record.province}')"
    # 执行sql语句
    cursor.execute(sql)

# 关闭数据库链接
conn.close()

```

