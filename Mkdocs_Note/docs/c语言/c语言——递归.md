#### c语言——递归

​	在C语言中，一个调用自身的函数——称为函数递归。(**`自己调用自己`**)

​	递归的方式：`用小的程序解决复杂问题`

​		通常把一个大型复杂的问题层层转化为一个与原问题相似的规模较小的问题来求解

##### 条件：

1. 要有--**`限制条件`--**，当满足这个限制条件时，递归不在继续。
2. 循环中的值**`要有规律`**，例如：1 2 3 4 .....这样的数列
3. 每次递归后，就越来越接近最后的限制条件。

**例题：**

​		

```c
1	3	5	7	9	11	13	......
{
    f(n)=f(n-1)+2;//数列表达式
	f(1)=1;//递归出口
}

```

```C
#include<stdio.h>
int f(int n)
{
    if(n==1)//当第1项时（n=1时），直接返回1；
    {
        return 1;
    }
    else return (f(n-1)+2);//递归式{第10项=第9项+2，第9项=第8项+2，...第2项=第1项+2，第1项（n=1)=1}
}
int main()
{
    int num=f(10);//调用函数
    printf("num=%d",num);
}
```

```c
计算1+2+3+4+5...+n的值————f(n)=f(n-1)+n;

#include<stdio.h>
int sum(int n)
{
    if(n==1)//递归出口
    {
        return 1;
    }
    else {
        return (sum(n-1)+n);//递归式
    }
}
int mian()
{
    int num=sum(100);
    printf("num=%d",num);
}

```

