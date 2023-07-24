### C++ 中string函数用法：

##### string的**大小和容量：**

###### `size()`和`length()`

​				：返回string所作用的字符串的**长度**

```c++
#include<iostream>
#include<string>
using namespace std;
int main()
{
    string num("1234567");
    cout<<"size="<<num.size()<<endl;
    //调用size和length函数输出字符串num的长度
    cout<<"length="<<num.length()<<endl;
    //输出为size=7，length=7
    return 0;
}
```

###### `max_size()`

​		返回字符串最多包含的字符数，超出会显示异常

```c++
#include<iostream>
#include<string>
using namespace std;
int main()
{
    string num("1234567");
    cout<<"max_size="<<num.max_size()<<endl;
   return 0;//输出为max_size=2147483647
   
}
```

###### `capacity()`

​		**重新分配内存之前**，string对象能包含的最大字符数

```c++
#include<iostream>
#include<string>
using namespace std;
int main()
{
    string num("1234567");
    cout<<"capacity="<<num.capacity()<<endl;
   return 0;
    //输出为capacity=15,即在重新分配内存之前num字符串最大能包容的字符数为15
  
}
   
```

##### string的**字符串比较**：`compare(）`函数

​	将字符按字典顺序进行逐一的比较。字典排序靠前的字符小,比较的顺序是从前向后比较(**遵从ASCII码**)。

​		例如：str1("abc")<str2("ABC")——***str1.compare(str2)***

​		返回值为：1——大于；（-1）——小于；0——等于

```c++
#include<iostream>
#include<string>
using namespace std;
int main()
{
    string s1("abc");//在ASCII码中a=97，A=65
    string s2("ABC");
    cout<<"s1.compare(s2)="<<s1.compare(s2)<<endl;
   return 0;
    //输出为s1.compare(s2)=1,即s1大于s2
  
}
```

##### **字符串的插入：`push_back()`、`insert()`、`append()`**



###### `push_back()函数`

​			：只能在原有的字符串的**最后面**插入新的字符

```c++
e.g：string s1("chin");
	s1.push_back('a');
//在字符串chin后插入一个a字符，输出为：china
```

###### `append()函数`

1、直接在原有字符串后添加新的字符串

```c++
string s1("chi");
string s2("na");
s1.append(s2);//将字符串s2中的字符添加到s1字符串的后面
cout<<s1;//输出为：china
```

2、添加新字符串的一部分

```c++
string s1("I love");
string s2("xx china");
s1.append(s2,2,6);//将字符串s2中从第2个字符后面的连续6个字符添加到s1中。
cout<<s1;//输出为：I love china
```

​	若是添加的子串中只有索引开始的位置，没有长度，则表示字符串从`第n个字符到末尾`的字符连接到当前字符串末尾。

```c++
string s1("I love");
string s2("xx china");
s1.append(s2,2);//将字符串s2中从第2个字符后面一直到s2字符串尾的字符添加到s1
cout<<s1;//输出为：I love china
```

在string后面添加**多个相同字符**,如下

```c++
  string s1 = "hello";
  s1.append(3, '!'); //在当前字符串结尾添加3个字符!
  //输出为： s1 = "hello!!!";
```

###### `insert()函数：`

```c++
string s("hina");
s.insert(s.begin(),c);
//括号前面的为字符串s的开头（即位置），后面是要插入的字符
cout<<s;//输出为：China
```

###### `erase()函数`：

​		删除字符串中的字符，从指定容器删除指定位置的元素或某段范围内的元素 

1、删除指定位置的字符。

```C++
iterator erase (iterator p);
```

2、删除指定长度的字符串。

```c++
string& erase(size_t pos=0, size_t len = npos);
```

其中，参数pos表示要删除字符串的起始位置，其默认值是0；len表示要删除字符串的长度，其默认值是string::npos。返回值是删除后的字符串。

3、删除指定范围的字符串。——范围是[first, last)。

```c++
iterator erase (iterator first, iterator last);
```

###### `删除例题：`

```c++
#include<iostream>
#include<string>
using namespace std;
int main()
{
	string str("Hello World！！！");

	str.erase(str.begin()+5);//删除从str字符串开始（从0开始）后面第5个字符
	cout << str<<endl;//输出为：HelloWorld！！！


}
```



```c++
#include<iostream>
#include<string>
using namespace std;
int main()
{
	string str("Hello World！！！");

	str.erase(6, 5);//删除从str字符串第6个字符后面的5个字符
	cout << str<<endl;//输出为：Hello ！！！


}
```

```c++
#include<iostream>
#include<string>
using namespace std;
int main()
{
	string str("Hello World！！！");

	str.erase(str.begin() + 5, str.end() - 2);
//输出从那个字符串开头往后第5个字符和从尾往前数第2个字符之间的字符范围删除
	cout << str << endl;//输出为：Hello！


}
```



###### string拼接字符串：`append()`

```c++
#include<iostream>
#incluce<string>
using namespace std;
int main()
{
    string s1("Hello World!");
    string s2("abc");
    s1.append(s2);//将s2的内容拼接到s1后面
    cout<<"s1:"<<s1<<endl;
    return 0;
}
//输出--->s1:Hello World!abc
```

###### string的字符替换：replace()

```c++
#include<iostream>
#include<string>
using namespace std;
int main()
{
    string s("Hello World");
    s.replace(6,5,"!!!");
    //括号中第1个数字表示原来字符串中要替换的字符开始的所在位置，第2个数字表示要把原来字符串中的几个字符替换。
    //将s中的第6个字符后面的5个字符全部替换成"!!!"。
    cout<<s<<endl;
    return 0;
}
//输出为：Hello !!!
```

###### string中的大小写转换

​			`tolower()`、`toupper()`、`transform()`

```c++
#include<iostream>
#include<string>
using namespace std;
int main()
{
    string s=("HELLO");
    for(int i=0;i<s.length();i++)
        //通过循环进行c语言字符数组的一个个转化操作
    {
        s[i]=tolower(s[i]);
    }
    cout<<s<<endl;
    return 0;
}//输出--->hello
```



###### STL中的 **transform()**用法：

```c++
#include<iostream>
#include<string>
#include <algorithm>//运用STL中的transform（）的头文件
using namespace std;
int main()
{
    string s1 = ("HELLO");
    string s2 = ("hello");
    transform(s2.begin(), s2.end(), s2.begin(), ::toupper);//化为大写
    transform(s1.begin(), s1.end(), s1.begin(), ::tolower);//化为小写
    cout << s1 << " " << s2 << endl;
    return 0;
}
//输出---->hello HELLO
```

###### 查找--->`find()`

```c++
#include<iostream>
#include<string>
using namespace std;
int main()
{
    int x=0;
    string s=("abcdefg");
    x=s.find("de");
    cout<<x<<endl;//输出为3；
    
    x=s.find("e",1);//从字符串第1个字符开始查找“e”这个字符
    cout<<x<<endl;//输出为4；
    
    x=s.rfind("e");//从字符串尾开始查找“e”
    cout<<x<<endl;//输出为4；
    
    x=s.find_first_of("1e2344");
    //在该字符串中查找第一个属于字符串s的字符
    cout<<x<<endl;
//输出为4，表示这个字符串中第一个属于s中的字符是s中的4---e；
    
    x= s.find_first_not_of("abcdh") ；
        //在该字符串中查找第一个不属于字符串s的字符
    cout<<x;//输出：4---h
    return 0;
}
```



###### 截取字符串：`substr()`

​	[strtok]函数会把分割前的字符串破坏掉，即每次分割后，**原来的字符串就会少掉一部分**，完整性会被破坏。

```c++
#include<iostream>
#include<string>
using namespace std;
int main()
{
    string s=("hello world admin");
	string m;
    m=s.substr(6,5);//截取字符串是中第6个字符后面5个字符
    cout<<m;
 	 return 0；//输出--->world
}
```

