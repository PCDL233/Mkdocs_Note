# 希尔排序(Shell Sort)

&emsp;&emsp;希尔排序是希尔(Donald Shell)于1959年提出的一种排序算法。希尔排序也是一种**插入排序**，它是简单插入排序经过改进之后的一个更高效的版本，也称为**缩小增量排序**，同时该算法是冲破$O(n^2)$的第一批算法之一。

## 原理

&emsp;&emsp;**希尔排序是把记录按下标的一定增量分组，对每组使用直接插入排序算法排序；随着增量逐渐减少，每组包含的关键词越来越多，当增量减至1时，整个文件恰被分成一组，算法便终止**。

算法步骤如下：

- 将待排序序列划分为若干子序列(每个子序列的元素在原始数组中间距相同)；
- 对这些子序列进行插入排序；
- 减小每个子序列中元素之间的间距，重复上述过程直至间距减少为1；

从步骤中可以看出，希尔排序主要是依据经典插入排序的以下两点进行改进：

- **插入排序在对几乎已经排好序的数据操作时，效率高，即可以达到线性排序的效率**。
- 插入排序一般来说是低效的，因为插入排序每次只能将数据移动一位；

动图演示：

![](./imags/shellSort_1.gif)

&emsp;&emsp;演示过程中，不同颜色标注出来的元素各自组成了不同的子序列，这些子序列就是依据**增量**进行划分。开始时增量很大，希尔排序对子序列进行插入排序，使得整个序列在"**宏观**"上是有序的，之后随着增量不断减少，使得整个序列在"**微观**"上是有序的，从而达到整体有序。之前谈论过，**插入排序在对几乎已经排好序的数据进行操作时，效率是很高的**。因此这种宏观上有序对插入排序的效率非常有利，因此，希尔排序虽然是插入排序，但其效率却远比普通的插入排序要高。

## 实现

```C++

void shellSort(int arr[],int len){
    // step是增量，每次折半减小
    for(int step = len / 2;step > 0;step /= 2){
        // 对子序列执行插入排序
        for(int i=step;i<len;i++){
            int t =arr[i];
            int index = i;
            // 找到合适的插入位置，数组小标移动要以增量为单位
            while(index >= step && arr[index - step] > t){
                arr[index] = arr[index-step];
                index -= step;
            }
            arr[index] = t;
        }
    }
}
```

时间复杂度与空间复杂度分析：事实上，希尔排序时间复杂度非常难以分析，它的平均复杂度界于$O(n*logn)$~$O(n^{1.25})$之间，空间复杂度为$O(1)$。

## 习题

待补充。