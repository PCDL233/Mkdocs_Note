# 归并排序(Merge Sort)

&emsp;&emsp;归并排序是建立在归并操作上的一种有效的排序算法其时间复杂度为$O(nlogn)$,空间复杂度$O(n)$。该算法是采用分治法的一个非常典型的应用。

## 原理

&emsp;&emsp;归并排序的工作原理是：**将数组划分为更小的子数组，对每个子数组进行排序，然后将已排序的子数组合并并返回一个新的排序好的数组，以此类推，最终得到一个有序的数组**。简单来说，归并排序的过程就是将数组分成两半，然后对每一半进行排序，然后将排序好的两半重新合并在一起，重复此过程，直到对整个数组进行排序。

![](./imags/mergeSort_1.gif)

## 实现

**算法步骤**：

- 申请空间，使其大小为两个已经排序序列之和，该空间用来存放合并后的序列；
- 设定两个指针，初始位置分别为两个已经排序序列的起始位置；
- 比较两指针所指向元素的大小，将相对较小的元素合并到开辟的空间中，同时指针移动到下一个指定位置；
- 重复上述步骤，直至指针指向序列尾部；
- 将剩余所有元素合并到开辟的空间中。

&emsp;&emsp;归并排序的经典实现方式就是利用**递归**。另外一种就是迭代，当然，递归与迭代其实差不多，只是当我们使用递归时，我们需要额外考虑栈是否会溢出。

&emsp;&emsp;我们都知道对于**一个元素的数组，一定是有序的**，而这正是我们的递归条件:

```C++
if(start == end){
    return {arr[start]};
}

```

&emsp;&emsp;为了降低空间复杂度，我们选择在原数组上进行划分与排序，使得函数不返回任何数组。因此，递归条件可改为：

```C++
if(start >= end){
    return;
}
```

&emsp;&emsp;那么在不相等时，也就是单层递归的逻辑设计，就是从中间一分为二，对两边子序列进行划分并排序：

```C++
// int mid = (start + end) / 2; 
// 上述表达式可能会发生精度损失，即两数相加超过int范围，因此使用下式较稳妥
int mid = start + (end - start) / 2;
mergeSort(arr,start,mid);
mergeSort(arr,mid+1,end);
```

&emsp;&emsp;之后，我们将划分后的序列进行一个合并

```C++
merge(arr,left,mid,right);
```

&emsp;&emsp;这个合并操作我们可以用单独的函数实现：

```C++
void merge(int arr[],int left,int mid,int right){
    int i,j,k;
    int len1 = mid - left + 1;
    int len2 = right - mid;
    // 两个子序列的临时数组
    int LL[len1],RL[len2];

    for(i=0;i<len1;i++){
        LL[i] = arr[left+i];
    }
    for(j=0;j<len2;j++){
        RL[j] = arr[mid + 1 + j];
    }

    i = j = 0;
    k = left;
    // 将相对较小的元素进行"合并"
    while(i < len1 && j < len2){
        if(LL[i] <= RL[j]){
            arr[k] = LL[i];
            i++;
        }else{
            arr[k] = RL[j];
            j++;
        }
        k++;
    }
    // 将剩下的元素进行"合并"
    while(i < len1){
        arr[k++] = LL[i++];
    }
    while(j < len2){
        arr[k++] = RL[j++];
    }
}
```

**完整代码**

```C++
// 合并
void merge(int arr[],int left,int mid,int right){
    int i,j,k;
    int len1 = mid - left + 1;
    int len2 = right - mid;
    // 两个子序列的临时数组
    int LL[len1],RL[len2];

    for(i=0;i<len1;i++){
        LL[i] = arr[left+i];
    }
    for(j=0;j<len2;j++){
        RL[j] = arr[mid + 1 + j];
    }

    i = j = 0;
    k = left;
    // 将相对较小的元素进行"合并"
    while(i < len1 && j < len2){
        if(LL[i] <= RL[j]){
            arr[k] = LL[i];
            i++;
        }else{
            arr[k] = RL[j];
            j++;
        }
        k++;
    }
    // 将剩下的元素进行"合并"
    while(i < len1){
        arr[k++] = LL[i++];
    }
    while(j < len2){
        arr[k++] = RL[j++];
    }
}
// 划分（分治）
void toMergeSort(int arr[],int left,int right){
    if(left < right){
        int mid = left + (right - left) / 2;
        toMergeSort(arr,left,mid);
        toMergeSort(arr,mid+1,right);
        merge(arr,left,mid,right);
    }
}

void mergeSort(int arr[],int len){
    toMergeSort(arr,0,len-1);
}
```

## 习题


### 习题一

&emsp;&emsp;给定两个排序后的数组 $A$ 和 $B$，其中 $A$ 的末端有足够的缓冲空间容纳 $B$。 编写一个方法，将 $B$ 合并入 $A$ 并排序。初始化 $A$ 和 $B$ 的元素数量分别为 $m$ 和 $n$。

> 思路

&emsp;&emsp;本题基本与归并排序中的归并函数(merge)一样，我们可以将B先直接赋值到A后，再以m为中心，进行归并。（赋值后直接排序也是没有问题的，但这里以归并为主）

> 代码

```C++
class Solution {
public:
    void merge(vector<int>& A, int m, vector<int>& B, int n) {
        // 临时数组
        vector<int> arr1(A.begin(),A.begin()+m);
        vector<int> arr2(B.begin(),B.end());
        // 合并
        int i=0,j=0,k=0;
        while(i < m && j < n){
            if(arr1[i] < arr2[j]){
                A[k] = arr1[i];
                i++;
            }else{
                A[k] = arr2[j];
                j++;
            }
            k++;
        }
        // 将剩余元素合并
        while(i < m){
            A[k++] = arr1[i++];
        }
        while(j < n){
            A[k++] = arr2[j++];
        }
    }
};
```

### 习题二

&emsp;&emsp;在数组中的两个数字，如果前面一个数字大于后面的数字，则这两个数字组成一个逆序对。输入一个数组，求出这个数组中的逆序对的总数。

> 思路

&emsp;&emsp;在归并排序过程中，我们可以将数组中的逆序对数量统计出来。在合并两个递增的有序数组时，如果右边的数字比左边的数字小，则说明左边数组中尚未合并的数字与右边数组的这个数字可以组成逆序对。反之，逆序对数量不增加。

> 代码

```C++
class Solution {
public:
    int ans = 0;
    int reversePairs(vector<int>& nums) {
        int len = nums.size();
        if(len < 2){
            return 0;
        }
        // 此处使用和nums相同大小的临时数组存储归并后的结果，供下一次归并使用
        // 避免每次合并阶段都需要开辟新的空间
        vector<int> temp(len);
        mergeSort(nums,0,nums.size()-1,temp);
        return ans;
    }

    void mergeSort(vector<int>& nums,int left,int right,vector<int>&temp){
        if(left < right){
            int mid = left + (right - left) / 2;
            mergeSort(nums,left,mid,temp);
            mergeSort(nums,mid+1,right,temp);
            merge(nums,left,mid,right,temp);
        }
    }

    void merge(vector<int>& nums,int left,int mid,int right,vector<int>& temp){
        
        int start1 = left,start2 = mid + 1,index = 0;
        while(start1 <= mid && start2 <= right){
            if(nums[start1] <= nums[start2]){
                temp[index++] = nums[start1++];
            }else{
                // 统计逆序对
                ans += mid-start1 + 1;
                temp[index++] = nums[start2++];
            }
        }
        while(start1 <= mid) temp[index++] = nums[start1++];
        while(start2 <= right) temp[index++] = nums[start2++];

        for(int i=left,k=0;i<=right;i++,k++){
            nums[i] = temp[k];
        }
    }
};
```
