# 快速排序(Quick Sort)

&emsp;&emsp;快速排序算法的时间复杂度为$O(nlogn)$。但它在时间复杂度为$O(nlogn)$级的几种快速排序算法中，大多数情况下效率更高，所以快速排序的应用非常广泛。

## 原理

&emsp;&emsp;快速排序的基本思想是（升序为例）：

- 从数组中取出一个数，称为基数（pivot）
- 遍历数组，将比基数大的数字放到它的右边，比基数小的数字放在它的左边。遍历完成后，数组会被分为左右两个子数组。
- 以基数为中心，对其左右两个数组重复上述步骤，直至排序完成。

&emsp;&emsp;动画演示:
![](./imags/quickSort.gif)

> 在动画中，黑色标记的元素就是基数，一般我们会从数组的左右两边一起遍历即双指针法，左指针指向遇到的大于基数的值，右指针指向遇到的小于基数的值，然后左右指针的值进行交换即可。

## 实现

&emsp;&emsp;依据快排思想，我们可以确定要想实现快速排序，需要有一个划分函数$partition(arr,start,end)$。该函数的功能就是将数组$arr$的$start$元素到$end$的元素划分为两个部分，同时返回一个基准位置。以该位置为中心，左边的子数组应该都小于该基准数，右边的子数组，应该都大于该基准数。之后，在对左右两子数组进行进行划分。整个流程就是快速排序。

&emsp;&emsp;首先实现划分函数$partition$:

```C++
int partition(int arr[],int start,int end){
    // 选第一个元素作为基准
    int pivot = arr[start];
    // 从第二个元素开始遍历
    int left = start+1;
    int right = end;
    while(left < right){
        // 从左边找到大于基准数的值
        while(left < right && arr[left] < pivot) left++;
        // 从右边找到小于基准数的值
        while(left < right && arr[right] > pivot) right--;

        if(left < right){
            // 交换两数
            swap(arr[left],arr[right]);
            left++;
            right--;
        }
    }
    // 如果出现left == right并且arr[left] > pivot的情况，让right自减
    if(left == right && arr[left] > pivot) right--;
    // 交换基数与中心轴
    swap(arr[start],arr[right]);
    // 返回基准
    return right;
}
```

&emsp;&emsp;快速排序就是调用划分函数，排的是基准数，再对基准数左右两边数组调用划分函数，排基准数。

```C++

// 快速排序
void quickSort(int arr[],int start,int end){
    if(start < end){
        int pivotIndex = partition(arr,start,end);
        // 对左右子数组执行快排
        quickSort(arr,start,pivotIndex-1);
        quickSort(arr,pivotIndex+1,end);
    }
}
```

&emsp;&emsp;可以非常清楚，第一次遍历，可以排好1个基准数，第二次遍历，可以排2个基准数，第三次遍历，可以排4个基准数，以此类推。总遍历次数就为$logn$ ~ $n$,每次遍历的时间复杂度为$O(n)$。以此，总时间复杂度可以确定为：$O(nlogn)$ ~ $O(n^2)$。

**完整代码**

```C++

int partition(int arr[],int start,int end){
    // 选第一个元素作为基准
    int pivot = arr[start];
    // 从第二个元素开始遍历
    int left = start+1;
    int right = end;
    while(left < right){
        // 从左边找到大于基准数的值
        while(left < right && arr[left] < pivot) left++;
        // 从右边找到小于基准数的值
        while(left < right && arr[right] > pivot) right--;

        if(left < right){
            // 交换两数
            swap(arr[left],arr[right]);
            left++;
            right--;
        }
    }
    // 如果出现left == right并且arr[left] > pivot的情况，让right自减
    if(left == right && arr[left] > pivot) right--;
    // 交换基数与中心轴
    swap(arr[start],arr[right]);
    // 返回基准
    return right;
}

// 快速排序
void quickSort(int arr[],int start,int end){
    if(start < end){
        int pivotIndex = partition(arr,start,end);
        // 对左右子数组执行快排
        quickSort(arr,start,pivotIndex-1);
        quickSort(arr,pivotIndex+1,end);
    }
}
```
