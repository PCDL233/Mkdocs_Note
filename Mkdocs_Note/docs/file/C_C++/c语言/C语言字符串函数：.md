### C语言字符串函数：

**字符串的定义：**

​			字符串常量是由双引号（“ ”）引起来的字符序列。

​			例如：“hello world！”		“ C	program”等。

字符串和字符常量的差别在于，编译器会自动的每一个字符串的后面加上一个空操作符`'\0'`，作为字符串结束的标志。

**字符函数：**

##### `gets`函数

​		：输入字符串的函数。



```c
#include<stdio.h>
#include<string.h>
int main()
{
    char str[10];//定义一个字符数组
    gets(str);//调用gets函数接收输入的字符串
    return 0;
    
}
```

##### `puts`函数

​		：输出字符串的函数。

```c
#include<stdio.h>
#include<string.h>
int main()
{
    char str[10]={"C program"};
    puts(str);//调用puts函数，输出str数组中的字符串。
    return 0;
}
```

##### `strcat`函数

​		：将字符串拼接起来的函数。将字符串2与字符串1进行拼接，然后放在字符串1所在的字符数组中。

```c
#include<stdio.h>
#include<string.h>
int main()
{
    char s1[10]={"chi"},s2[10]={"na"};//定义两个字符数组分别存储字符串
    
    strcat(s1,s2);//将s1与s2中的字符串进行拼接，再存储在s1中
    puts(s1);//输出s1，为china。
    return 0;
}

```

##### `strcpy`函数

​		：复制字符串的函数。

```c
#include<stdio.h>
#include<string.h>
int main()
{
    char s1[10]={"china"};
    char s2[10]={"abc"};
    strcpy(s1,s2);//将字符串s2复制到s1中。
    puts(s1);//输出s1，为：abc
    return 0;
}
```

##### `strlen`函数

​		：测量字符串长度的函数，不包括`'\0'`(空字符)。

```c
#include<stdio.h>
#include<string.h>
int main()
{
    char s1={"qweqweq"};
  	int m=strlen(s1);//定义一个变量存储字符串s1的长度
    printf("%d",m);//输出字符串s1长度,输出为7
    return 0;
    
}
```

##### `strlwr`函数

​			：将字符串的所有字母转换为小写的。

```c
#include<stdio.h>
#include<string.h>
int main()
{
    char s1[10]={"AbbA"};
    strlwr(s1);//将大写转换为小写
    puts(s1);//输出为：abba
    return 0;
}
        
```

##### `strupr`函数

​			：将字符串的所有字母转换为大写的。

```c
#include<stdio.h>
#include<string.h>
int main()
{
    char s1[10]={"aBBa"};
    strupr(s1);
    puts(s1);//输出为：ABBA
    return 0;
}
```

##### `strstr`函数

​		：查找字符串的函数

​		函数用于判断字符串str2是否是str1的子串。如果是，则该函数返回str2在str1中**首次出现的地址**；否则，返回NULL（为空）。如果找到该数组，就会从**找到的地方开始输出**；

```c
#include <string.h>
#include <stdio.h> 
int main()
{
	char a[10] = "abcdefg";
	char b[10] = "bc";
 
	char* ret = strstr(a, b);
    //定义一个指针变量存储字符串bc在a数组中首次出现的地址。
 	
    printf("%s\n", *ret);  //输出 bcdefg
	return 0;
}
```

