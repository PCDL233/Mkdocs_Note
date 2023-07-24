# 线性表

## 1. 线性表的定义
> 零个或多个数据元素的有限序列


## 2. 线性表的顺序存储
> - 定义：用一段连续的存储空间对数据元素进行存储。
> 
> - 根据定义，线性表的顺序存储可以直接用数组进行表示。但是实际上，线性表的一些算法操作并不能单独通过一个数组来实现。
> - 需要一个额外的数据对线性表的长度进行描述，才能使得线性表的算法操作正常执行。
>
> - 顺序存储线性表的构成：一段连续的存储空间 + 用于描述空间的长度的变量
>

## 3. 顺序表的操作集
```C++
#include "bits/stdc++.h" // 万能头文件，math.h，string.h

// typedef old_name new_name; ---> 将old_name 重新命名为 new_name

// 将int重命名为dataType ---> dataType表示数据类型
// 这个int照常可以用。只是之后的程序中，dataType会被看做int
typedef int dataType;
// 将int重命名为Status ---> 用来表示算法执行状态。如果我的算法执行成功，就返回1，否则返回0
typedef int Status;

// #define True 1; ---> 使用宏定义 ---> 出Bug可能性会很高
// const 定义一个int类型的常量，TURE、FALSE --> 1,0
const int TRUE = 1;
const int FALSE = 0;

// 定义顺序表的最大空间
const int MAX = 1000;

// 顺序表的定义 ---> 用结构体将：一段连续的存储空间 和 用于描述空间长度的变量 放在一起
typedef struct Node{
    dataType data[MAX]; // 用于存储数据
    // dataType* data; ---> malloc函数可以动态地开辟出空间 ==> 在链表里具体讲讲
    int length; // 描述线性表长度
}Sqlist;
// 将Struct Node结构体重新命名为Sqlist
// 顺序表在定义完成后，所有对顺序表的算法操作都需要通过我定义出的内容执行。
// (对于当前顺序表)后续的算法实现都是通过data数组和length变量操作的。

// 1. 初始化list ---> 调用该函数，得到一个list表。1. 传入一个数据数组和该数组的长度，直接返回一个Sqlist的东西
Sqlist createList(dataType data[], int length){
    // 得到一个链表
    Sqlist list;
    // 将传入进来的数据数组赋值给我的顺序表中
    for(int i=0;i<length;i++){
        list.data[i] = data[i];
    }
    list.length = length;
    return list;
}

// 2. 判断表是否为空 ---> 若表为空，则返回TRUE，否则返回FALSE
Status isEmpty(Sqlist list){ // list长度为0，list就为空
    // (!list.length)
    if(list.length == 0){
        return TRUE; // 表示空
    }else{
        return FALSE; // 表示不为空
    }
}

// 3. 销毁表 --->
// 如果用动态数组定义的顺序表 -- > malloc函数开辟 用free函数释放
// 这里使用的是静态数组的线性表
Status deleteList(Sqlist* list){
    if(list==NULL){
        return FALSE;
    }
    list->length = 0;
    return TRUE;
}

// 4. 增 --> 根据位置插入元素
Status insertElem(Sqlist* list, int index, dataType elem ){
    // 判断插入位置是否合法
    // 插入范围(0 - length-1)
    if(index < 0 || index > list->length -1 ){
        return FALSE;
    }

    // 移位
    for(int i=list->length-1;i>=index;i--){
        list->data[i+1] = list->data[i];
    }
    // 插入
    list -> data[index] = elem;
    // 插入完成之后，线性表的长度加一
    list -> length++;
    return TRUE;
}

// 5. 删 ---> 根据索引删除元素，并用一个变量e保存删除的值
Status deleteElem(Sqlist* list,int index,dataType *e){
    if(index < 0 || index > list->length-1){
        return FALSE;
    }
    *e = list->data[index];
    // 移位
    for(int i = index; i < list->length; i++){
        list->data[i] = list->data[i+1];
    }
    // 删除完之后，线性表的长度减一
    list->length--;
    return TRUE;
}

// 6. 改 ---> 根据索引修改元素
Status updateElem(Sqlist* list, int index, dataType e){
    if(index < 0 || index > list->length-1){
        return FALSE;
    }
    list->data[index] = e;
    return TRUE;

}

// 7. 查 ---> 根据数据元素来进行查询 e --> 返回e在顺序表中第一次出现的位置
// return list->data[idnex]
Status searchElem(Sqlist* list,dataType e){
    for(int i=0;i<list->length;i++){
        if(list->data[i] == e){
            return i;
        }
    }
    return -1;
}



// 8. 遍历 ---> 打印顺序表中的所有元素
void display(Sqlist list)
{
    // list的长度是list.length,数据是list.data数组。
    for(int i=0;i<list.length;i++){
        printf("%d ",list.data[i]);
    }
    printf("\n");
}


int main(){
    system("chcp 65001");
    dataType datas[] = {4,5,6,3,7,3};
    Sqlist list = createList(datas,6);
    display(list);
    // &变量 --> 取出变量的地址 scanf("%d",&a) --> 访问变量a的地址，并将缓存区的数据赋值给相应的格式站位符上。
    // *地址 --> 访问地址所在的空间
    // deleteList(&list);
    insertElem(&list,3,0);
    display(list);
    dataType e;
    deleteElem(&list,5,&e);
    display(list);
    printf("e=%d\n",e);
    updateElem(&list,3,10);
    display(list);
    printf("10‘s index = %d\n", searchElem(&list,10));
    printf("100's index = %d\n",searchElem(&list,100));
    return 0;
}

```