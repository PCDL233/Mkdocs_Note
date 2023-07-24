# 选择排序（Selection Sort）

&emsp;&emsp;选择排序是一种简单而高效的排序算法，无论什么样的数据使用选择排序，其时间复杂度都是$O(n^2)$。所以使用选择排序，其数据规模应当越小越好。

## 原理

&emsp;&emsp;选择排序通过列表的未排序部分中重复选择最大/最小元素并将其移动到列表的已排序部分。该算法不断从未排序序列中选择最大/最小元素，并将其与未排序序列的第一个元素或已排序序列后一个元素进行交换。对整个列表不断执行该过程，最终得到一个有序序列。步骤如下：

- 首先在未排序序列中找到最小/最大元素，存放到排序序列的起始位置。开始时，未排序序列的第一个位置为0(序列下标从0开始)，或已排序序列之后的位置(开始时没有任何元素是已排状态，整个序列都是待排状态)。
- 再从剩余未排序元素中找到最小/最大元素，放到已排序列的末尾。
- 重复上述过程，直至待排序列为空。

![](./imags/selectionSort_1.gif)

> 上述动画中，黄色部分是已排序列，蔚蓝色是待排序列，红色是待排序列中的最小值，绿色移动过程就是在查找最值的过程。

## 实现

### 代码一

&emsp;&emsp;选择排序也是可以优化的，此处先介绍未优化的代码：

```C++

void selectionSortWay1(int arr[],int len){
    // 记录待排序列的最小元素的下标
    int minIndex;
    for(int i=0;i<len;i++){
        minIndex = i;
        for(int j=i;j<len;j++){
            // 若发现更小元素，更新下标
            if(arr[j] < arr[minIndex]){
                minIndex = j;
            }
        }
        // 将最小元素插入到待排序列的第一个位置上
        int t = arr[minIndex];
        arr[minIndex] = arr[i];
        arr[i] = t;
    }
}

```

> 上述代码的外层$for$循环其实控制的就是待排序列的范围$[i,len-1]$;因此，待排序列的第一个位置其实就是$i$，我们**只需要找到整个待排序列的最小值放到位置$i$上**就行了。

### 代码二

&emsp;&emsp;代码一展示的就是从待排序列中找到最小值将其放到相应位置的实现逻辑。实际上，我们可以用二元变量对其进行修改，这两个变量分别记录待排序列中的最大和最小值。再扫描完整个待排序列后，最大值放在右边，最小值放在左边。这种优化方法也称为“双向选择排序”。

```C++

void selectionSortWay2(int arr[],int len){
    // 记录最大最小索引
    int minIndex,maxIndex;
    // 双向选择
    for(int i=0;i<len/2;i++){
        minIndex = i;
        maxIndex = len-1-i;
        for(int j = i;j<len-i;j++){
            if(arr[j] < arr[minIndex]){
                minIndex = j;
            }
            if(arr[j] > arr[maxIndex]){
                maxIndex = j;
            }
        }
        // 当最大索引和最小索引相等时，说明序列是有序的了
        if(maxIndex == minIndex) break;
        // 将最小元素插入到待排序列的第一个位置上
        int t = arr[i];
        arr[i] = arr[minIndex];
        arr[minIndex] = t;
        // 当最大值的下标恰好是i时，由于i位置上的已进行了交换，因此原来i上的元素是在交换后的minIndex上
        if(maxIndex == i) maxIndex = minIndex;
        t = arr[len-1-i];
        arr[len-1-i] = arr[maxIndex];
        arr[maxIndex] = t;
    }
}

```

&emsp;&emsp;由代码可分析出选择排序的时间复杂度和空间复杂度分别为:$O(n^2)$和$O(1)$。

## 习题

### 习题一

&emsp;&emsp;给定整数数组 $nums$ 和整数 $k$，请返回数组中第 $k$ 个最大的元素。请注意，你需要找的是数组排序后的第 $k$ 个最大的元素，而不是第 $k$ 个不同的元素。

示例：

```
输入: [3,2,1,5,6,4], k = 2
输出: 5
```

> 思路

&emsp;&emsp;由题意可知，我们可以不用对整个数组的所有元素进行排序，只需排$k$个数即可。像这种部分排序的场景，可以使用选择排序或堆排序解决。在选择排序中，我们每次选出最大值放在待排序列的第一个元素的位置上即可，即进行倒序排序。

> 代码

```C++
class Solution {
public:
    int findKthLargest(vector<int>& nums, int k) {
        int len = nums.size();
        int maxIndex;
        // 只排k个元素
        for(int i=0;i<k;i++){
            maxIndex = i;
            for(int j=i;j<len;j++){
                if(nums[j] > nums[maxIndex]){
                    maxIndex = j;
                }
            }

            int t = nums[i];
            nums[i] = nums[maxIndex];
            nums[maxIndex] = t;
        }
        return nums[k-1];
    }
};
```
