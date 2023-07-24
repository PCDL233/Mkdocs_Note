

## C++ **标准模板库（STL）**

#### 特点：

1、标准模板库中的数据结构和算法是**分离**的

2、不是面向对象的

#### STL六大组件：

1. `容器`（Container）：为一种数据结构，以模板类的方法提供。为了访问容器中的数据，可以使用由容器类输出的迭代器。

2. `迭代器`（Lterator）：提供了访问容器中对象的方法。可以使用一对迭代器指定list或vector中的一定范围的对象。**迭代器就如同一个指针**。

3. `算法`（Algorithm）：是用来操作容器中的数据的**模板函数**。

4. `仿函数`（Functor）：是一个定义了operator（）的对象（即重载了括号运算符），**可以将它视为一般的函数**，**但它是一个类**。但它与一般函数的区别是其功能是在其成员函数operator()中定义，主要具有以下三个优点:

   （1）比一般的函数灵活，应为仿函数拥有状态（即有成员变量做数据的记录）；

   （2）仿函数型别可以**作为模板参数**；

   （3）仿函数要比函数指针的执行速度要快；

5. `适配器`（Adaptor）：容器适配器，迭代器适配器和函数适配器。

   ​		能够将仿函数和另一个仿函数（或某个值，或某个一般函数）**结合起来的仿函数**。

   函数配接器包含在头文件`<functional>`中。

6. `分配器`（allocator）：用特殊对象处理**`[内存]`**的分配和规划，这样的对象称为**分配器。**

   #### 

#### queues(队列)，Lists(链表)，stacks(栈)

#### 顺序结构：C++ Vectors

|         函数          |                             表述                             |
| :-------------------: | :----------------------------------------------------------: |
|   c.assign(beg,end)   |              将[beg; end)区间中的数据赋值给c。               |
|     c.assign(n,x)     |                  将n个x的元素拷贝赋值给c。                   |
|       c.at(idx)       | 传回索引**`i`**所指的数据，如果**`i`**越界，抛出out_of_range。 |
|       c.back()        |          传回最后一个数据，不检查这个数据是否存在。          |
|       c.begin()       |                  传回迭代器中的第一个数据。                  |
|     c.capacity()      |                     返回容器中数据个数。                     |
|       c.clear()       |                     移除容器中所有数据。                     |
|       c.empty()       |                      判断容器是否为空。                      |
|        c.end()        |               指向迭代器中的最后一个数据地址。               |
|     c.erase(pos)      |          删除pos位置的数据，传回下一个数据的位置。           |
|   c.erase(beg,end)    |       删除[beg,end)区间的数据，传回下一个数据的位置。        |
|       c.front()       |                       传回第一个数据。                       |
|     get_allocator     |                  使用构造函数返回一个拷贝。                  |
|  c.insert(pos,elem)   |         在pos位置插入一个elem拷贝，传回新数据位置。          |
|   c.insert(pos,n,x)   |            在pos位置插入n个x元素数据。无返回值。             |
| c.insert(pos,beg,end) |         在pos位置插入在[beg,end)区间的数据。无返回值         |
|     c.max_size()      |                   返回容器中最大数据的数量                   |
|     c.pop_back()      |                      删除最后一个数据。                      |
|   c.push_back(elem)   |                     在尾部加入一个数据。                     |
|      c.rbegin()       |                传回一个逆向队列的第一个数据。                |
|       c.rend()        |         传回一个逆向队列的最后一个数据的下一个位置。         |
|     c.resize(num)     |                     重新指定队列的长度。                     |
|      c.reserve()      |                       保留适当的容量。                       |
|       c.size()        |                  返回容器中实际数据的个数。                  |
|      c1.swap(c2)      |                      将c1和c2元素互换。                      |
|      swap(c1,c2)      |                      将c1和c2元素互换。                      |



##### `Constructors` 	构造函数

 		vector是由STL提供的一种序列式容器，它的底层其实就是一个**动态数组**。如要使用vector，需要`#include<vector>`。

**语法**：vector<元素类型>数据对象名（数据长度，元素初值）

例：

```c++
vector<int> v1( 5, 42 );
//构造了一个包含5个值为42的元素的Vector
```



##### `assign（）`函数

```c++
语法：c.assign(n,elem)----->//c.assign(n,elem)

	 c.assign(beg,end)------>//将[beg; end)区间中的数据赋值给c。

```



```c++
void assign(const_iterator first,const_iterator last);
//相当于拷贝函数，将区间[first,last)中的元素赋值到当前的vector容器中
void assign(size_type n,const T& x = T());
//赋 n 个值为 x 的元素到 vector 容器中，并且清除掉 vector 容器中以前的内容。

```

```c++
   //输入
    vector<int> v1;
    vector<int> v2;
    
    //assigning
    v1.assign(5, 100);
    v2.assign(v1.begin(), v1.end());
 
  	//输出
    //if we print the value
    v1: 100 100 100 100 100
    v2: 100 100 100 100 100


```



##### `at（）`函数

语法：c.at(i)------>传回索引**`i`**所指的数据，如果**`i`**越界，抛出out_of_range或者**终止程序。**

```c++
#include<iostream>
#include<string>
using namespace std;
int main()
{
    string str;
	cin>>str;  //str=="12345"
	char ch;
	ch = str.at(0);
	cout<<ch;   //输出ch=='1';
    return 0;

}

```

##### `back（）`函数

​		**：**返回当前vector容器中**末尾元素**的引用。

语法：c.back()------>返回c中最后一个元素，**不检查这个数据是否存在**

**`front（）`函数：**

​		返回当前vector**起始元素**的引用

```c++
语法：c.front()------>//返回c中初始的元素。
```

```c++
#include<iostream>
#include<string>
#include<vector>
using namespace std;
int main()
{
    vector<int> s1;//定义一个空的容器s1；
 for(int i=0;i<4;i++)
 {
     s1.push_back(i);//利用循环将i插入到s1容器中
 }
    cout<<s1.back()<<endl<<s1.front()<<endl;
    //返回s1容器中的最后的元素和初始元素，输出为3，0；
    return 0;   	
}
```

##### `begin()`函数

​		**：**返回一个指向当前vector(容器)起始元素的**迭代器**（`iterator`）

##### `end`函数

​		**：**返回一个指向当前vector末尾元素的**下一位置**的**迭代器**（`iterator`）；与begina()函数相似。

##### `rbegin()`函数

​			**：**返回指向当前vector**末尾**位置的**逆**迭代器，与**[end()函数]()**相似。

##### **`rend()`**函数

​			**：**返回指向当前vector**起始**位置的**逆**迭代器,与**[begin()函数]()**相似



```c++
#include<iostream>
#include<string>
#include<vector>
using namespace std;
int main()
{
	vector<int> s1(2,56);//定义一个存放2个"56"的容器s1;
    vector<int>::iterator it;//定义一个迭代器it
    //用迭代it来接收容器中第一个元素的地址
    for(it=s1.begin();it!=s1.end();it++)//利用迭代器it从s1中的第一个元素开始
    {
        cout<<*it<<endl;//输出解引用it的值；
       
    }
     return 0;
}
```



##### `capacity（）`函数

​		指容器在**分配新的存储空间之前**能存储的**元素总数**。capacity（）是容器可存储的最大总数，size（）是当前容器存储的个数（***即容器实际存储的元素的个数***）。

```c++
#include<iostream>
#include<string>
#include<vector>
using namespace std;
int main()
{
  vector<int> v;  //此时没有初始化，所以size()和capacity()都是0；

v.push_back(1);
cout<<"size="<<v.size()<<" capacity="<<v.capacity()<<endl;
    //此时容器内有一个元素了，那么size()和capacity()都是1
v.push_back(1);
cout<<"size="<<v.size()<<" capacity="<<v.capacity()<<endl;
    //此时容器内能够提供的空间capacity()不够用了，需要申请内容，申请多少呢，申请后的大小应该是以前的2倍，那就应该是2了，此时有两个元素，size（）为2，capacity（）也是2
v.push_back(1);
cout<<"size="<<v.size()<<" capacity="<<v.capacity()<<endl;
    //此时容器能够提供的空间是2，又增加元素，不够，需要申请空间，申请后的空间为原来2倍，就是4了，那么size()为3，capacity（）为4
v.push_back(1);
cout<<"size="<<v.size()<<" capacity="<<v.capacity()<<endl;
    //容器还能够提供一个空间，不需要申请新空间，size()为4，capacity（）为4
v.push_back(1);
cout<<"size="<<v.size()<<" capacity="<<v.capacity()<<endl;
    //空间不够，需要申请，size()为5，capacity为8
    return 0;
}

//输出为：
size=1 capacity=1
size=2 capacity=2
size=3 capacity=4
size=4 capacity=4
size=5 capacity=8
```



##### **`clear()`函数**

​		删除当前vector中的所有元素。

```c++
语法：c. clear();----->//移除容器c中所有的元素。
```



```c++
#include<iostream>
#include<string>
#include<vector>
using namespace std;
int main()
{
    int a[5]={1,2,3,4,5};
    vector<int> s1(a,a+6);
    vector<int>::iterator it;//定义迭代器it和mi
    vector<int>::iterator mi;
    for(it=s1.begin();it!=s1.end();it++)//利用迭代器it从s1中的第一个元素开始
    {
        cout<<*it<<endl;//输出解引用it的值；
     }
    s1.clear();//清除后s1容器为空。
     for(mi=s1.begin();mi!=s1.end();mi++)//利用迭代器mi从s1中的第一个元素开始
    {
        cout<<*mi<<endl;//输出解引用mi的值；
     }
    return 0;
}
```

![](C:\Users\CMQ233\Pictures\竞赛刷题\屏幕截图 2022-11-17 160016.png)

![](C:\Users\CMQ233\Pictures\竞赛刷题\屏幕截图 2022-11-17 160156.png)



##### `empty()`函数

​		用来测试变量是否已经配置。若变量已存在、**非空**字符串或者非零，则返回 **false** 值；反之返回 **true**值。所以，当字符串的值为0时，也返回true，就是执行empty内部的语句。

即：**验证当前这个容器是否已经赋值（已经有元素在里面）**

```c++
#include<iostream>
#include<vector>
using namespace std;
int main()
{
    vector<int> s;
    int s1=s.empty();
    cout<<"s1="<<s1<<endl;
    //输出：s1=1，没有容纳任何元素返回1----->为真
     s.assign(5, 100);
    int s2=s.empty();
    cout<<"s2="<<s2;
    //输出：s2=0，有元素了，返回值为0---->为假
    return 0;
}
```

**可做为循环的条件执行：**



```c++
while( !v.empty() )------>//作为循环执行的判断条件
{
  cout << v.back() << endl;
   v.pop_back();
 }

```



##### `erase()函数`

​		**：**要么删作**指定位置loc的元素**,要么删除**区间[start, end)**的所有元素。返回值是指向删除的最后一个元素的下一位置的迭代器(**即下一个数据的`位置`**）。

```c++
c.erase(pos)---->//删除pos位置的数据，传回下一个数据的位置。

c.erase(beg,end)---->//删除[beg,end)区间的数据，传回下一个数据的位置。

```

```c++
#include<iostream>
#include<vector>
#include<string>
using namespace std;
int main()
{
    string s = { "abcdef"};
    s.erase(s.begin()+3);
    cout << s;//输出：abcef，将字符'd'删除；
    s.erase(s.begin() + 3,s.end());
    cout << s << endl;//输出：abc，将字符串中区间[3,6)的字符删除；
    return 0;
}
```



##### `pop_back()`函数

​			**：**删除当前容器中（vector)**最后**的一个元素。

```c++
语法：void pop_back();
	 vector<int> c;
	 c.pop_back();----->//删除容器c中最后的元素。
```

```c++
#include<iostream>
#include<vector>
#include<string>
using namespace std;
int main()
{
    vector<int> s;
    for (int i = 0; i < 10; i++)
        s.push_back(i);
   
    vector<int>::iterator b;
    for (b = s.begin(); b != s.end(); b++)
    {
        cout << *b << " ";//输出：0 1 2 3 4 5 6 7 8 9
    }
    cout << endl;
    s.pop_back();//删除容器s中最后一个元素'9'。

    vector<int>::iterator a;
    for (a = s.begin(); a != s.end(); a++)
    {
        cout << *a << " ";//输出：0 1 2 3 4 5 6 7 8
     }
    
    
}

```



##### `push_back()函数`

​			：添加元素到当前容器（vector）**末尾**，（插入元素到容器中）；

```c++
#include<iostream>
#include<vector>
#include<string>
using namespace std;
int main()
{
    string s1;
    for (char i = 'a'; i<'a'+10; i++)
    {
        s1.push_back(i);//从i='a'开始的字符插入s1中
    }
    vector<int> s2;
    for (int i = 0; i <10; i++)
    {
        s2.push_back(i);//将i的值插入容器s2中
    }
    
    cout << "s1="<< s1 << endl;//输出：s1=abcdefghij


    vector<int>::iterator a;
    cout << "s2=";
    for (a = s2.begin(); a != s2.end(); a++)
    {
        cout  << *a << " ";//输出：s2=0 1 2 3 4 5 6 7 8 9
    }
    return 0;
}
```



##### **`reserve()`函数**

​			：为当前vector预留至少共容纳size个元素的空间.(译注:实际空间可能大于size)。**调整vector大小**，使之可以容纳n个元素，如果当前vector容量小于n，则扩展容量至n，其他情况则不进行存储重新分配，对容量没有影响。

```c++
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    int  s1;
    vector<int> a1;
    s1 = a1.capacity();//定义是s1存储容器a1的最大存储数
    cout << "a1:" << endl;
    for (int i = 0; i < 100; i++) 
    {
        a1.push_back(i);//向容器中插入i的值
        if (s1 != a1.capacity()) 
        {
            s1 = a1.capacity();
            cout << "capacity changed: " << s1 << '\n';
            //输出容器最大存储数的变化：1，2，3，4，6，9，13，19......
            //容器中的最大存储数随着元素的增加而增加
        }
    }

    vector<int> a2;
    s1 = a2.capacity();//将容器a1的最大存储数赋值给s1。
    a2.reserve(500);   // 直接调整容器bar的空间为100。
  cout <<"a2:"<<endl;
    for (int i = 0; i < 100; ++i) 
    {
        a2.push_back(i);
        if (s1 != a2.capacity()) 
        {
            s1 = a2.capacity();
            cout << "capacity changed: " << s1 << '\n';
            //容器足够存储增加的值，所以输出的值不会改变；输出为：500。
        }
    }
    return 0;
}
```



##### **`resize()`**函数

​		

```c++
c.resize(num)----->改变c容器的存储大小为num(数字)
```

```c++
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    vector<int> s;
    for(int i=0;i<10;i++)
    {
        s.push_back(i);
	}
    cout<<"size of:"<<s.size()<<endl;//输出=size of:10

    s.resize(100);//重新调整容器s的size为100；
   cout<<"changed size of:"<<s.size()<<endl;//输出=changed size of:100
    return 0;
}
```



##### `swap()`函数

```c++
c1.swap(c2)----->将c1和c2元素互换。
swap(c1,c2)----->将c1和c2元素互换。
```

```c++
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    vector<int> s1;
    s1.assign(1, 500);
    vector<int> s2;
    s2.assign(1, 100);
    cout << "s1=" << s1[0] << "s2=" << s2[0] << endl;
    swap(s1, s2);
    cout << "changed s1=" << s1[0] << "changed s2=" << s2[0] << endl;
    return 0;
    //输出：s1=500s2=100
		//changed s1=100changed s2=500
}

```

