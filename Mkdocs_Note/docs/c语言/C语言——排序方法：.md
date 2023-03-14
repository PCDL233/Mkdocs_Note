### C语言——排序方法：

排序分为：内排序和外排序。

`内排序`：插入排序、交换排序、选择排序、归并排序

**简单算法**：冒泡排序、简单排序、直接插入排序

**改进算法**：希尔排序、堆排序、归并排序、快速排序。





###### `冒泡排序`：

​	两两比较相邻记录的关键字，如果反序则交换，直到没有反序的记录为止。

![冒泡排序](https://img-blog.csdnimg.cn/20210402155752573.gif#pic_center)



```c
#include<stdio.h>
int main()
{
	int i, j, t;
	int sum[20] = {95,95,94,93,93,92,89,89,86,85,84,83,83,82,82,81,80,78,76};

	printf("输入你要插入学生的成绩:");
	scanf_s("%d", &sum[19]); //输入插入的成绩

	for (j = 0; j < 19; j++) //冒泡法排序，从小到大重新排序
        //当j=0时，与i=0,一直持续到i<19的值进行比较，如果大于则交换
        //第2次从i=1开始，与j=0,一直持续到i<18的值进行比较
	{
		for (i = 0; i < 19-j; i++)
		{
			if (sum[i] > sum[i + 1])//使用第三变量交换大小
			{
				t = sum[i];
				sum[i] = sum[i + 1];
				sum[i + 1] = t;
			}
		}
	}
	printf("重新排序后的成绩为：\n"); //输出从大到小重新排序后的成绩
	for (i =19;i>=0;i--)
	{
		printf("%d ", sum[i]);
	}
	return 0;
}

```







###### `简单选择排序`：	

​	通过n-i次关键字间的比较，从**n-i+1**个记录中选出关键字最小的记录，并和第	**i**（1≤i≤n）个记录交换。



![select](https://img-blog.csdnimg.cn/img_convert/a39c02b57f8c91c353f21035922d3493.gif)

​	

```c
#include<stdio.h>
 
int main() 
{
	int n, m, i, j, p, temp;
	int arr[100];
 
	scanf_s("%d", &n);
	for (i = 0; i < n; i++)
    {
		scanf_s("%d", &arr[i]);						//输入 
	}
 
	for (i = 0; i < n - 1; i++)
    {
		p = i;                            //p用于记录最小元素的下标
		for (j = i + 1; j < n; j++)  //从第一个元素开始，每一个元素(下标为i)和后面的元素进行比较，找到剩下元素中最小的那一个
        {      
			if (arr[p] > arr[j])
				p = j;
		}
		temp = arr[i];                        //temp是交换两数时的中间变量
		arr[i] = arr[p];
		arr[p] = temp;
	}
	for (i = 0; i < n; i++) 
    {
		printf("%d ", arr[i]);						//输出 
	}
	return 0;
}
```





###### **`直接插入排序`**：

​	直接插入排序就是将一个记录插入到已经排好序的有序表中，从而得到一个新的、记录增加了一个数的有序表。

​	通过构建有序序列，对于未排序数据，在已排序序列中从后向前扫描，找到相应位置并插入。

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200701163959370.gif)

![img](https://img-blog.csdnimg.cn/4b7dafa386a74908afddc01c71961e89.gif)

```c
//插入排序(从小到大) 
#include<stdio.h>
int num[100];
int main()
{
    int i = 0, n, m = 0, temp = 0;
    printf("输入数字个数：\n");
    scanf_s("%d", &n);

    printf("输入数字:");

    for (int j = 0; j < n; j++)
        scanf_s("%d", &num[j]);//输入数字存储到数组。
    for (i = 1; i < n; i++)
    {
        temp = num[i];//将temp每一次赋值给temp
        m = i - 1;

        while (m >= 0 && temp < num[m])   //改顺序 
        {
            num[m + 1] = num[m];//满足条件的，与后面的数交换，较大的放在后面
            m--;
        }
        num[m + 1] = temp;
    }
    for (i = 0; i < n - 1; i++)//输出
        printf("%d ", num[i]);
    printf("%d\n", num[i]);
    return 0;
}

```



###### **`快速排序`**：