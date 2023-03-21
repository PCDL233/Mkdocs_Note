###### 数据结构

###### 宏定义

###### 1. 线性表

###### 顺序表(Sequence List)

###### 初始化

###### 获取元素

###### 查找元素

###### 插入

###### 删除

###### 销毁，清空，检查为空

###### 顺序表的头文件

###### 单链表(Single Linked List)

###### 初始化

###### 创建链表(头插法)

###### 创建链表(尾插法)

###### 获取元素

###### 查找元素

###### 插入元素

###### 删除元素

###### 总结插入和删除操作算法的不同

###### 销毁链表

###### 单链表头文件

###### 循环链表(Circular Linked List)

###### 双向链表(Double Linked List)

###### 初始化

###### 创建双向链表

###### 插入和删除

###### 线性表玩具

###### 线性表合并

###### 有序表合并(并归排序的基础)

###### 有序链表合并

###### 多项式创建 and 多项式相加

###### 2. 栈和队列(Stack and Queue)

###### 顺序栈(Sequence Stack)

###### 栈的类型定义

###### 栈的初始化

###### 入栈(Push)

###### 出栈(Pop)

###### 栈的其他操作

###### 测试代码

###### 链栈(Linked Stack)

###### 链栈的类型定义

###### 链栈初始化

###### 链栈Push

###### 链栈Pop

###### 链栈的其他操作

###### 测试代码

###### Stack.h

###### 栈与递归


###### 函数的调用过程

###### 循环队列

###### 顺换队列初始化

###### 顺换队列入队

###### 循环队列出队

###### 循环队列其他操作

###### 测试代码

###### 链队

###### 链队初始化

###### 链队入队

###### 链队出队

###### 栈和队列玩具

###### 进制转化

###### 括号的匹配

###### 10 以内的计算器

###### 3. 字符串，数组，广义表

###### 字符串匹配

###### BF算法(Brute Force)

###### KMP算法

###### 求next数组

###### 字符串匹配玩具

###### 数组

###### 广义表(Generalized List)

###### 4. 树、二叉树、森林

###### 定义

###### 树的基本术语

###### 二叉树的定义

###### 二叉树的性质

###### 二叉树定理

###### 完全二叉树性质及定理

###### 链式二叉树

###### 存储结构

###### 遍历方式(递归)

###### 遍历方式(非递归)

###### 先序遍历创建二叉树

###### 测试(创建，遍历)

###### 层次遍历算法

###### 复制二叉树

###### 求深度和节点数

###### 销毁二叉树(递归和非递归)

###### 头文件

###### 线索二叉树 Threaded Binary Tree(了解即可)

###### 数据类型定义

###### 树和森林

###### 树的存储结构

###### 1. 双亲表示法

###### 2. 孩子链表

###### 3. 孩子兄弟表示法(树转化二叉树的基础)

###### 树与二叉树之间相互转换

###### 树转二叉树


###### 二叉树转树

###### 森林与二叉树之间的转化

###### 森林转二叉树

###### 二叉树转森林

###### 树和森林的遍历

###### 树的遍历

###### 森林的遍历

###### 哈夫曼树

###### 术语

###### 最优二叉树

###### 构造哈夫曼树

###### step和定理

###### 代码实现

###### 哈夫曼编码

###### 代码实现

###### 整体头文件

###### 5. 图(Graph)

###### 图的定义和术语

###### 完全图

###### 稀疏图(Sparse Graph)和稠密图(Dense Gaph)

###### 顶点的度(degree)

###### 路径(path)

###### 连通图(Connected Graph)

###### 连通子图和连通分量(Connected Component)

###### 极小连通子图和生成树(Spanning Tree)

###### 图的存储结构

###### 邻接矩阵(Adjacency Matrix)

###### 无向图

###### 有向图

###### 带权图(网) weighted Graph

###### 代码实现

###### 无向无权图

###### 无向带权图

###### 有向带权图

###### 有向无权图

###### 邻接表(Adjacency List)

###### 代码实现

###### 无向无权图

###### 邻接表和邻接矩阵的比较

###### 十字链表

###### 邻接多重链表

###### 图的遍历

###### 深度优先 (Depth First Search)

###### 遍历矩阵

###### 遍历邻接表

###### 广度优先 (Breadth First Search)

###### 遍历矩阵

###### 遍历邻接表

###### 算法效率

###### 最小生成树 Spanning Tree


###### Prim 算法

###### 代码实现

###### 邻接矩阵

###### 邻接表

###### Kruskal 算法

###### 代码实现

###### 邻接矩阵

###### 邻接表

###### 最短路径

###### Dijkstra 算法

###### 代码实现

###### 邻接矩阵

###### Floyd算法

###### 代码实现

###### 邻接矩阵

###### 有向无环图(Directed Acycline Graph)

###### AOC和AOE

###### 拓扑排序

###### 代码实现

###### 邻接表

###### 关键路径

###### 代码实现

###### 邻接表

###### 图的头文件

###### define_Graph.h

###### AMGraph.h

###### ALGraph.h


# 数据结构

## 宏定义

###### 在本笔记中用到的宏定义，头文件为define.h

## 1. 线性表

## 顺序表(Sequence List)

###### 特点：逻辑上相邻的数据元素，其物理次序也是相邻的

###### 线性表中第 个数据元素的存储位置 和第个元素满足下列关系

###### 代表每个元素所占的存储单元

###### 循序表的存储结构：

## 初始化

```
#ifndef __DEFINE_H
#define __DEFINE_H
```
```
#define TRUE 1
#define FALSE 0
#define OK 1
#define ERROR 0
#define INFEASIBLE -
#define OVERFLOW -
typedef int Status;
```
```
#endif
```
```
#define SQLMAXSIZE 100
typedef int SqlElemType;
typedef struct __Sqlist {
SqlElemType *base;
int length;
} Sqlist;
```

#### 获取元素

#### 查找元素

###### 平均查找长度ASL(Average Search Length)

###### 为查找第个元素成功的概率

###### 为查找第个元素需要比较的次数

###### 可知

###### 为第个元素在表中位置

###### 因此可知 的时间复杂度为

```
Status InitSL(Sqlist *L, int length) {
L->base = (SqlElemType *)malloc(sizeof(SqlElemType) * SQLMAXSIZE);
if (!L->base)
return OVERFLOW;
L->length = 0 ;
```
```
for (int i = 1 ; i < length + 1 ; i++) {
SqlElemType e;
scanf(" %d", &e);
SqlInsert(L, i, e);
}
return OK;
}
```
```
Status GetElem(Sqlist *L, int position, SqlElemType *e) {
if (position < 1 || position > L->length)
return ERROR;
*e = L->base[position - 1 ];
return OK;
}
```
```
int LocateElem(Sqlist *L, SqlElemType e) {
for (int i = 0 ; i < L->length; i++) {
if (e == L->base[i])
return i + 1 ;
}
return 0 ; // 0代表查找元素不在循序表中
}
```

#### 插入

###### 表示插入元素所需要移动元素次数的期望值平均次数

###### 假设在各个位置上插入元素的概率相等

###### 因此

#### 删除

#### 销毁，清空，检查为空

```
Status SqlInsert(Sqlist *L, int position, SqlElemType e) {
if (position < 1 || position > L->length + 1 )
return ERROR;
if (L->length == SQLMAXSIZE)
return OVERFLOW;
for (
int i = L->length - 1 ; i >= position - 1 ;
i--) { //注意需要把数组中的元素全部向右移动，需要从数组最右边的元素开始移动
L->base[i + 1 ] = L->base[i];
}
L->base[position - 1 ] = e;
L->length++;
return OK;
}
```
```
Status SqlDelete(Sqlist *L, int position, SqlElemType *e) {
if (position < 1 || position > L->length)
return ERROR;
for (int i = position; i < L->length; i++) {
L->base[i - 1 ] = L->base[i];
}
*e = L->base[position - 1 ];
L->length--;
return OK;
}
```
```
Status SqlDelete(Sqlist *L, int position, SqlElemType *e) {
if (position < 1 || position > L->length)
return ERROR;
for (int i = position; i < L->length; i++) {
L->base[i - 1 ] = L->base[i];
```

#### 顺序表的头文件

```
}
*e = L->base[position - 1 ];
L->length--;
return OK;
}
```
```
Status SqlDestroy(Sqlist *L) {
if (!L->base)
return ERROR;
else {
free(L->base);
return OK;
}
}
```
```
void SqlClear(Sqlist *L) { L->length = 0 ; }
```
```
Status SqlIsEmpty(Sqlist *L) {
if ( 0 == L->length)
return TRUE;
else
return FALSE;
}
```
```
#include "define.h"
#include <stdio.h>
#include <stdlib.h>
```
```
#ifndef __SEQUENCELIST_H
#define __SEQUENCELIST_H
```
```
#define SQLMAXSIZE 100
typedef int SqlElemType;
typedef struct __Sqlist {
SqlElemType *base;
int length;
} Sqlist;
```
```
Status InitSL(Sqlist *L, int length);
Status GetElem(Sqlist *L, int position, SqlElemType *e);
int LocateElem(Sqlist *L, SqlElemType e);
Status SqlInsert(Sqlist *L, int position, SqlElemType e);
Status SqlDelete(Sqlist *L, int position, SqlElemType *e);
Status SqlDestroy(Sqlist *L);
void SqlClear(Sqlist *L);
Status SqlIsEmpty(Sqlist *L);
void MergeList(Sqlist *La, Sqlist *Lb);
void Traverse(Sqlist *L);
void MergeList_Seq(Sqlist *La, Sqlist *Lb, Sqlist *Lc);
```

### 单链表(Single Linked List)

###### 单链表由头节点(不存放数据只存放下个节点的地址)和n个节点组成，

###### 每个节点分为两个域：数据域和指针域(存放下个节点的地址)

###### 第n个节点的指针域为NULL

###### 如下图所示

#### 初始化

#### 创建链表(头插法)

```
#endif
```
```
typedef int LlElemtype;
typedef struct __LNode {
LlElemtype data; //存放单个节点的数据
__LNode *next; //存放下个节点的地址
} LNode, *LinkList;
```
```
Status InitLL(LinkList *L) // L是个二级指针
{
(*L) = (LinkList)malloc(sizeof(LNode));
(*L)->next = NULL;
return OK;
}
```
```
void CreatLL_H(LinkList L, int n)
//用此方法创建的链表，遍历的顺序和创建的顺序相反
{
printf("Please input %d numbers:", n);
for (int i = 0 ; i < n; i++) {
LinkList p = (LinkList)malloc(sizeof(LNode));
int data;
scanf(" %d", &data); //%d前面的空格代表清除制表符回车等符号
p->data = data;
p->next = L->next;
L->next = p;
}
}
```

#### 创建链表(尾插法)

#### 获取元素

#### 查找元素

#### 插入元素

```
void CreatLL_R(LinkList L, int n) {
printf("Please input %d numbers:", n);
LinkList ptail;
ptail = L;
for (int i = 0 ; i < n; i++) {
LinkList pnew;
pnew = (LinkList)malloc(sizeof(LNode));
int data;
scanf(" %d", &data);
pnew->data = data;
pnew->next = NULL;
ptail->next = pnew;
ptail = pnew;
}
}
```
```
Status GetElem(LinkList L, int position, LlElemtype *e) {
LinkList p = L->next;
int i = 1 ; //使i和p的位置同步，即i代表着p在链表中的位置
if (position < 1 || !p)
return ERROR;
while (p && i < position) { //此处不可 i<=position,因为while成立时，内部会i++
p = p->next;
i++;
}
*e = p->data;
```
```
return OK;
}
```
```
LinkList LocateElem(LinkList L, LlElemtype e) {
LinkList p = L->next;
while (p && p->data != e) {
p = p->next;
}
if (!p)
return NULL; //如果p的地址为空 说明e不在链表中
return p;
}
```

##### 想在 ， 之间插入 ,需要先知道 节点的地址

###### 如图所示，如果想要在位置 插入节点，则需要知道位置 节点的位置

###### 注意因为插入操作和GetElem操作不同

###### 要从 0 开始，p要从L开始

###### 如果从 1 和L开始的话，无法再位置 1 插入元素

#### 删除元素

###### 想要删除 ，则必须先知道 的地址

###### 注意因为插入操作和GetElem操作不同

###### 要从 0 开始，p要从L开始

###### 如果从 1 和L开始的话，无法再位置 1 插入元素

```
Status LlInsert(LinkList L, int position, LlElemtype e) {
LinkList p = L; //注意因为插入操作和GetElem操作不同
int i = 0 ; // i要从 0 开始，p要从L开始
//如果从 1 和L开始的话，无法再位置 1 插入元素
while (p && i < position - 1 ) { //查找插入节点位置的前一个节点
i++;
p = p->next;
}
if (!p || i > position - 1 )
return ERROR;
```
```
LinkList pnew = (LinkList)malloc(sizeof(LNode));
pnew->data = e;
pnew->next = p->next;
p->next = pnew;
return OK;
}
```

#### 总结插入和删除操作算法的不同

```
Status LlDelete(LinkList L, int position, LlElemtype *e) {
LinkList p = L;
int i = 0 ;
```
```
while (p && i < position - 1 ) {
//查找posision-1位置节点的地址
i++;
p = p->next;
}
if (i > position - 1 || !p || !p->next)
return ERROR;
//注意是 多增加了判断条件!(p->next) 当节点数为n，删除的位置为n+1时会返回error
```
```
LinkList pfree = p->next;
*e = pfree->data;
p->next = pfree->next; //此处可改写成 p->next = p->next->next;
free(pfree);
return OK;
}
```
```
while (p){
p = p->next;
}//最终p的值为NULL
```
```
while(p->next){
p = p->next;
}//最终p的值为最后一个节点的地址
//---------------------插入----------------------
//如果插入操作的position不合法，即position > n+1(n为链表长度)，那么p一定会指向NULL，此时按照
退出条件!p可以返回ERROR
if (!p || i>position- 1 ) return ERROR;
//但是如果采用:
while(p->next)
//则最终会指向链表最后一个节点，即使position不合法，那么也会在最后一个节点后方插入新节点
//所以使用:
while(p)
```
```
////---------------------删除----------------------
//如果删除操作的positoin不合法，即position>链表长度，p会指向，最后一个节点的地址(position ==
n+1时)或是NULL(position > n+1)，那么下面的代码会出错
LinkList pfree = p->next;
//如果p指向最后一个节点，此时pfree指向NULL。如果p指向NULL，此时pfree指向非法空间(不受主程序控
制)，从而导致下面代码报错
*e = pfree->data;
//所以需要增加一个判断条件
```

#### 销毁链表

#### 单链表头文件

```
if (i>position- 1 || !p || !p->next) return ERROR;
//必须保证 !p 要在 !p->next的左边，即position > n+1 的情况
//这是因为如果 !p->next 在 !p 的左边，如果p指向NULL，那么NULL->next会报错
```
```
Status LlDestroy(LinkList *L) {
if (!(*L))
return ERROR;
LinkList p = *L;
while (p) {
LinkList pfree = p; // pfree保存要释放的节点地址
p = p->next; //此行和下行的顺序不能反
free(pfree);
pfree = NULL;
}
*L = NULL;
return OK;
}
```
```
#include "define.h"
#include <stdio.h>
#include <stdlib.h>
```
```
#ifndef __LINKLIST_H
#define __LINKLIST_H
```
```
typedef int LlElemtype;
typedef struct __LNode {
LlElemtype data; //存放单个节点的数据
__LNode *next; //存放下个节点的地址
} LNode, *LinkList;
```
```
Status InitLL(LinkList *L);
void CreatLL_H(LinkList L, int n);
void CreatLL_R(LinkList L, int n);
Status GetElem(LinkList L, int position, LlElemtype *e);
LinkList LocateElem(LinkList L, LlElemtype e);
Status LlInsert(LinkList L, int position, LlElemtype e);
Status LlDelete(LinkList L, int position, LlElemtype *e);
void Traverse(LinkList L);
Status LlDestroy(LinkList *L);
void Merge_LinkedList(LinkList *La, LinkList *Lb, LinkList *Lc);
#endif
```

### 循环链表(Circular Linked List)

###### 循环链表的特点：

###### 最后一个节点的指针域指向头节点，整个表链形成一个环

###### 由此，从表中任意节点出发，可以找到其他节点

###### 和单链表很像，区别就是最后一个节点的next域指向头节点

### 双向链表(Double Linked List)

###### 有两个指针域，一个指向直接前驱，另一个指向直接后继

###### 数据类型

#### 初始化

#### 创建双向链表

```
typedef int DouLElemtype;
typedef struct __DouLinkNode {
DouLElemtype data;
__DouLinkNode *prior;
__DouLinkNode *next;
} DouLinkNode, *DouLinkList;
```
```
void InitDL(DouLinkList *L) {
*L = (DouLinkList)malloc(sizeof(DouLinkNode));
(*L)->next = NULL;
(*L)->prior = NULL;
}
```
```
void CreatDL_H(DouLinkList L, int length) {
for (int i = 0 ; i < length; i++) {
DouLinkList pnew = (DouLinkList)malloc(sizeof(DouLinkNode));
int data;
printf("(for %d)Please input the data:", i + 1 );
scanf("%d", &data);
pnew->data = data;
pnew->next = L->next;
pnew->prior = L;
L->next = pnew;
```

#### 插入和删除

```
}
}
```
```
void CreatDL_R(DouLinkList L, int length) {
DouLinkList ptail = L;
for (int i = 0 ; i < length; i++) {
DouLinkList pnew = (DouLinkList)malloc(sizeof(DouLinkNode));
int data;
printf("(for %d)Please input the data:", i + 1 );
scanf("%d", &data);
pnew->data = data;
pnew->next = NULL;
pnew->prior = ptail;
ptail->next = pnew;
ptail = pnew;
}
}
```
```
void DlInsert(DouLinkList L, int position, DouLElemtype e) {
int i = 0 ;
DouLinkList p = L;
while (p->next && i < position - 1 ) {
i++;
p = p->next;
}
DouLinkList pnew = (DouLinkList)malloc(sizeof(DouLinkNode));
pnew->data = e;
pnew->next = p->next;
pnew->prior = p;
p->next = pnew;
p->next->prior = pnew;
}
```
```
void DlDelete(DouLinkList L, int position, DouLElemtype *e) {
DouLinkList p = L;
int i = 0 ;
while (p->next && i < position - 1 ) {
p = p->next;
i++;
}
DouLinkList pfree = p->next;
*e = pfree->data;
p->next = p->next->next;
p->next->next->prior = p;
free(pfree);
pfree = NULL;
}
```

### 线性表玩具

#### 线性表合并

###### 已知两个集合

###### 求出合并后集合

#### 有序表合并(并归排序的基础)

```
void MergeList(Sqlist *La, Sqlist *Lb) {
for (int i = 1 ; i < Lb->length + 1 ; i++) {
SqlElemType e;
GetElem(Lb, i, &e);
if (!LocateElem(La, e)) {
La->base[La->length++] = e;
}
}
}
```
```
void Traverse(Sqlist *L) {
for (int i = 0 ; i < L->length; i++) {
printf("%d ", L->base[i]);
}
}
```
```
#include <SequenceList.h>
```
```
int main(void) {
Sqlist La, Lb;
Sqlist *pa = &La;
Sqlist *pb = &Lb;
InitSL(pa, 4 );
InitSL(pb, 3 );
```
```
MergeList(pa, pb);
```
```
Traverse(pa);
```
```
system("pause");
return 0 ;
}
/*
7 5 3 11
2 6 3
*/
```

###### 合并成新集合

#### 有序链表合并

```
void MergeList_Seq(Sqlist *La, Sqlist *Lb, Sqlist *Lc) {
Lc->length = La->length + Lb->length;
SqlElemType *pa = La->base, *pa_last = pa + La->length - 1 ;
// pa指向La->base的首地址，pa_last指向base中最后一个元素的地址，下面同理
SqlElemType *pb = Lb->base, *pb_last = pb + Lb->length - 1 ;
SqlElemType *pc = Lc->base;
```
```
while (pa <= pa_last && pb <= pb_last) {
//当pa>pa_last时说明，有集合中的元素已经全部加入到Lc中
if (*pa < *pb)
*(pc++) = *(pa++);
else
*(pc++) = *(pb++);
}
```
```
while (pa <= pa_last)
*(pc++) = *(pa++); //判断La的元素是否全部加入Lc中，下面同理
while (pb <= pb_last)
*(pc++) = *(pb++);
}
```
```
#include <SequenceList.h>
```
```
int main(void) {
Sqlist La, Lb, Lc;
InitSL(&La, 4 );
InitSL(&Lb, 7 );
InitSL(&Lc, 0 );
```
```
MergeList_Seq(&La, &Lb, &Lc);
Traverse(&Lc);
```
```
system("pause");
return 0 ;
}
/*
3 5 8 11
2 6 8 9 11 15 20
*/
```
```
void Merge_LinkedList(LinkList *La, LinkList *Lb, LinkList *Lc) {
*Lc = *La; //让Lc使用La的头节点进行合并
LinkList pa = (*La)->next, pb = (*Lb)->next; // pa, pb分别表示合并时所指节点
```

#### 多项式创建 and 多项式相加

###### 创建一个多项式，并按照指数的高低排序

###### 多项式结构体

###### 多项式创建

```
LinkList pc = *Lc; // pc表示Lc的尾节点
```
```
while (pa && pb) {
if (pa->data < pb->data) {
pc->next = pa;
pc = pa;
pa = pa->next;
} else {
pc->next = pb;
pc = pb;
pb = pb->next;
}
}
pc->next = pa? pa : pb;
// pc->next不需要NULL,因为合并时一定会剩下一串节点，只需指向该剩下的节点就OK
free(*Lb);
*La = *Lb = NULL;
}
```
```
#include "LinkList.h"
```
```
int main(void) {
LinkList La, Lb, Lc;
InitLL(&La), InitLL(&Lb), InitLL(&Lc);
CreatLL_R(La, 4 );
CreatLL_R(Lb, 7 );
Merge_LinkedList(&La, &Lb, &Lc);
```
```
Traverse(Lc);
```
```
system("pause");
return 0 ;
}
/*
3 5 8 11
2 6 8 9 11 15 20
*/
```
```
typedef struct __PolyNode {
double coeffcient;
int exponent;
__PolyNode *next;
} PolyNode, *Polynomial;
```

###### 核心变量为 Polynomial q; Polynimial pre;

###### 核心语句为 while(q && q->exponent < pnew->exponent)

###### 主程序

```
void InitPolynomial(Polynomial *p, int length) {
*p = (Polynomial)malloc(sizeof(PolyNode)); //先初始化头节点
(*p)->next = NULL;
```
```
printf("Please input the coefficient and exponent:");
for (int i = 0 ; i < length; i++) {
Polynomial pnew = (Polynomial)malloc(sizeof(PolyNode));
scanf(" %lf", &(pnew->coeffcient));
scanf(" %d", &(pnew->exponent));
Polynomial q = (*p)->next; // q为指向比pew->exponent大的节点
Polynomial pre = (*p); // pre指向q的直接前驱节点
```
```
while (q && q->exponent < pnew->exponent) { //第 1 次的for循环不会执行
//直到找到一个节点的exponent大于pnew->exponent,如果没找到q指向NULL
pre = q;
q = q->next;
}
pnew->next = q; //因为q->exponent > pnew->exponent
pre->next = pnew;
}
}
```
```
#include <stdio.h>
#include <stdlib.h>
```
```
typedef struct __PolyNode {
double coeffcient;
int exponent;
__PolyNode *next;
} PolyNode, *Polynomial;
```
```
void InitPolynomial(Polynomial *p, int length);
void Traverse(Polynomial P);
Polynomial AddPolynomial(Polynomial pa, Polynomial pb);
int main(void) {
Polynomial p1, p2, p3;
InitPolynomial(&p1, 3 );
InitPolynomial(&p2, 4 );
p3 = AddPolynomial(p1, p2);
Traverse(p1);
```

## 2. 栈和队列(Stack and Queue)

### 顺序栈(Sequence Stack)

###### 栈是限定仅在表尾进行插入或删除操作的线性表，表末端为栈顶(Top)，表头称为栈顶(Bottom),不含元

###### 素称为空战

###### (用顺序表存储的栈更常见)

###### 因此栈又称为后进先出(Last in First out, LIFO)的线性表，如下图

#### 栈的类型定义

```
system("pause");
return 0 ;
}
/*
x^6+2x^2+3x^
-2x^2+3x^5+2x^6+x^
---------------------------
intput:
1 6 2 2 3 5
-2 2 3 5 2 6 1 3
----------------------------
output:
(1.0x^3)+(6.0x^5)+(3.0x^6)
*/
```

#### 栈的初始化

###### 观察上图，发现top指向内存空间不存放元素

#### 入栈(Push)

###### 因为top指向的内存不存放空间，当为base分配的空间存满元素时，top = 分配空间的最后一个元素的

###### 地址+1，此时表示栈满，即top-base = stacksize

```
#define MAXSTACK 100
typedef char StackElemType; //栈数据类型
typedef struct __SqStack //顺序栈，最常用
{
StackElemType *base;
StackElemType *top;
int stacksize;
} SqStack;
```
```
Status InitStack(SqStack *S) {
S->base = (StackElemType *)malloc(sizeof(StackElemType) * MAXSTACK);
if (!S->base)
exit(OVERFLOW);
S->top = S->base; //栈顶和指向栈底
S->stacksize = MAXSTACK; //栈的容量
return OK;
}
```
```
Status Push(SqStack *S, StackElemType e) {
if (S->top - S->base == S->stacksize)
return ERROR; //表示此时栈满
*(S->top++) = e; // top指向内存单元存放e，且top指向下一个内存单元
return OK;
}
```

#### 出栈(Pop)

###### 当 base == top 时，表示栈空

#### 栈的其他操作

#### 测试代码

```
Status Pop(SqStack *S, StackElemType *e) {
if (S->base == S->top)
return ERROR; //栈空
*e = *(--(S->top));
return OK;
}
```
```
Status IsEmpty(SqStack *S) {
if (S->base == S->top)
return TRUE;
else
return FALSE;
}
```
```
Status IsFull(SqStack *S) {
if (S->top - S->base == S->stacksize)
return TRUE;
else
return ERROR;
}
```
```
StackElemType GetTop(SqStack *S) {
if (!IsEmpty(S))
return *(S->top - 1 );
}
```
```
#include <Stack.h>
```
```
int main(void)
{
SqStack S;
InitStack(&S);
Push(&S, 'A');
Push(&S, 'B');
Push(&S, 'C');
Push(&S, 'C');
while (!IsEmpty(&S))
{
StackElemType e;
Pop(&S, &e);
printf("%c ", e);
}
```
```
system("pause");
```

### 链栈(Linked Stack)

###### 由于栈的主要操作是对栈顶进行Push和Pop，所以选用top作为链表的头节点

#### 链栈的类型定义

#### 链栈初始化

#### 链栈Push

```
在第一次Push时，第一个节点的next指向NULL
```
```
return 0 ;
}
```
```
typedef struct __StackNode //链栈
{
StackElemType data;
__StackNode *next;
} StackNode, *LinkStack;
```
```
Status InitStack(LinkStack *S) {
*S = NULL;
//(*S)->next = NULL; 不需要此行代码
return OK;
}
```

#### 链栈Pop

#### 链栈的其他操作

```
Status Push(LinkStack *S, StackElemType e) {
LinkStack pnew = (LinkStack)malloc(sizeof(StackNode));
pnew->data = e;
pnew->next =
*S; //在第一次Push时，第一个节点的next指向NULL，因为初始化了*S=NULL;
*S = pnew;
return OK;
}
```
```
Status Pop(LinkStack *S, StackElemType *e) {
LinkStack pfree = *S; //临时保存栈顶节点S
*e = (*S)->data;
*S = (*S)->next;
free(pfree); //出栈后释放
return OK;
}
```
```
StackElemType GetTop(LinkStack *S) {
if (*S)
return (*S)->data;
}
```
```
Status IsEmpty(LinkStack *S) {
if (!(*S))
return TRUE;
else
return FALSE;
}
```

#### 测试代码

#### Stack.h

```
#include "Stack.h"
```
```
int main(void)
{
LinkStack S;
InitStack(&S);
Push(&S, 'E');
Push(&S, 'A');
Push(&S, 'C');
Push(&S, 'H');
Push(&S, 'R');
while (!IsEmpty(&S))
{
StackElemType e;
Pop(&S, &e);
printf("%c ", e);
}
system("pause");
return 0 ;
}
```
```
#include "define.h"
#ifndef _STACK_H
#define _STACK_H
//-----------------------------------------------------
#define MAXSTACK 100
typedef char StackElemType; //栈数据类型
typedef struct __SqStack //顺序栈，最常用
{
StackElemType *base;
StackElemType *top;
int stacksize;
} SqStack;
```
```
Status InitStack(SqStack *S);
Status Push(SqStack *S, StackElemType e);
Status Pop(SqStack *S, StackElemType *e);
Status IsEmpty(SqStack *S);
Status IsFull(SqStack *S);
StackElemType GetTop(SqStack *S);
//---------------------------------------------------------
typedef struct __StackNode //链栈
{
StackElemType data;
__StackNode *next;
} StackNode, *LinkStack;
```
```
Status InitStack(LinkStack *S);
Status Push(LinkStack *S, StackElemType e);
Status Pop(LinkStack *S, StackElemType *e);
StackElemType GetTop(LinkStack *S);
```

### 栈与递归

#### 函数的调用过程

###### 调用前系统完成：

###### 1. 将实参，返回地址(下行代码地址)等传递给被调用函数

###### 2. 为被调用函数的局部变量分配空间

###### 3. 将控制转移到被调用函数的入口

###### 调用后，系统完成：

###### 1. 保存被调用函数的计算结果(返回值)

###### 2. 释放被调用函数的数据区

###### 3. 依照被调用函数保存的返回地址，将控制转移到调用函数

###### 递归调用函数时，如下图

###### 按照调用顺序依此把各个函数入栈

###### 当栈顶函数满足return条件时，依此出栈(按照FISLO原则)，并且返回值从上向下传递

###### 直到主程序调用的fact(4)出栈后，递归完成

```
Status IsEmpty(LinkStack *S);
#endif
```

### 循环队列

###### 定义：只能在表的一端进行插入运算，在表的另一端进行删除运算的 线性表

###### 先进先出(First in Firs out)原则

###### 数据类型定义

###### 如上图，(d)虽然数组中的空间没有满，但是rear却不能继续增加，假溢出

###### 解决方法：把base数组想象成一个环形的循环队列如下图

###### 此时如果 front == rere表示 队空 ，而 front == (rere+1) % QMAXSIZE时表示 队满

#### 顺换队列初始化

###### 把 front 和 rere 初始化为 0

```
#define QMAXSIZE 100
typedef char QElemType;
typedef struct __SqQueue {
QElemType *base;
int front, rere; //front为队头下标，rere为队尾下标(rere下标的位置不存放元素)
} SqQueue;
//入队rere+1,出队front+1,但是此种情况存在问题，如下图
```
```
Status InitQueue(SqQueue *Q) {
if (!(Q->base = (QElemType *)malloc(sizeof(QElemType) * QMAXSIZE)))
exit(OVERFLOW);
Q->front = Q->rere = 0 ;
return OK;
}
```

#### 顺换队列入队

#### 循环队列出队

#### 循环队列其他操作

```
Status EntryQ(SqQueue *Q, QElemType e) {
if ((Q->rere + 1 ) % QMAXSIZE == Q->front) //判断是否队满
return ERROR;
Q->base[Q->rere] = e;
Q->rere = (Q->rere + 1 ) % QMAXSIZE; // Q->rere++ 错误写法
return OK;
}
```
```
Status OutQ(SqQueue *Q, QElemType *e) {
if (Q->rere == Q->front) //判断是否队满
return ERROR;
*e = Q->base[Q->front];
Q->front = (Q->front + 1 ) % QMAXSIZE; // Q->front++; 为错误写法
return OK;
}
```
```
Status IsEmpty(SqQueue *Q) {
if (Q->front == Q->rere)
return TRUE;
else
return FALSE;
}
```
```
Status IsFull(SqQueue *Q) {
if ((Q->rere + 1 ) % QMAXSIZE == Q->front)
return TRUE;
else
return FALSE;
}
```
```
Status GetFront(SqQueue *Q, QElemType *e) {
if (IsEmpty(Q))
return ERROR;
*e = Q->base[Q->front];
return OK;
}
```
```
int LengthQueue(SqQueue *Q) {
return (Q->rere - Q->front + QMAXSIZE) % QMAXSIZE;
}
```

#### 测试代码

### 链队

###### 链队结构类似于链表，不同于链表的头指针，用两个指针域 front rere 来表示队列，如下图

###### 数据类型定义：

```
#include "Queue.h"
```
```
int main(void) {
SqQueue Q;
InitQueue(&Q);
EntryQ(&Q, 'A');
EntryQ(&Q, 'B');
EntryQ(&Q, 'N');
EntryQ(&Q, 'M');
printf("%d\n", LengthQueue(&Q));
QElemType e;
while (!(IsEmpty(&Q))) {
OutQ(&Q, &e);
printf("%c ", e);
}
system("pause");
return 0 ;
}
```
```
typedef struct __QueueNode {
QElemType data;
__QueueNode *next;
} QueueNode;
typedef struct __LinkedQueue {
QueueNode *front;//front相当于链表的头指针
QueueNode *rere;//rere指向整个链表的最后一个节点
} LinkedQueue;
```

#### 链队初始化

#### 链队入队

#### 链队出队

```
Status InitQueue(LinkedQueue *Q) {
// front rere 指向同一节点
if (!(Q->front = Q->rere = (QueueNode *)malloc(sizeof(QueueNode))))
exit(OVERFLOW);
Q->front->next = NULL; //使该节点next域为NULL
return OK;
}
```
```
Status EntryQ(LinkedQueue *Q, QElemType e) {
QueueNode *pnew = (QueueNode *)malloc(sizeof(QueueNode));
if (!pnew)
exit(OVERFLOW);
pnew->data = e;
pnew->next = NULL;
Q->rere->next = pnew;
Q->rere = pnew;
return OK;
}
```

### 栈和队列玩具

#### 进制转化

###### 一个进转换函数，有一个参数n(十进制)，要求输出n的 8 进制

#### 括号的匹配

###### 输入括号()[]，判断括号是否匹配成功，#字符表示输入结束

###### 例: ([()])成功 [(())]] 失败

###### 写法 1 ：

```
Status OutQ(LinkedQueue *Q, QElemType *e) {
if (Q->front == Q->rere)
return ERROR;
QueueNode *pfree = Q->front->next;
*e = pfree->data;
Q->front->next = pfree->next;
//如果删除的节点为队尾，那么释放pfree之后，rere指向未知存储空间
if (Q->rere == pfree)
Q->rere = Q->front;
free(pfree);
return OK;
}
```
```
//需要提前修改 StackElemType的类型
void Convert_8(int n) {
SqStack S;
InitStack(&S);
```
```
int temp = n;
while (temp) {
Push(&S, temp % 8 );
temp = temp / 8 ;
}
```
```
while (!IsEmpty(&S)) {
int i;
Pop(&S, &i);
printf("%d", i);
}
printf("\n");
}
```
```
Status Matching_Parentheses(void) {
SqStack S;
```

###### 写法 2 ：

```
InitStack(&S);
char ch, pop;
int flag = 1 ;
scanf(" %c", &ch);
```
```
while (flag && ch != '#') {
switch (ch) {
// 注意:不可以写成 case '(' || '[': 如果这样写 ||运算符只会返回 1
case '(':
Push(&S, ch);
break;
```
```
case '[':
Push(&S, ch);
break;
```
```
case ')':
// 若栈为空，则说明有多余的右括号，则匹配失败
if (!IsEmpty(&S) && GetTop(&S) == '(') {
Pop(&S, &pop);
} else {
flag = 0 ;
}
break;
```
```
case ']':
if (!IsEmpty(&S) && GetTop(&S) == '[') {
Pop(&S, &pop);
} else {
flag = 0 ;
}
break;
}
```
```
scanf(" %c", &ch);
}
```
```
if (flag && IsEmpty(&S))
return TRUE;
else
return FALSE;
}
```
```
bool Matching_Parenthese(void) {
SqStack S;
InitStack(&S);
char x;
char buffer[ 1024 ];
scanf("%s", &buffer);
char *ptr = buffer;
bool flag = true;
```
```
while (*ptr != '\0' && flag) {
if (*ptr == '(' || *ptr == '[') {
Push(&S, *(ptr++));
```

#### 10 以内的计算器

###### 写出一个只有加减乘除的计算器，要求每一步计算结果小于 10

###### 运算符顺序要求如下(#代表结束标志，且#运算级最小)

```
} else if (*ptr == ')') {
if (!IsEmpty(&S) && GetTop(&S) == '(') {
Pop(&S, &x);
ptr++;
} else
flag = false;
} else if (*ptr == ']') {
if (!IsEmpty(&S) && GetTop(&S) == '[') {
Pop(&S, &x);
ptr++;
} else
flag = false;
}
}
```
```
if (flag && IsEmpty(&S)) {
return true;
} else {
return false;
}
}
```
```
char Evaluate() {
SqStack opnd; //运算数栈
SqStack optr; //运算符栈
InitStack(&opnd);
InitStack(&optr);
Push(&optr, '#'); //先把#结束表示压入运算符栈
char ch, theta;
char a, b;
scanf(" %c", &ch);
```
```
while ('#' != ch || GetTop(&optr) != '#') {
//先判断是否为运算符
if (!IsOperator(ch)) {
Push(&opnd, ch);
scanf(" %c", &ch);
```

###### 测试代码:

```
} else {
//比较栈顶运算符和输入运算符比较
switch (Precede(GetTop(&optr), ch)) {
//输入运算符大于栈顶运算符，则入栈
case '<':
```
```
Push(&optr, ch);
//开始读取下一个运算符
scanf(" %c", &ch);
break;
//如果输入运算符小于栈顶运算符，弹出optr栈顶运算符，并弹出opnd的两个运算数，进行运算
case '>':
Pop(&optr, &theta);
Pop(&opnd, &a);
Pop(&opnd, &b);
//把运算结果入栈
Push(&opnd, operate(a, theta, b)); //
//注意此时并没有对输入运算符ch进行任何操作，所以不用往后读取字符，
//即不需要scanf("%c", &ch);
break;
//如果相等则说明括号匹配结束
case '=':
Pop(&optr, &theta);
scanf(" %c", &ch);
break;
}
}
}
//返回opnd栈顶，表达式的最终结果
return GetTop(&opnd);
}
```
```
#include "Stack.h"
#define OPERATORMAX 7
```
```
char operators[OPERATORMAX] = {'+', '-', '*', '/', '(', ')', '#'};
int LocateChar(char *array, char theta);
char operate(char a, char theta, char b);
char Precede(char theta1, char theta2);
char Evaluate(void);
int main(void) {
```
```
printf("%c ", Evaluate());
// printf("%c", Precede('(', '/'));
// printf("%c", operate('2', '*', '4'));
system("pause");
return 0 ;
}
```
```
char Precede(char theta1, char theta2) {
```
```
int index1 = LocateChar(operators, theta1);
int index2 = LocateChar(operators, theta2);
```

## 3. 字符串，数组，广义表

```
char precedences[OPERATORMAX][OPERATORMAX] = {
{'>', '>', '<', '<', '<', '>', '>'}, {'>', '>', '<', '<', '<', '>', '>'},
{'>', '>', '>', '>', '<', '>', '>'}, {'>', '>', '>', '>', '<', '>', '>'},
{'<', '<', '<', '<', '<', '=', 0 }, {'>', '>', '>', '>', 0 , '>', '>'},
{'<', '<', '<', '<', '<', 0 , '='}};
```
```
return precedences[index1][index2];
}
```
```
char operate(char a, char theta, char b) {
int val_a = atoi(&a);
int val_b = atoi(&b);
int result;
switch (theta) {
case '+':
result = val_a + val_b;
break;
case '-':
result = val_a - val_b;
break;
case '*':
result = val_a * val_b;
break;
case '/':
result = val_a / val_b;
break;
}
char val[ 24 ];
itoa(result, val, 10 );
return val[ 0 ];
}
```
```
int LocateChar(char *array, char theta) {
for (int i = 0 ; i < OPERATORMAX; i++) {
if (array[i] == theta)
return i;
}
return - 1 ;
}
```
```
bool IsOperator(char a) {
if (- 1 == LocateChar(operators, a)) {
return false;
} else
return true;
}
```

#### 字符串匹配

###### 字符串的存储结构可以分为两类：

###### 顺序存储结构：

###### 链式存储结构：

###### 本笔记只记录顺序存储结构的字符串

###### 输入字符串函数和初始化

###### BF算法(Brute Force)

```
typedef struct __SString {
char ch[MAXLEN + 1 ]; //为了代码理解方便，不使用数组 0 号位置
int length;
} SString;
```
```
#define CHUNKSIZE 80 //每一节点的最大长度
typedef struct __Chunk {
char ch[CHUNKSIZE + 1 ];
__Chunk *next;
} Chunk;
```
```
typedef struct __LString {
Chunk *head, *tail;
int curlen; //当前字符串长度
} LString;
#endif
```
```
int GetLength(SString *S) {
int cnt = 0 ;
int i = 1 ; //因为不使用 0 号位置，从 1 开始
```
```
while (S->ch[i] != '\0') {
i++;
cnt++;
}
```
```
return cnt;
}
```
```
void InputString(SString *S) {
scanf(" %s", &S->ch[ 1 ]);
S->length = GetLength(S);
}
```
```
int BF_Match(SString S, SString T, int position) {
int i = position;
int j = 1 ;
```

###### BF算法效率分析

###### 令主串长度为 子串长度为 ，若从主串的第个位置开始与模式串匹配成功

###### 则在前 趟匹配中字符总共比较了 次

###### 若第趟匹配成功，则比较次数为 ，总比较次数为

###### 即

###### 最坏情况

###### 假设从主串对的第个位置开始与模式串匹配成功，则在前 趟中总共比较了 次

###### 若第趟匹配成功，则第趟需要 次匹配，总比较次数为

###### KMP算法

###### 令字符串 ，和模式串

###### 匹配到 和 时失匹 则

###### 下标由来： 为失匹之前成功匹配的子串长度

###### 指向 中失配字符，则有

###### 下标由来：

###### 由 可知，

###### 由 可知，如果 和 失匹，无需从 开始和 比较，只需要把 滑动到 的位置比较即可

###### 令 表示在匹配中 失匹时，让 与 比较

###### 可得

###### ，因为当 失匹时字符串来到 位置空串，有 空串

###### 且

###### 需要从 开始重新比较

```
while (i <= S.length && j <= T.length) {
if (S.ch[i] == T.ch[j]) {
i++;
j++;
} else {
// i-j+1 是回溯到初始匹配位置
i = i - j + 1 + 1 ;
j = 1 ;
}
}
//如果匹配成功，那么此时i和j都会自增+1，此时j>T.length
if (j > T.length)
return i - T.length;
else
return 0 ;
}
```

###### 求next数组

###### 求 数组的过程实际上是 的过程，即如果存在，那么 必然存在

###### 也是模式串的字串匹配模式串的过程

###### 设 即有

###### 第一种情况

###### 此时则有

###### 那么则有

###### 第二种情况

###### 说明在 处失匹，则回溯到

###### 如果 如下图

###### 那么

###### 如果

###### 那么一直回溯 若出现 则同上，若未出现

###### 未优化前，求next数组

```
void GetNext(SString T, int *next) {
next[ 1 ] = 0 ;
int j = 0 ;
int i = 1 ;
```
```
while (i < T.length) {
if ( 0 == j || T.ch[i] == T.ch[j]) {
i++, j++;
next[i] = j;
} else {
j = next[j];
}
}
}
```

###### 考虑如下问题，如果回溯的 也等于 会出现什么问题

###### 会出现无意义比较，解决办法让 也进行回溯

###### 优化后

###### KMP算法

```
void GetNext(SString T, int *next) {
next[ 1 ] = 0 ;
int j = 0 ;
int i = 1 ;
//! 注意:while里面 不能写i<=T.length，因为如果这么写，那么i经过++后,i=T.length+1
//! 因为操作的内存是动态的，这样会导致内存泄漏
//! 所以必须是i<T.length，这样最后i才会指向T.length
while (i < T.length) {
if ( 0 == j || T.ch[i] == T.ch[j]) {
i++, j++;
//在未优化之前，如果ch[i]匹配失败，那么会回溯到ch[j]上
//如果ch[j] == ch[i]那么说明匹配仍然会失败，因为ch[i]匹配失败
if (T.ch[i] == T.ch[j]) {
//在i++,j++之后提前判断是否相等
next[i] = next[j];
} else {
next[i] = j;
}
} else {
j = next[j];
}
}
}
```
```
int KMP_Match(SString S, SString T, int position) {
int *next = (int *)malloc(sizeof(int) * (T.length + 1 ));
GetNext(T, next);
```
```
int i = position;
int j = 1 ;
```
```
while (i <= S.length && j <= T.length) {
if (j == 0 || S.ch[i] == T.ch[j]) {
i++, j++;
```

###### 测试代码

###### 字符串匹配玩具

###### 输入一个病毒序列长度为 ，从文件中读取病人样本，确认病人是否被感染

###### 注意 病毒序列是环状的

###### 比如病毒序列为 那么 都属于病毒

###### 思路 利用一个数组存储病毒序列，并把该序列扩大到 长度，依此比较

###### 实现代码

```
} else {
j = next[j];
}
}
free(next);
if (j > T.length)
return i - j;
else
return 0 ;
}
```
```
#include "SString.h"
```
```
int main(void) {
SString S, T;
InputString(&S);
InputString(&T);
int i = KMP_Match(S, T, 1 ); //把KMP改成BF就是BF算法
printf("%d", i);
```
```
system("pause");
return 0 ;
}
```
```
#include "SString.h"
#include <fstream>
#define FILENAME "Virus.txt"
//获取文件中样本个数
int File_GetNumber();
```
```
int main(void) {
//创建结构体Virus存储病毒信息
SString Virus;
//输入病毒序列
InputString(&Virus);
//获取文件中样本个数
int number = File_GetNumber();
// id用户标记文件中第几个样本
int id = 1 ;
//创建文件输入对象
std::ifstream ifs(FILENAME);
//判断文件是否打开成功
if (!ifs.is_open()) {
printf("Failed!\n");
```

exit( 0 );
}
//如果打开成功,扩大病毒序列，如 xyz 扩大称 xyzxyz
for (int i = Virus.length, j = 1 ; j <= Virus.length; j++) {
Virus.ch[i + j] = Virus.ch[j];
}
//因为病毒序列被扩大，所以要重新设置'\0'
Virus.ch[ 2 * Virus.length + 1 ] = '\0';

while (number--) {
//创建样本结构体
SString sample;
//设置检测是否被感染标记flag
int flag = false;
// ifs读文件，并输入到sample上面
ifs >> &sample.ch[ 1 ];
//初始化sample的长度
sample.length = GetLength(&sample);
//设置临时结构体temp，用于获取不同的病毒序列
SString temp;
temp.length = Virus.length;
//把不同的序列赋值给temp
for (int i = 0 ; i < Virus.length; i++) {
for (int j = 1 ; j <= Virus.length; j++) {
temp.ch[j] = Virus.ch[j + i];
}
//为temp设置结束标识符
temp.ch[Virus.length + 1 ] = '\0';
//此时已经获取了病毒序列储存在temp中，把病毒样本和病毒序列比对
flag = KMP_Match(sample, temp, 1 );
if (flag) { //如果flag!=0说明检测成功
printf("%d infected\n", id++);
break;
}
}
if ( 0 == flag)
printf("%d Not infected\n", id++);
}
system("pause");
return 0 ;
}

int File_GetNumber() {
std::ifstream ifs(FILENAME);
char buffer[ 1024 ];
int cnt = 0 ;
// ifs会一直读取字符输入到buff数组上，直到遇到空格等制表符停止
while (ifs >> buffer) {
cnt++;
}
return cnt;
}


### 数组

###### 声明格式 数据类型变量名称行数 列数

###### 如

###### 一个二维数组也可以被定义成一维数组

###### 例如:

###### 三维数组 每个元素都是二维数组，且二维数组中的每个元素又都是一维数组

###### 维数组 每个元素都是 维数组，且 维数组的每个元素都是 维数组

###### 维数组中的每个元素都是一维数组

###### 若有三维数组 各元素维

###### 则

###### 可以抽象成下图

###### 若有 维数组，各个维度的元素个数为

###### 则

### 广义表(Generalized List)

###### 广义表通常记作

###### 为表名通常用大写字母表示

###### 为长度

###### 为表的元素

```
typedef elemtype array2[m][n];
等价于
typedef elemtype array1[n];
typedef array1 array2[m];
```

###### 表头 若 非空 ，则第一元素 就是表头

###### 表尾 除表头之外的其他元素组成的表

###### 注意 表尾不是一个元素，而是一个子表

###### 例

###### 空表，

###### ， 和 都是 但并不是同一

###### 广义表的性质:

###### 广义表中的元素有相对次序 一个直接前驱和一个直接后继

###### 广义表的长度定义为最外层所包含的元素个数 广义表的深度定义为该广义表展开后所含括号的层数

###### 如 深度 ， 深度 ， 深度

###### 注意 原子的深度为 ，空表的深度为

###### 在广义表中可以为其他广义表共享，如上述广义表 就共享

###### 广义表可以是一个递归的表，如上述 广义表

###### 注意 递归表的长度是有限的，但是深度是

###### 广义表的基本运算

## 4. 树、二叉树、森林

### 定义

###### 树是 个节点的有限集合

###### 当 时为空树

###### 有且仅有一个称之为根的节点

###### 令一颗树为

###### 除根节点外，可分为 个互不相交的有限集 ，其中一个集合又是一棵树

###### 称其为 的子树

###### 如下图


### 树的基本术语

###### 节点的度

###### 节点拥有的子树个数成为节点的度

###### 如上图

###### 树的度

###### 树的度是树内各节点度的最大值

###### 上图的度为

###### 层次

###### 节点的层次从根开始定义，根为第一层，根的孩子为第二层

###### 树中任意节点的层次 它的双亲层次

###### 高度

###### 树中节点的最大层次成为树的高度

###### 如上图

###### 森林

###### 是 颗互不相交的树的集合

###### 对任意一棵树而言，其子树组成森林

### 二叉树的定义

###### 是 个节点组成的集合， 时为空树

###### 对于非空树

###### 有且仅有一个根节点

###### 除根结点外，有互不相交的 两棵子树可以为空树，分别称其为 的左右子树

### 二叉树的性质

###### 每个节点最多有两棵子树即

###### 子树有左右之分，不可颠倒

### 二叉树定理

###### 定理

###### 在二叉树的第层上，最多有 个节点


###### 定理

###### 深度为 的二叉树，最多有 个节点

###### 定理

###### 令一颗二叉树 有 个节点，其中 分别为 的节点个数

###### 即有

###### 可知 的根无双亲节点，而其他的节点都有双亲 令这些节点的个数为

###### 即

###### 由 可知

###### 所以

### 完全二叉树性质及定理

###### 定义

###### 深度为 的，由 个节点的二叉树

###### 当且仅当其每一个节点都与深度为 的满二叉树中编号从 到 的节点一一对应时

###### 称其为完全二叉树

###### 如下图

###### 特点

###### 对完全二叉树的任意节点

###### 若其右分支的子孙最大层次为 ，则其左分支的子孙最大层次为 或


###### 定理

###### 若一个完全二叉树有 个节点，深度为 ，则

###### 根据完全二叉树性质可知

###### 对其 化

###### 因为 所以

###### 定理

###### 一颗完全二叉树 ，有 个节点，若按照节点层次从左到右给其编号，则对于任意节点

###### 无双亲

###### 的双亲为

###### 则无左孩子

###### 为的左孩子

###### 则无右孩子

###### 则 为的右孩子

###### 如下图

### 链式二叉树

#### 存储结构

#### 遍历方式(递归)

```
typedef char BitreeElemType;
typedef struct __BiNode {
BitreeElemType data;
__BiNode *lchild, *rchild;
} BiNode, *BiTree;
```
```
void InOrder(BiTree T) {
if (!T)
return;
InOrder(T->lchild);
printf("%c ", T->data);
```

#### 遍历方式(非递归)

#### 先序遍历创建二叉树

```
InOrder(T->rchild);
}
```
```
void PreOrder(BiTree T) {
if (!T)
return;
printf("%c ", T->data);
PreOrder(T->lchild);
PreOrder(T->rchild);
}
```
```
void PostOrder(BiTree T) {
if (!T)
return;
PostOrder(T->lchild);
PostOrder(T->rchild);
printf("%c ", T->data);
}
```
```
void InOrder_unrec(BiTree T) {
SqStack S;
InitStack(&S);
BiTree p = T;
// BiTree pop = NULL;
while (p || !IsEmpty(&S)) {
if (p) {
//栈顶元素始终是p的parent节点
Push(&S, p);
p = p->lchild;
} else {
Pop(&S, &p); //把栈顶元素弹出给p，此时变成了原p的parent
//此时p的左孩子为空，根据in-oder规则，输出根节点p，然后再以相同的方式遍历他的右孩子
printf("%c", p->data);
p = p->rchild; //输出根节点后，遍历其右子树
}
}
}
```

#### 测试(创建，遍历)

###### 输入如下一棵树，按照中序遍历方式输出

#### 层次遍历算法

```
void Creat_BiTree_Pre(BiTree *T) {
//根据输出字符识别虚空节点，'#' 代表虚空节点
char e;
scanf(" %c", &e); //输入字符
if ('#' == e)
*T = NULL; //设置虚空节点
else {
*T = (BiTree)malloc(sizeof(BiNode));
(*T)->data = e;
Creat_BiTree_Pre(&(*T)->lchild);
Creat_BiTree_Pre(&(*T)->rchild);
}
}
```
```
#include "BinaryTree.h"
```
```
int main(void) {
BiTree T = NULL;
Creat_BiTree_Pre(&T);
InOrder_unrec(T); //非递归
// InOrder(T); 递归调用
system("pause");
return 0 ;
}
// 输入数据：CDNK##J##BZ###FL##M##
// 输出: KNJDZBCLFM
```
```
void LevelOrer(BiTree T) {
BiTree temp = NULL;
SqQueue Q;
```

#### 复制二叉树

#### 求深度和节点数

```
InitQueue(&Q);
if (T) // 先入队根
EntryQ(&Q, T);
while (!IsEmpty(&Q)) {
OutQ(&Q, &temp); // temp暂存弹出值
printf("%c", temp->data); //输出
if (temp->lchild) //在入队temp的左孩子和右孩子
EntryQ(&Q, temp->lchild);
if (temp->rchild)
EntryQ(&Q, temp->rchild);
}
}
```
```
/*
input: CDNK##J##BZ###FL##M##
------------------------------------------
output:CDFNBLMKJZ
*/
```
```
void Copy(BiTree *Tnew, const BiTree T) {
if (!T) {
*Tnew = NULL;
return;
} else {
*Tnew = (BiTree)malloc(sizeof(BiNode));
(*Tnew)->data = T->data;
Copy(&(*Tnew)->lchild, T->lchild);
Copy(&(*Tnew)->rchild, T->rchild);
}
}
```
```
int Depth(BiTree T) {
if (!T)
return 0 ;
else {
return Depth(T->lchild) > Depth(T->rchild)? Depth(T->lchild) + 1
: Depth(T->rchild) + 1 ;
}
}
```
```
int Nodes(BiTree T) {
if (!T)
return 0 ;
else
return 1 + Nodes(T->lchild) + Nodes(T->rchild);
}
```

#### 销毁二叉树(递归和非递归)

```
//递归的方式
void Destroy(BiTree *root) {
//销毁操作必须按照后续遍历的顺序
if (!(*root))
return;
else {
Destroy(&(*root)->lchild);
Destroy(&(*root)->rchild);
free(*root);
*root = NULL;
}
}
```
```
void Destroy_unrec(BiTree *root) {
//此算法的思路是:创建一个链栈，分别依次入栈
//<根节点>,<根节点的左孩子>,<左孩子的左孩子>,.....<最后一个左孩子>
//利用lchild充当链栈的next.
//当lchild发生变法时，树的结构必然发生变化，所以需要一个current指针来指向入栈节点
//当所有根节点左子树的所有左孩子入栈完毕，使current指向栈顶top
//判断栈顶节点是否有右孩子，如果有则current指向它的右孩子，并把current入栈
//如果没有右孩子，则出栈，并释放栈顶
//重复此步骤
BiTree top = NULL; //初始化一个链栈
BiTree temp; //暂存current
BiTree current = (*root)->lchild; //因为要把root入栈，current指向root的左孩子
(*root)->lchild = top; //因为lchild充当链栈的next，所以lchild指向top
top = *root; //此时root变成栈顶
```
```
while (top) {
while (current) { //如果current不为空，则入栈
temp = current; //暂存current
current = current->lchild;
temp->lchild = top; //入栈
top = temp;
}
//此时已经把root的左孩子，左孩子的左孩子.....入栈，栈顶为树的最左路径的最后一个节点
current = top; // current 和 top 指向同一个节点
if (current->rchild) { //如果栈顶有右孩子
temp = current;
// current指向它的右孩子，然后再次循环上面的步骤
current = current->rchild;
//因为栈顶的右孩子地址已经被current保存，所以可以把该指针指向NULL
temp->rchild = NULL;
} else { // 如果栈顶元素没有左孩子
//此时top和current指向同一节点
top = top->lchild;
free(current);
current = NULL;
//回到上面的循环时，因为current为空，所以不会有元素入栈，并且current会指向栈顶
```

#### 头文件

### 线索二叉树 Threaded Binary Tree(了解即可)

###### 问题，如何寻找特点遍历顺序中二叉树节点的前驱和后继

###### 办法

###### 通过遍历，浪费时间

###### 给结构体内增加前驱和后继指针，增加存储负担

###### 利用二叉链表中的空指针域

###### 定理

###### 如果一个二叉树有 个节点，那么空指针域为 个

###### 总指针域为 个，除去根节点，一个有 个节点，即需要 个指针域

```
}
}
*root = NULL; //销毁完毕，把root指向空
}
```
```
#include "Queue.h"
#include "Stack.h"
#include "define.h"
```
```
#ifndef __BINARYTREE_H
#define __BINARYTREE_H
```
```
typedef char BitreeElemType;
typedef struct __BiNode {
BitreeElemType data;
__BiNode *lchild, *rchild;
} BiNode, *BiTree;
```
```
void Creat_BiTree_Pre(BiTree *T);
void InOrder(BiTree T);
void InOrder_unrec(BiTree T);
void PreOrder(BiTree T);
void PostOrder(BiTree T);
void LevelOrer(BiTree T);
void Copy(BiTree *Tnew, const BiTree T);
int Depth(BiTree T);
int Nodes(BiTree T);
void Destroy_unrec(BiTree *root);
void Destroy(BiTree *root);
#endif
```

###### 线索二叉树的定义

###### 如果某个节点的左孩子为空，那么利用左孩子指针域，把它指向它的前驱

###### 如果右孩子为空，则指向它后继

###### 这种改变指向的指针称为线索

#### 数据类型定义

###### 左孩子为空

###### 左孩子指向前驱

###### 右孩子为空

###### 右孩子指向前驱

###### 如果按照遍历的顺序，那么序列中第一个元素必然没有前驱

###### 把该节点的左孩子指向一个头指针

###### 该头指针的左孩子指向根节点，右孩子指向序列最后一个节点

###### 一个中序遍历为 的线索二叉树

###### 如下图

### 树和森林

#### 树的存储结构

###### 1. 双亲表示法

```
typedef struct BiThrNode {
int data;
int ltag, rtag; //为了区分左右孩子指向为空还是前驱或后继，新增ltag,rtag
BiThrNode * lchidl, *rchild;
} *BiThrTree;
```

###### 2. 孩子链表

```
struct PTNode {
DataType data;
int parent; //存放parent在数组中的位置
};
```
```
struct PTree {
PTNode[MAXSIZE];
int root; //根节点位置
int n; //当前节点个数
};
```
```
//孩子节点结构
struct CTNode {
int chlid;
CTNode *next;
};
```
```
//双亲结点结构
struct CTBox {
DataType data;
int parent; //可有可无，看具体需求
CTNode * child;
};
```
```
//整体树结构
struct CTree {
CTBox[MAXSIZE];
int root;
int n;
};
```

###### 3. 孩子兄弟表示法(树转化二叉树的基础)

#### 树与二叉树之间相互转换

###### 树转二叉树

###### 在兄弟之间连线

###### 对于任意一个节点 ，除了其左孩子外，去除掉所有孩子与其的关系

###### 以根节点的左孩子为中心，顺时针旋转 ，再与根节点相连

```
//节点的child指针域指向它的第一个孩子，sibling指向第一个兄弟
struct CSNode {
DataType data;
CSNode * child, *sibling;
};
```

###### 二叉树转树

###### 若 节点是双亲节点的左孩子，则将 的右孩子，右孩子的右孩子 连接到 的双亲结点上

###### 抹掉所有双亲结点和右孩子之间关系

###### 整理成树状

#### 森林与二叉树之间的转化

###### 森林转二叉树

###### 将森林中的各棵树转化为二叉树

###### 链接这些二叉树的根节点

###### 第一棵树的根为二叉树的根，进行调整


###### 二叉树转森林

###### 若是二叉树的根，则取消所有 的右孩子，右孩子的右孩子 之间的关系

###### 此时有 颗孤立的二叉树，把这些二叉树转成树

#### 树和森林的遍历

###### 树的遍历

###### 先根遍历 若树不为空，则先访问根节点，然后再依次先根遍历遍历各个子树

###### 后根遍历 若树不为空，先依次后根遍历各个子树，再访问根节点

###### 层次遍历 自上到下，从左到右

###### s

###### 先根遍历为

###### 后根遍历

###### 森林的遍历

###### 假设有森林 ，有 棵互不相交的树

###### 将森林看成三部分

###### 森林中第一棵树的根节点

###### 森林中第一棵树的所有子树

###### 森林中 到 颗树

###### 先序遍历

###### 访问 的根节点

###### 先序遍历 的所有子树

###### 先序遍历 到

###### 即从左到右依次对 进行先根遍历


###### 中序遍历

###### 中序遍历 的所有子树

###### 访问 的根节点

###### 中序遍历 到

###### 即从左到右依次对 进行后根遍历

###### 对上图进行先序遍历和中序遍历

###### 先序

###### 中序

### 哈夫曼树

#### 术语

###### 路径

###### 从树中一个节点到另一个节点之间的分支，组成两个节点间的路径

###### 节点的路径长度

###### 两节点间路径上的分支数

###### 树的路径长度

###### 从树根到每一个节点的路径长度之和，记作

###### 节点数目相同的二叉树中，完全二叉树是路径长度最短的二叉树

###### 权

###### 将树中节点赋给一个含有某种意义的值，这个值叫

###### 结点的带权路径长度

###### 从根节点到该节点之间的路径长度与该节点的乘积，即

###### 树的带权路径长度

###### 树中所有叶子节点的带权路径长度之和

###### 如下图


#### 最优二叉树

###### 哈夫曼树，又称最优二叉树，即带权路径 最短的树

###### 注意

###### 是 相同的树比较之下

###### 完全二叉树包括满二叉树不一定是哈夫曼树

###### 哈夫曼树中权值越大的叶子节点离根节点越近

###### 具有相同带权路径的哈夫曼树，节点位置不唯一

#### 构造哈夫曼树

#### step和定理

###### 根据 个给定的权值 构成 个只有根节点的森林 森林里全是根

###### 在 中选取两个权值最小的树 ，构造一颗新的二叉树

###### 在 中删除 ，把 加入 中

###### 重复如上步骤，直到 中只有一颗树

###### 定理

###### 包含 个节点的树，需要经过 次合并才能形成哈夫曼树

###### 定理

###### 把一颗含有 个节点的树，转化成哈夫曼树，那么这个哈夫曼树一共有 个

###### 定理

#### 代码实现

###### 数据类型定义

```
typedef struct __HTNode {
int weight;
int parent, lchild, rchild;
} HTNode, *HTree;
```

前置函数，选取两个最小值

Creat_Huffman

```
void Select_Min(const HTree T, int length, int *e1, int *e2) {
int min1, min2;
min1 = min2 = INT_MAX;
int pos1, pos2;
pos1 = pos2 = 0 ;
```
```
for (int i = 1 ; i < length + 1 ; ++i) {
if (T[i].parent == 0 ) { //! parent==0 说明在森林中
if (T[i].weight < min1) {
min2 = min1;
pos2 = pos1;
min1 = T[i].weight;
pos1 = i;
} else if (T[i].weight < min2) {
min2 = T[i].weight;
pos2 = i;
}
}
}
```
```
*e1 = pos1;
*e2 = pos2;
}
```
```
void Creat_Huffman(HTree *T, int n) {
if (n <= 1 )
return;
int m = 2 * n - 1 ; //定理 2
```
```
*T = (HTree)malloc(sizeof(HTNode) * (m + 1 )); // 0号位置不存元素
```
```
for (int i = 1 ; i < m + 1 ; ++i) { //进行初始化
(*T)[i].lchild = (*T)[i].rchild = 0 ;
(*T)[i].parent = 0 ;
}
```
```
for (int i = 1 ; i < n + 1 ; ++i) { //赋值weight
scanf(" %d", &(*T)[i].weight);
}
//-------------------初始化完毕，开始构造--------------------------
int min1, min2; //表示第一小和第二小的位置
for (int i = n + 1 ; i < m + 1 ; ++i) { // n+1号位置为新构造的节点下标
Select_Min(*T, i - 1 , &min1, &min2); //! 核心语句 动态的选择大小
```
```
(*T)[min1].parent = (*T)[min2].parent = i; //合并
(*T)[i].lchild = min1; //新节点的左右孩子
(*T)[i].rchild = min2;
(*T)[i].weight = (*T)[min1].weight + (*T)[min2].weight; //赋值权值
}
}
```

###### 测试代码

### 哈夫曼编码

###### 讨论的背景

###### 在远程通信中传递字符串时，需要转换成二进制的字符串

###### 即，让待传递字符串中出现次数多的字符采用尽可能短的编码

###### 这样的话二进制字符串的编码就会缩短

###### 但，由于二进制只有 和 ，所以有可能二进制代码转成字符时，出现二义性

###### 所以要设计长度不等的编码，则必须使任一字符的编码都不是另一个字符编码的前缀

###### 如上形式的编码称为 前缀码

###### 哈夫曼编码

```
#include "HuffmanTree.h"
#define NODES 8
int main(void) {
HTree T = NULL;
Creat_Huffman(&T, NODES);
```
```
for (int i = 1 ; i < 2 * NODES; ++i) {
printf("weight = %d\tparent = %d\tlchild = %d\trchild = %d\n", T[i].weight,
T[i].parent, T[i].lchild, T[i].rchild);
}
```
```
system("pause");
return 0 ;
}
//
/*
input: 7 19 2 6 32 3 21 10
------------------------------------------
output:
weight = 7 parent = 11 lchild = 0 rchild = 0
weight = 19 parent = 13 lchild = 0 rchild = 0
weight = 2 parent = 9 lchild = 0 rchild = 0
weight = 6 parent = 10 lchild = 0 rchild = 0
weight = 32 parent = 14 lchild = 0 rchild = 0
weight = 3 parent = 9 lchild = 0 rchild = 0
weight = 21 parent = 13 lchild = 0 rchild = 0
weight = 10 parent = 11 lchild = 0 rchild = 0
weight = 5 parent = 10 lchild = 3 rchild = 6
weight = 11 parent = 12 lchild = 9 rchild = 4
weight = 17 parent = 12 lchild = 1 rchild = 8
weight = 28 parent = 14 lchild = 10 rchild = 11
weight = 40 parent = 15 lchild = 2 rchild = 7
weight = 60 parent = 15 lchild = 12 rchild = 5
weight = 100 parent = 0 lchild = 13 rchild = 14
*/
```

###### 哈夫曼编码是总长最短的前缀码

###### 统计字符集中每个字符在电文中出现的平均概率概率越大，编码要求最短

###### 利用哈夫曼树的特点 权值越大的叶子离根越近 将每个字符的概率值最为权值，构造哈夫曼树

###### 在哈夫曼树的每个分支上标 和 ，左分支为 ，右分支为

###### 为什么哈夫曼编码是最短的前缀码？

###### 根据哈夫曼树的特性，原树中的 个节点，在哈夫曼树中变成了叶子

###### 叶子节点不会是另一个叶子的双亲或是祖先，所以是前缀码

###### 哈夫曼树的性质

###### 性质 哈夫曼编码是前缀码

###### 性质 哈夫曼编码是最优前缀码

#### 代码实现

###### 测试代码

###### 构建如下哈夫曼编码

```
HuffmanCode Creat_HuffmanCode(const HTree HT, int n) {
// HC和哈夫曼树一样，不使用 0 号下标
HuffmanCode HC = (char **)malloc(sizeof(char *) * (n + 1 ));
char *temp_string = (char *)malloc(sizeof(char) * n); //此数组使用 0 号下标
temp_string[n - 1 ] = '\0'; //因为存放字符串所以最后一个位置 '\0'
```
```
for (int i = 1 ; i < n + 1 ; ++i) {
int parent = HT[i].parent; //需要向上回溯
int current = i; //回溯中当前节点
int start = n - 1 ; //数组中最后一个位置，即'\0'
while (parent) {
```
```
if (current == HT[parent].lchild) //如果是左孩子，那么为'0'
temp_string[--start] = '0';
else
temp_string[--start] = '1'; //右孩子为 '1'
```
```
current = parent;
parent = HT[parent].parent;
}
//计算长度:因为strat表示字符串的起始下标，n-1表示末尾结束符'\0',所以 length
//= n-1-start+1=n-start;
HC[i] = (char *)malloc(sizeof(char) * (n - start)); //根据长度分配空间
strcpy(HC[i], &temp_string[start]); //拷贝字符串
}
```
```
free(temp_string); //释放堆空间
return HC;
}
```
```
#include "HuffmanTree.h"
```

#define NODES 7
int main(void) {
HTree T = NULL;
Creat_Huffman(&T, NODES);

HuffmanCode HC = Creat_HuffmanCode(T, NODES);
int a = 65 ; // ASCII 65 是'A'
for (int i = 1 ; i < NODES + 1 ; ++i) {
printf("%c=%s\n", a, HC[i]);
++a;
}

system("pause");
return 0 ;
}
//
/*
input: 40 30 15 5 4 3 3
------------------------------------------
output:
A=0
B=10
C=110
D=11111
E=11110
F=11100
G=11101
*/


#### 整体头文件

## 5. 图(Graph)

### 图的定义和术语

###### 图

###### 顶点的有限非空集合

###### 边的有限集合

###### 图分为有向图 和无向图

###### 如下图

#### 完全图

###### 完全图

###### 任意两个点都有一条边相连

###### 若有 个顶点的无向完全图，则

###### 若有 个顶点的有向完全图，则

```
#include "define.h"
#include "string.h"
#ifndef __HUFFMANTREE_H
#define __HUFFMANTREE_H
```
```
typedef struct __HTNode {
int weight;
int parent, lchild, rchild;
} HTNode, *HTree;
typedef char **HuffmanCode;
```
```
void Select_Min(const HTree T, int length, int *e1, int *e2);
void Creat_Huffman(HTree *T, int n);
```
```
HuffmanCode Creat_HuffmanCode(const HTree HT, int n);
#endif
```

#### 稀疏图(Sparse Graph)和稠密图(Dense Gaph)

###### 稠密图

###### 稠密图 有较多边的图

#### 顶点的度(degree)

###### 与该顶点相关联的边的数量

###### 中，顶点的度

###### 问题 当 中，仅有一个顶点的 为 ，其余顶点的 ，此时图为什么形状

###### 答 树，有向树

#### 路径(path)

###### 路径 接续的边构成的顶点序列

###### 路径长度 路径上边的数量或权值之和

###### 回路 第一个顶点和最后一个顶点相同的路径

###### 路径 路径上的顶点均不相同

###### 回路 除路径起点和终点可以相同外，其余顶点均不相同的路径

#### 连通图(Connected Graph)

###### 若连通图

###### 在无向图 中

###### 若对任何两个顶点 ，都存在 路径，则 是连通图

###### 弱连通图

###### 若把有向图 中所有的边替换成无向边，此时得到的图为 的基图

###### 若它的基图为连通图，则 为若连通

###### 强连通

###### 任取有向图 中两个顶点 ，若 和 中间存在路径，则 为强连通

#### 连通子图和连通分量(Connected Component)

###### 无向图 的极大连通子图称为 的连通分量

###### 极大连通子图 若无向图 的子图 为连通图

###### 任取 即

###### 若把 加入到 中，如果 不再连通，则称 为 的极大连通子图

###### 如下图


###### 强连通分量

###### 有向图 的极大强连通子图称为 的连通分量

###### 若有向图 的子图 为连通图

###### 任取 即

###### 若把 加入到 中，如果 不再连通，则称 为 的极大强连通子图

#### 极小连通子图和生成树(Spanning Tree)

###### 若子图 是 的连通子图，在改子图中删除任意一条边， 不再连通，则称 是 的极小连通子图

###### 注意 极小连通子图中不存在 ，极大连通子图可以存在

###### 生成树

###### 若无向图 ， 中所有的点构成的极小连通子图就是 的生成树

### 图的存储结构

#### 邻接矩阵(Adjacency Matrix)

###### 若有图 ，有 个顶点，则对应 矩阵

###### 注意 无向图的邻接矩阵为对称矩阵，而有向图的邻接矩阵未必

###### 无向图


###### 的邻接矩阵为

###### 行中 的个数

###### 有向图

###### 第列 的个数

###### 第行 的个数

###### 带权图(网) weighted Graph

###### 若有带权图 ，有 个顶点，则对应 矩阵

###### 代码实现

###### 数据类型定义

###### 无向无权图

```
#define MAXWEIGHT 99999 //最大权值
#define MAXVERTEX 20 //最大定点数
typedef char VetexType; //顶点用字符表示
typedef int MatrixType; //矩阵类型
```
```
typedef struct __AMGraph {
char vertex[MAXVERTEX];
MatrixType edge[MAXVERTEX][MAXVERTEX];
int vertices, edges;
} AMGraph;
```
```
void Creat_unAMGraph_unweightd(AMGraph *G) {
//初始化点和边个数
printf("Please input the number of vertices:");
scanf(" %d", &G->vertices);
printf("Please input the number of edges:");
scanf(" %d", &G->edges);
//输入各个顶点的名字
```

###### 测试代码

```
printf("Please input the name of vertices(just like A B C):");
for (int i = 0 ; i < G->vertices; ++i) {
scanf(" %c", &G->vertex[i]);
}
//把矩阵初始化
for (int i = 0 ; i < G->vertices; ++i)
for (int j = 0 ; j < G->vertices; ++j)
G->edge[i][j] = 0 ;
```
```
char v1, v2; //一条边的顶点
int index_v1, index_v2; //边的顶点的下标
for (int i = 0 ; i < G->edges; ++i) {
printf("(for %d)Please input the edge(just like A B):", i + 1 );
scanf(" %c %c", &v1, &v2);
index_v1 = Locate_vertex(G, v1);
index_v2 = Locate_vertex(G, v2);
```
```
G->edge[index_v1][index_v2] = 1 ;
G->edge[index_v2][index_v1] = 1 ;
}
}
```
```
#include "Graph.h"
```
```
int main(void) {
AMGraph G;
Creat_unAMGraph_unweightd(&G);
print_Matrix(&G);
```
```
system("pause");
return 0 ;
}
//
/*
5 6
A B C D E
A B
A D
B C
D C
C E
B E
----------------------
0 1 0 1 0
1 0 1 0 1
0 1 0 1 1
1 0 1 0 0
0 1 1 0 0
*/
```

###### 无向带权图

###### 有向带权图

```
void Creat_unAMGraph_weightd(AMGraph *G) {
//初始化点和边个数
printf("Please input the number of vertices:");
scanf(" %d", &G->vertices);
printf("Please input the number of edges:");
scanf(" %d", &G->edges);
//输入各个顶点的名字
printf("Please input the name of vertices(just like A B C):");
for (int i = 0 ; i < G->vertices; ++i) {
scanf(" %c", &G->vertex[i]);
}
//把矩阵初始化
for (int i = 0 ; i < G->vertices; ++i)
for (int j = 0 ; j < G->vertices; ++j)
G->edge[i][j] = MAXWEIGHT;
```
```
char v1, v2; //一条边的顶点
int index_v1, index_v2; //边的顶点的下标
int weight;
for (int i = 0 ; i < G->edges; ++i) {
printf("(for %d)Please input the edge(just like A B):", i + 1 );
scanf(" %c %c %d", &v1, &v2, &weight); //相比无向无权图只多了一个weight
index_v1 = Locate_vertex(G, v1);
index_v2 = Locate_vertex(G, v2);
```
```
G->edge[index_v1][index_v2] = weight;
G->edge[index_v2][index_v1] = weight;
}
}
```
```
void Creat_AMGraph_weightd(AMGraph *G) {
//初始化点和边个数
printf("Please input the number of vertices:");
scanf(" %d", &G->vertices);
printf("Please input the number of edges:");
scanf(" %d", &G->edges);
//输入各个顶点的名字
printf("Please input the name of vertices(just like A B C):");
for (int i = 0 ; i < G->vertices; ++i) {
scanf(" %c", &G->vertex[i]);
}
//把矩阵初始化
for (int i = 0 ; i < G->vertices; ++i)
for (int j = 0 ; j < G->vertices; ++j)
G->edge[i][j] = MAXWEIGHT;
```
```
char v1, v2; //一条边的顶点
int index_v1, index_v2; //边的顶点的下标
int weight;
for (int i = 0 ; i < G->edges; ++i) {
```

###### 有向无权图

#### 邻接表(Adjacency List)

###### 数据类型定义

```
printf("(for %d)Please input the edge(just like A B):", i + 1 );
scanf(" %c %c %d", &v1, &v2, &weight);
index_v1 = Locate_vertex(G, v1);
index_v2 = Locate_vertex(G, v2);
```
```
G->edge[index_v1][index_v2] = weight;
}
}
```
```
void Creat_AMGraph_unweightd(AMGraph *G) {
//初始化点和边个数
printf("Please input the number of vertices:");
scanf(" %d", &G->vertices);
printf("Please input the number of edges:");
scanf(" %d", &G->edges);
//输入各个顶点的名字
printf("Please input the name of vertices(just like A B C):");
for (int i = 0 ; i < G->vertices; ++i) {
scanf(" %c", &G->vertex[i]);
}
//把矩阵初始化
for (int i = 0 ; i < G->vertices; ++i)
for (int j = 0 ; j < G->vertices; ++j)
G->edge[i][j] = 0 ;
```
```
char v1, v2; //一条边的顶点
int index_v1, index_v2; //边的顶点的下标
int weight;
for (int i = 0 ; i < G->edges; ++i) {
printf("(for %d)Please input the edge(just like A B):", i + 1 );
scanf(" %c %c %d", &v1, &v2, &weight);
index_v1 = Locate_vertex(G, v1);
index_v2 = Locate_vertex(G, v2);
```
```
G->edge[index_v1][index_v2] = 1 ; //有向图不是对称矩阵
}
}
```

###### 代码实现

###### 无向无权图

###### 无向有权，有向无权，有向有权图的创建方法和此方法类似，只需改动weight,和新建节点个数即可

```
typedef struct __EdgeNode {
int adjvertex;
__EdgeNode *next;
int weight;
} EdgeNode;
```
```
typedef struct __ALGNode {
VertexType name;
EdgeNode *first;
} ALGNode;
```
```
typedef struct __ALGraph {
ALGNode vertex[MAXVERTEX];
int edges, vertices;
} ALGraph;
//如下图
```
```
void Creat_unALGraph_unweighted(ALGraph *G) {
//初始化点和边个数
printf("Please input the number of vertices:");
scanf(" %d", &G->vertices);
printf("Please input the number of edges:");
scanf(" %d", &G->edges);
//输入各个顶点的名字
printf("Please input the name of vertices(just like A B C):");
for (int i = 0 ; i < G->vertices; ++i) {
scanf(" %c", &G->vertex[i].name);
G->vertex[i].first = NULL;
}
```
```
char v1, v2; //一条边的顶点
int index_v1, index_v2; //边的顶点的下标
```
```
for (int i = 0 ; i < G->edges; ++i) {
printf("(for %d)Please input the edge(just like A B):", i + 1 );
scanf(" %c %c", &v1, &v2);
index_v1 = Locate_vertex(G, v1);
index_v2 = Locate_vertex(G, v2);
```

###### 测试代码

#### 邻接表和邻接矩阵的比较

###### 邻接矩阵

###### 优点

###### 便于判断顶点间是否有边

###### 便于计算各个顶点的度

```
//创造新节点 1
EdgeNode *pnew1 = (EdgeNode *)malloc(sizeof(EdgeNode));
pnew1->adjvertex = index_v2;
//头插法
pnew1->next = G->vertex[index_v1].first;
G->vertex[index_v1].first = pnew1;
//创造新节点 2
EdgeNode *pnew2 = (EdgeNode *)malloc(sizeof(EdgeNode));
pnew2->adjvertex = index_v1;
//头插法
pnew2->next = G->vertex[index_v2].first;
G->vertex[index_v2].first = pnew2;
}
}
```
```
#include "ALGraph.h"
```
```
int main(void) {
ALGraph G;
Creat_unALGraph_unweighted(&G);
print_ALG_unweighted(&G);
```
```
system("pause");
return 0 ;
}
//
/*
5 6
A B C D E
A B
A D
B C
D C
C E
B E
----------------------
A:A--D A--B
B:B--E B--C B--A
C:C--E C--D C--B
D:D--C D--A
E:E--B E--C
*/
```

###### 缺点

###### 不便于插入和删除顶点

###### 不便于统计边数，需要扫描矩阵才能计算.

###### 空间复杂度较高，但如果 较大时，可以采用上三角或下三角矩阵(因为矩阵是对称的)

###### 邻接表

###### 优点

###### 便于增加和删除顶点

###### 便于统计边的数量，按顶点顺序扫描所有边即可。

###### 空间效率高，无向图 ，有向图

###### 缺点

###### 不便于判断两顶点间是否有边(相对于矩阵的随机取值而言)

###### 不便于计算各个顶点的度。

###### 对于无向图， 第个表的节点个数

###### 对无向图

###### )

##### ，入度为第个表的节点个数，但是出度却要历遍所有的表

#### 十字链表

###### 十字链表可以解决用邻接链表储存的有向图求顶点degree的问题

###### 根据上图可知，一条边即是一个顶点的入度，也是另外一个顶点的出度

###### 设是 的一条边

###### 当建立边节点 时，使 的 域指向，使 的 指向

###### 当 再次有出度边 时，使 的 域指向 的 所指节点 指向

###### 当 再次有入度边 时，使 的 域指向 的 所指节点 指向

#### 邻接多重链表

###### 用于 解决 用 邻接表 存储的 无向图 每条边都要存储 两遍 的问题


###### 如上图

###### 记录该边是否被搜索过

###### 分别表示边 顶点的下标

###### 分别表示 的下条边节点， 的下条边节点

###### 令

###### 使 的 指向 的 域， 的 指向 的 域

###### 的 的下标， 的 的下标

###### 使 和 的 指向

###### 遍历

###### 令 的 为

###### 打印

### 图的遍历

###### 图中可能存在 ，且图的任何一点都有可能和其他顶点相连

###### 在访问完某个顶点之后，可能会沿着某些边又回到了曾经访问过的顶点

###### 解决思路

###### 设置辅助数组 ，用来标记顶点是否被访问过

###### 顶点未被访问过

###### 顶点被访问过


#### 深度优先 (Depth First Search)

###### 算法描述

###### 先访问 ，再访问 的邻接点

###### 再访问 的邻接点

###### 开始出栈，控制节点再次来到

###### 因为 已经被访问过，所以开始访问

###### 全部出栈完，控制再次回到

###### 出栈，结束

###### 代码实现下图

###### 注意上图中的当访问完 之后，并不是直接回到

###### 而是退回到 ，需要依次出栈

###### 遍历矩阵

```
void DFS_AM(AMGraph *G, int v, bool *visit) {
```
```
printf("%c ", G->vertex[v]); //先遍历顶点
visit[v] = true; //访问标记
```
```
for (int k = 0 ; k < G->vertices; ++k) {
if (G->edge[v][k] && !visit[k]) //如果v，k之间存在边，并且k顶点并未被访问过
DFS_AM(G, k, visit);
}
```

###### 测试代码

###### 遍历邻接表

###### 注意:使用邻接表时，遍历的顺序和邻接矩阵不一样，因为创建邻接表使用头插法(如果使用尾插法顺序

###### 则一样)

```
}
```
```
void DFS_AMGraph(AMGraph *G, VertexType v) { //封装函数
bool *visit = (bool *)malloc(sizeof(bool) * G->vertices); //为visit分配空间
memset(visit, false, sizeof(bool) * G->vertices); //初始化为false
```
```
int index = Locate_vertex(G, v); //找到下标
DFS_AM(G, index, visit); //以此下标为顶点出发，遍历
free(visit);
}
```
```
#include "AMGraph.h"
```
```
int main(void) {
AMGraph G;
Creat_unAMGraph_unweightd(&G);
DFS_AMGraph(&G, 'A');
```
```
system("pause");
return 0 ;
}
//
/*
8 9
A B C D E F G H
A B
A C
B D
D H
B E
E H
C F
C G
F G
----------------------
A B D H E C F G
*/
```
```
void DFS_AL(ALGraph *G, int v, bool *visit) {
printf("%c ", G->vertex[v].name);
visit[v] = true;
```
```
EdgeNode *p = G->vertex[v].first;
while (p) {
int adj = p->adjvertex;
if (!visit[adj]) // 只需判断visit数组，因为当p不为空时，adjvertex必然存在
```

###### 测试代码

#### 广度优先 (Breadth First Search)

###### 从图的 出发，首先访问 ，然后访问 的所有邻接点

###### 然后按照 的顺序，依次访问他们的邻接点

###### 实现遍历下图

```
DFS_AL(G, adj, visit);
```
```
p = p->next;
}
}
void DFS_ALGraph(ALGraph *G, VertexType v) { //封装代码
bool *visit = (bool *)malloc(sizeof(bool) * G->vertices);
memset(visit, false, sizeof(bool) * G->vertices);
```
```
int index = Locate_vertex(G, v);
DFS_AL(G, index, visit);
}
```
```
#include "ALGraph.h"
```
```
int main(void) {
ALGraph G;
Creat_unALGraph_unweighted(&G);
DFS_ALGraph(&G, 'A');
```
```
system("pause");
return 0 ;
}
//
/*
8 9
A B C D E F G H
A B
A C
B D
D H
B E
E H
C F
C G
F G
----------------------
A C G F B E H D
*/
```

###### 代码实现

###### 遍历矩阵

###### 测试代码

```
void BFS_AM(AMGraph *G, int v, bool *visit) {
SqQueue Q;
InitQueue(&Q);
EntryQ(&Q, v); //先让顶点入队
visit[v] = true; //入队时设置visit状态
int pop; //用于接收队列弹出数据
while (!IsEmpty(&Q)) {
OutQ(&Q, &pop);
printf("%c ", G->vertex[pop]); //出队时，打印
```
```
for (int k = 0 ; k < G->vertices; ++k) {
if (G->edge[pop][k] && !visit[k]) {
EntryQ(&Q, k);
visit[k] = true;
//! 设置visit状态，不可以放在printf后面，因为for循环可能造成重复入队
}
}
}
}
void BFS_AMGraph(AMGraph *G, VertexType v) {
bool *visit = (bool *)malloc(sizeof(bool) * G->vertices); //为visit分配空间
memset(visit, false, sizeof(bool) * G->vertices); //初始化为false
```
```
int index = Locate_vertex(G, v); //找到下标
BFS_AM(G, index, visit); //以此下标为顶点出发，遍历
free(visit);
}
```
```
#include "AMGraph.h"
```
```
int main(void) {
AMGraph G;
```

###### 遍历邻接表

###### 注意:使用邻接表时，遍历的顺序和邻接矩阵不一样，因为创建邻接表使用头插法(如果使用尾插法顺序

###### 则一样)

```
Creat_unAMGraph_unweightd(&G);
BFS_AMGraph(&G, 'A');
```
```
system("pause");
return 0 ;
}
//
/*
8 9
A B C D E F G H
A B
A C
B D
D H
B E
E H
C F
C G
F G
----------------------
A B C D E F G H
*/
```
```
void BFS_AL(ALGraph *G, int v, bool *visit) {
SqQueue Q;
InitQueue(&Q);
EdgeNode *p; //用于遍历邻接表
EntryQ(&Q, v); //入队顶点
visit[v] = true; //设置顶点visit数组状态
int pop; //用于接收队列弹出数据
while (!IsEmpty(&Q)) {
OutQ(&Q, &pop);
printf("%c ", G->vertex[pop].name); //出队后打印
p = G->vertex[pop].first; //利用p遍历
```
```
while (p) {
if (!visit[p->adjvertex]) { //判断p遍历中的邻接点是否被遍历过
EntryQ(&Q, p->adjvertex); //如果没有被遍历过，入队
visit[p->adjvertex] = true; //同时设置visit状态
}
p = p->next;
}
}
}
void BFS_ALGraph(ALGraph *G, VertexType v) {
bool *visit = (bool *)malloc(sizeof(bool) * G->vertices); //为visit分配空间
memset(visit, false, sizeof(bool) * G->vertices); //初始化为false
```
```
int index = Locate_vertex(G, v); //找到下标
```

###### 测试代码

#### 算法效率

###### 可知，邻接矩阵的时间效率为 邻接表的时间效率为

### 最小生成树 Spanning Tree

#### Prim 算法

```
BFS_AL(G, index, visit); //以此下标为顶点出发，遍历
free(visit);
}
```
```
#include "ALGraph.h"
```
```
int main(void) {
ALGraph G;
Creat_unALGraph_unweighted(&G);
BFS_ALGraph(&G, 'A');
```
```
system("pause");
return 0 ;
}
//
/*
8 9
A B C D E F G H
A B
A C
B D
D H
B E
E H
C F
C G
F G
----------------------
A C B G F E D H
*/
```

###### 令 为连通图带权，且

###### 设起点为 把 加入到 中

###### 选取 为最小

###### 输出 边

###### 把 加入 中

###### 选取 为最小

###### 输出 边

###### 直到存在 条边

###### 此时输出的边即为

###### 代码实现

###### 实现下图的Spanning Tree

###### 需要辅助集合U

###### 邻接矩阵

###### 前置算法

```
struct Uset {
int adjvertex; //下标为i的点的邻接点
int weight; //当前权值
};
```

###### 邻接表

```
int Min_Uset(Uset *U, int n) {
int min = INT_MAX;
int pos = 0 ;
```
```
for (int i = 0 ; i < n; ++i) {
if (U[i].weight != 0 && U[i].weight < min) {
//! 核心语句 U[i].weight != 0 说明不在U中，即V-U
min = U[i].weight;
pos = i;
}
}
return pos;
}
```
```
void MST_Prim(AMGraph *G, VertexType v) {
int u = Locate_vertex(G, v);
Uset *U = (Uset *)malloc(sizeof(Uset) * G->vertices);
//动态为U分配空间，大小为n(顶点个数)
for (int i = 0 ; i < G->vertices; ++i) {
//初始化U集合，因为先把顶点v放入U集合中，所以U[i].adjvertex为
//顶点v的下标，即u。如果i与点v存在边
U[i].adjvertex = u;
//如果i与点v存在边，赋值，如果不存在weight为 99999
U[i].weight = G->edge[u][i];
}
U[u].weight = 0 ; // weight = 0 说明此点已经加入U集合
```
```
for (int i = 1 ; i < G->vertices; ++i) { //选取n-1条边
int min = Min_Uset(U, G->vertices); //在V-U中选取权值最小的边
int u_0 = U[min].adjvertex; // u_0为最小边的邻接点
printf("%c->%c ", G->vertex[u_0], G->vertex[min]); //输出此两点
U[min].weight = 0 ; //把该边的顶点加入集合U
```
```
for (int j = 0 ; j < G->vertices; ++j) { //更新U集合
if (G->edge[min][j] < U[j].weight) {
//如果成立，使U的weight，和adjvertex和min相关
U[j].weight = G->edge[min][j];
U[j].adjvertex = min;
}
}
}
```
```
free(U);
}
```
```
void MST_Prime(ALGraph *G, VertexType v) {
int u = Locate_vertex(G, v);
Uset *U = (Uset *)malloc(sizeof(Uset) * G->vertices);
```

###### 测试代码

```
for (int i = 0 ; i < G->vertices; ++i) {
//邻接表的weight不会为最大值，所以初始化为最大值
U[i].weight = MAXWEIGHT;
U[i].adjvertex = u;
}
U[u].weight = 0 ; //加入U集合
EdgeNode *p = G->vertex[u].first;
while (p) {
//遍历点v的邻接表，把weight放入U中
U[p->adjvertex].weight = p->weight;
p = p->next;
}
```
```
for (int i = 1 ; i < G->vertices; ++i) {
// n-1个边
int min = Min_Uset(U, G->vertices); // 权值最小边
int u_0 = U[min].adjvertex;
printf("%c->%c ", G->vertex[u_0].name, G->vertex[min].name);
U[min].weight = 0 ; //加入集合U中
```
```
EdgeNode *p_min = G->vertex[min].first;
while (p_min) {
//因为邻接表的特性，无需要遍历所有顶点，只需遍历min的邻接表即可
if (p_min->weight < U[p_min->adjvertex].weight) {
U[p_min->adjvertex].adjvertex = min;
U[p_min->adjvertex].weight = p_min->weight;
}
p_min = p_min->next;
}
}
```
```
free(U);
}
```
```
#include "ALGraph.h"
```
```
int main(void) {
ALGraph G;
Creat_unALGraph_weighted(&G);
MST_Prime(&G, 'A');
```
```
system("pause");
return 0 ;
}
//
/*
6 10
A B C D E F
A B 6
A D 5
A C 1
B C 5
C D 5
B E 3
E C 6
```

#### Kruskal 算法

###### 定理

###### 若无向有权无环图 为 图的最大连通子图

###### ，作为连通依赖点，则 集合所有点必然存在一条通往 的路径

###### 单个顶点的连通依赖点为自身注意 表示为 不可以这么表示

###### 令 为连通依赖点，且 使 之间并不存在路径

###### 为连通图

###### 引理

###### 若 分别为 的最大连通子图

###### 若 ，则

###### 利用

###### 若 ，则说明 中所有的点都有一条通往 的路径

###### 为最大连通子图子图 同理

###### 算法

###### 若存在无向带权图 且 连通

###### 令集合

###### 对 进行排序，取 ，把 加入 中

###### 循环对 进行如下操作

###### 如果 的连通依赖点 的联通点

###### 则把 加入到

###### 直到遍历所有边

###### 集合中为 的

###### 代码实现

###### 数据类型定义

```
C F 4
D F 2
E F 6
----------------------
A->C C->F F->D C->B B->E
*/
```
```
struct Eset { //边集合
int start; //起点
int end; //终点
int weight;
};
```
```
void Sort_Eset(Eset *E, int length); //排序函数
```

###### 采用冒泡排序，可以灵活变换

###### 邻接矩阵

```
void Sort_Eset(Eset *E, int length) {
bool flag = true; //排序flag
for (int i = 0 ; i < length - 1 && flag; ++i) { //如果未发生交换则说明有序
flag = false; //第一次设置为false
for (int j = 0 ; j < length - 1 - i; ++j) {
if (E[j].weight > E[j + 1 ].weight) {
flag = true; //如果发生交换，为true
Eset temp = E[j];
E[j] = E[j + 1 ];
E[j + 1 ] = temp;
}
}
}
}
```
```
void InitEset(Eset *E, AMGraph *G) {
//遍历上三角矩阵
Eset *p = E;
for (int i = 0 ; i < G->vertices; ++i) // i为array
for (int k = i + 1 ; k < G->vertices; ++k) { // k为column
if (G->edge[i][k] < MAXWEIGHT) { //小于说明存在
(p)->start = i;
(p)->end = k;
(p)->weight = G->edge[i][k];
++p;
}
}
p = NULL;
}
```
```
void MST_Krusal(AMGraph *G) {
Eset *E = (Eset *)malloc(sizeof(Eset) * G->edges);
InitEset(E, G);
Sort_Eset(E, G->edges);
//此时E集合有序
//建立V集合存放连通依赖点
int V[G->vertices]; //例如V[i] = k;
//表示顶点i依赖于k点(即必有一条到k的路径)
for (int i = 0 ; i < G->vertices; ++i) //清掉所有边
V[i] = i; //现在V集合的连通分量就是自己，即所有顶点无邻接点
```
```
for (int j = 0 ; j < G->edges; ++j) {
int v_1 = E[j].start; // v_1和v_2分别为这个边的顶点
int v_2 = E[j].end;
```
```
int component_v_1 = V[v_1]; // v_1所属的连通分量
int component_v_2 = V[v_2]; // v_2所属的连通分量
if (component_v_1 != component_v_2) { //说明不会形成loop
```

###### 测试代码

###### 邻接表

```
printf("%c->%c ", G->vertex[v_1], G->vertex[v_2]);
//链接这两个顶点，并且输出
//因为链接了两个顶点，那么此时构成一条新的连通分量，所以要更新连通分量依赖点
for (int k = 0 ; k < G->vertices; ++k) {
if (V[k] == component_v_2) //如果k顶点依赖于v_2的连通分量
//那么在连接之后，所有的顶点都依赖于v_1的连通分量
V[k] = component_v_1;
}
}
}
```
```
free(E);
}
```
```
#include "AMGraph.h"
```
```
int main(void) {
AMGraph G;
Creat_unAMGraph_weightd(&G);
```
```
MST_Krusal(&G);
system("pause");
return 0 ;
}
```
```
//
/*
6 10
A B C D E F
A B 6
A D 5
A C 1
B C 5
C D 5
B E 3
E C 6
C F 4
D F 2
E F 6
----------------------
A->C D->F B->E C->F B->C
*/
```
```
void InitEset(Eset *E, ALGraph *G) {
//! 邻接表和邻接矩阵不一样，矩阵是连续的，而邻接表在存储上不是连续的
//! ALGraph需要为有向图
Eset *p_E = E;
```
```
for (int i = 0 ; i < G->vertices; ++i) {
EdgeNode *p = G->vertex[i].first;
```

###### 测试代码

```
while (p) {
p_E->start = i;
p_E->end = p->adjvertex;
p_E->weight = p->weight;
```
```
p = p->next;
```
```
++p_E;
}
}
p_E = NULL;
}
```
```
void MST_Krusal(ALGraph *G) {
Eset *E = (Eset *)malloc(sizeof(Eset) * G->edges);
InitEset(E, G);
Sort_Eset(E, G->edges);
```
```
for (int w = 0 ; w < G->edges; ++w) {
printf("(%d)start=%d, end=%d,weight=%d\n", w, E[w].start, E[w].end,
E[w].weight);
}
int V[G->vertices];
for (int i = 0 ; i < G->vertices; ++i)
V[i] = i;
```
```
for (int j = 0 ; j < G->edges; ++j) {
int v_1 = E[j].start;
int v_2 = E[j].end;
```
```
int component_v_1 = V[v_1];
int component_v_2 = V[v_2];
```
```
if (component_v_1 != component_v_2) {
printf("%c->%c ", G->vertex[v_1].name, G->vertex[v_2].name);
```
```
for (int k = 0 ; k < G->vertices; ++k) {
if (component_v_2 == V[k])
V[k] = component_v_1;
}
}
}
```
```
free(E);
}
```
```
#include "ALGraph.h"
```
```
int main(void) {
ALGraph G;
Creat_ALGraph_weighted(&G); //! 需要用有向图来表示无向图
```

### 最短路径

#### Dijkstra 算法

###### 若有无向带权网

###### 以 为顶点，求出所有 和 间的最路径

###### 令 为 到 间的路径长度，集合

###### 若 存在，则初始化 ，若不存在则

###### 遍历所有点之后，把 加入到 中

###### 把 加入到 中，若 为 的邻接点，且

###### 则

###### 重复上步骤，直到

###### 用代码实现此图

```
MST_Krusal(&G);
```
```
system("pause");
return 0 ;
}
//
/*
6 10
A B C D E F
A B 6
A D 5
A C 1
B C 5
C D 5
B E 3
E C 6
C F 4
D F 2
E F 6
----------------------
A->C D->F B->E C->F B->C
*/
```

###### 代码实现

###### 邻接矩阵

```
void ShortestPath(AMGraph *G, int v, int *path) {
//! 数组path[i]表示i的最短前驱
int D[G->vertices]; //集合D表示各个顶点到v的距离
bool S[G->vertices]; //集合S，如果i点在S中则为true
```
```
for (int i = 0 ; i < G->vertices; ++i) {
//初始化D,S,path
D[i] = G->edge[v][i]; //如果不存在边，则为MAXWEIGHT
S[i] = false; //初始化S为空集
```
```
if (D[i] < MAXWEIGHT) //说明边存在
path[i] = v; //设置前驱
else
path[i] = - 1 ; //如果不存在边，-1
}
```
```
S[v] = true;
D[v] = 0 ;
//初始化完成
```
```
for (int i = 1 ; i < G->vertices; ++i) {
int min_index;
int min = MAXWEIGHT;
for (int j = 0 ; j < G->vertices; ++j) {
//从D中选出路径最短点，且不在集合S中
if (!S[j] && D[j] < min) {
min_index = j;
min = D[j]; //求出D[j]最小的点
}
}
S[min_index] = true; //把该点加入到S中
```
```
for (int k = 0 ; k < G->vertices; ++k) {
if (!S[k] && (G->edge[min_index][k] + D[min_index] < D[k])) {
//遍历min_index的邻接点，进行判断
D[k] = G->edge[min_index][k] + D[min_index];
```

###### 测试代码

```
path[k] = min_index;
}
}
}
}
```
```
void ShortestPath_Dijkstra(AMGraph *G, VertexType v) {
//封装的函数，表示以v为起点，求出所有点与v的最短路径
int v_index = Locate_vertex(G, v);
int *path = (int *)malloc(sizeof(int) * G->vertices);
ShortestPath(G, v_index, path);
// for (int i = 0; i < G->vertices; ++i)
```
```
for (int i = 0 ; i < G->vertices; ++i) {
if (i != v_index) {
print_path(G, path, v_index, i);
printf("\n");
}
}
```
```
free(path);
}
```
```
void print_path(AMGraph *G, int *path, int start, int end) {
SqStack S;
InitStack(&S);
printf("%c->", G->vertex[start]);
Push(&S, end); //先入栈end
int flag = end; //用于判断是否输出"->""
end = path[end];
while (end != start) {
Push(&S, end);
end = path[end];
}
```
```
int head = start;
int pop;
while (!IsEmpty(&S)) {
```
```
Pop(&S, &pop);
printf("%c(%d)", G->vertex[pop], G->edge[head][pop]);
if (pop != flag)
printf("->");
head = pop;
}
}
```
```
#include "AMGraph.h"
```
```
int main(void) {
AMGraph G;
Creat_unAMGraph_weightd(&G);
ShortestPath_Dijkstra(&G, 'A');
```

#### Floyd算法

###### 本质上为暴力算法

###### 令矩阵 存储图 的权值，其中 有 个顶点

###### 表示到的 表示 到 的

###### 遍历矩阵所有元素，向 之间插入点 ，如果

###### 则

###### 遍历结束后，矩阵 记录 的最短路径

###### 代码实现

###### 邻接矩阵

```
system("pause");
return 0 ;
}
//
/*
7 11
A B C D E F G
A B 15
A C 9
A D 4
C F 12
F G 16
F D 6
D B 5
B G 8
B E 2
E G 3
D G 11
----------------------
A->D(4)->B(5)
A->C(9)
A->D(4)
A->D(4)->B(5)->E(2)
A->D(4)->F(6)
A->D(4)->B(5)->E(2)->G(3)
*/
```
```
int **Path_Matrix(AMGraph *G) {
// path[i][j]表示从i到j的路径上，j点的直接前驱
int n = G->vertices;
int **path = (int **)malloc(sizeof(int *) * n); //先分配一维指针数组
for (int i = 0 ; i < G->vertices; ++i) // path[i]分配空间;
path[i] = (int *)malloc(sizeof(int) * n);
//此时path为二维数组
```

int D[n][n];

for (int i = 0 ; i < n; ++i)
for (int j = 0 ; j < n; ++j) {
D[i][j] = G->edge[i][j]; // copy给D
if (D[i][j] < MAXWEIGHT) //点i,j如果为邻接点
path[i][j] = i; //此时的路径即为i，j之间的边，所以j的前驱为i
else
path[i][j] = - 1 ;
}

for (int k = 0 ; k < n; ++k) //尝试在两点之间加入点k
for (int i = 0 ; i < n; ++i)
for (int j = 0 ; j < n; ++j) {
if (D[i][k] + D[k][j] < D[i][j]) {
D[i][j] = D[i][k] + D[k][j];
path[i][j] = path[k][j]; //更新path，即j的前驱，向前递归
}
}

return path;
}

void ShortestPath_Floyd(AMGraph *G, VertexType v1, VertexType v2) {
int start = Locate_vertex(G, v1);
int end = Locate_vertex(G, v2);

int **path = Path_Matrix(G);

SqStack S;
InitStack(&S);
Push(&S, end); //先入栈末端点
int prior = path[start][end];

while (prior != start) {
//向前回溯，直到prior == start
Push(&S, prior);
prior = path[start][prior];
}

int head = start; // head用于向前追溯
int pop;
printf("%c->", G->vertex[start]);
while (!IsEmpty(&S)) {
Pop(&S, &pop);
printf("%c(%d)", G->vertex[pop], G->edge[head][pop]);
if (pop != end)
printf("->");
head = pop; //向前追溯
}

for (int i = 0 ; i < G->vertices; ++i)
//因为path本质上是一维指针数组，每个指针又指向一块空间，所以逐个释放
free(path[i]);
free(path); //还需要释放path


### 有向无环图(Directed Acycline Graph)

#### AOC和AOE

###### 网

###### 用一个有向图表示一个工程的各个子工程及其相互制约关系

###### 其中顶点表示活动，弧表示优先制约关系

###### 网

###### 弧表示活动，以顶点表示活动开始或结束事件

#### 拓扑排序

###### 在 网没有回路的前提下，将全部活动排列成一个线性序列

###### 网中边 存在，则在这个序列中一定排在的前面

###### 对 网进行如上排序，即为拓扑排序

###### 算法思路

###### 若 图中 ，则去除掉所有和 相关的边

###### 令 ，把 加入到 中

###### 更新所有 的

###### 直到

###### 此时 的序列则为拓扑序列

###### 代码实现

###### 实现下图

```
path = NULL;
}
```

###### 邻接表

###### 前置函数

```
void InDegree(ALGraph *G, int *a) {
//获取所有点的indegree
for (int i = 0 ; i < G->vertices; ++i) {
EdgeNode *p = G->vertex[i].first;
```
```
while (p) {
++a[p->adjvertex];
p = p->next;
}
}
}
```
```
int *Get_Topo(ALGraph *G) {
int *indegree = (int *)malloc(sizeof(int) * G->vertices);
memset(indegree, 0 , sizeof(int) * G->vertices); //主要要对堆数据初始化
int *topo = (int *)malloc(sizeof(int) * G->vertices);
memset(topo, 0 , sizeof(int) * G->vertices);
```
```
InDegree(G, indegree); //获取全部点的indegree
```
```
SqStack S;
InitStack(&S);
```
```
for (int i = 0 ; i < G->vertices; ++i)
if (!indegree[i]) //如果indegree==0 入栈
Push(&S, i);
```
```
int m = 0 ; //用于控制topo下标
int pop; //用于接收栈弹出值
while (!IsEmpty(&S)) {
Pop(&S, &pop); //弹出
topo[m++] = pop; //栈顶即为拓扑序列顶点
EdgeNode *p = G->vertex[pop].first;
```
```
while (p) {
//因为在逻辑上删除了pop点，所以更新它邻接点的indegree
--indegree[p->adjvertex];
```
```
if (!indegree[p->adjvertex]) //判断indegree==0
Push(&S, p->adjvertex);
```
```
p = p->next;
}
}
```
```
if (m < G->vertices) {
//如果m=G->vertices 说明G为AOV
//如果不说明有回路
free(indegree);
free(topo);
return NULL; //返回空
```

### 关键路径

###### 如上图 网，源点 表示事件整体的开始，汇点 表示事件整体结束

###### 其他的点则表示一个活动的结束，同时也表示另外一个活动的开始

###### 关 表示时间，而 表示活动， 表示活动所需要的时间

###### 令 表示 的最早开始时间，即 时间之前的活动必须完成， 才能开始

###### 即 为的直接前驱

###### 令 表示 的最迟开始时间 即 的后继点 需要为 留出时间 为 的直接前驱

###### 若已知 ，则

```
} else {
free(indegree);
return topo;
}
}
```
```
void TopoSort(ALGraph *G) {
int *topo = Get_Topo(G);
if (!topo) { //如果为NULL
printf("The Graph is not AVO!\n");
return;
}
```
```
for (int i = 0 ; i < G->vertices; ++i) {
printf("%c ", G->vertex[topo[i]].name);
}
```
```
free(topo); //注意释放堆区数据
topo = NULL;
}
```

###### 活动时间 表示边 的

###### 表示， 发生的最早时间，只有 发生了， 才能发生

###### 所以

###### 注意

###### ，即源点 的最早发生时间为

###### 即汇点 的发生最早时间 的最迟时间

###### 由此可知 从源点开始向前递归 从后向前递归

###### 表示 的最迟发生时间

###### 若 则说明活动 没有缓冲时间，为关键路径

###### 如果 这说明活动 有 时间可以调整

###### 代码实现

###### 实现下图

###### 邻接表

```
void CriticalPath(ALGraph *G) {
int *topo = Get_Topo(G);
if (!topo) {
printf("The Graph is not AVO");
return;
}
```
```
int n = G->vertices;
int ve[n], vl[n]; // ve表示i顶点的最早发生时间，vl表示i顶点的最晚发生时间
memset(ve, 0 , sizeof(int) * n); //初始化为 0
```
```
for (int i = 0 ; i < n; ++i) {
int k = topo[i]; //按照拓扑序列遍历各点的邻接点
```

### 图的头文件

#### define_Graph.h

```
EdgeNode *p = G->vertex[k].first;
while (p) {
if (ve[p->adjvertex] < ve[k] + p->weight) //求出最大值
ve[p->adjvertex] = ve[k] + p->weight;
p = p->next; //接着判断下一个邻接点
}
}
//把所有的顶点的最晚发生时间初始化为汇点的最晚发生时间
for (int i = 0 ; i < n; ++i)
vl[i] = ve[topo[n - 1 ]]; // topo[n-1]的ve是最大的，为下面求vl最小值做准备
//--------------------------------------------
for (int i = n - 1 ; i >= 0 ; --i) {
//从汇点从后向前遍历拓扑序列
int k = topo[i];
```
```
EdgeNode *p = G->vertex[k].first;
```
```
while (p) {
if (vl[k] > vl[p->adjvertex] - p->weight)
vl[k] = vl[p->adjvertex] - p->weight; //要vl的最小值
p = p->next;
}
}
//------------------------------------------
for (int i = 0 ; i < n; ++i) {
```
```
EdgeNode *p = G->vertex[i].first;
while (p) {
int j = p->adjvertex;
int e = ve[i]; // 活动的最发生时间 = 该边的前驱节点i的最早发生时间
//活动的最晚发生时间=该边前驱节点的最晚发生时间-该边的weight
int l = vl[j] - p->weight;
```
```
if (e == l) //如果等于即为关键路径
printf("%c->%c ", G->vertex[i].name, G->vertex[j].name);
```
```
p = p->next;
}
}
```
```
free(topo);
}
```
```
#include "Queue.h"
#include "Stack.h"
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
```

#### AMGraph.h

```
#define MAXWEIGHT 99999 //最大权值
#define MAXVERTEX 20 //最大定点数
```
```
typedef char VertexType; //顶点用字符表示
typedef int MatrixType; //矩阵类型
```
```
struct Uset {
int adjvertex; //下标为i的点的邻接点
int weight; //当前权值
};
```
```
int Min_Uset(Uset *U, int n);
```
```
struct Eset {
int start;
int end;
int weight;
};
```
```
void Sort_Eset(Eset *E, int length);
```
```
#include "define_Graph.h"
```
```
#ifndef __GRAPH_H
#define __GRAPH_H
```
```
typedef struct __AMGraph {
VertexType vertex[MAXVERTEX];
MatrixType edge[MAXVERTEX][MAXVERTEX];
int vertices, edges;
} AMGraph;
```
```
int Locate_vertex(AMGraph *G, char v);
void print_Matrix_weighted(const AMGraph *G);
void print_Matrix_unweighted(const AMGraph *G);
void Creat_unAMGraph_unweightd(AMGraph *G);
void Creat_unAMGraph_weightd(AMGraph *G);
void Creat_AMGraph_weightd(AMGraph *G);
void Creat_AMGraph_unweightd(AMGraph *G);
```
```
void DFS_AM(AMGraph *G, int v, bool *visit);
void DFS_AMGraph(AMGraph *G, VertexType v);
```
```
void BFS_AM(AMGraph *G, int v, bool *visit);
void BFS_AMGraph(AMGraph *G, VertexType v);
```
```
void MST_Prim(AMGraph *G, VertexType v);
```
```
void InitEset(Eset *E, AMGraph *G);
void MST_Krusal(AMGraph *G);
```
```
void ShortestPath(AMGraph *G, VertexType v);
```

#### ALGraph.h

```
void ShortestPath_Dijkstra(AMGraph *G, VertexType v);
```
```
void ShortestPath(AMGraph *G, int v, int *path);
void ShortestPath_Dijkstra(AMGraph *G, VertexType v);
void print_path(AMGraph *G, int *path, int start, int end);
```
```
int **Path_Matrix(AMGraph *G);
void ShortestPath_Floyd(AMGraph *G, VertexType v1, VertexType v2);
#endif
```
```
#include "define_Graph.h"
```
```
#ifndef __ALGRAPH_H
#define __ALGRAPH_H
```
```
typedef struct __EdgeNode {
int adjvertex;
__EdgeNode *next;
int weight;
} EdgeNode;
```
```
typedef struct __ALGNode {
VertexType name;
EdgeNode *first;
} ALGNode;
```
```
typedef struct __ALGraph {
ALGNode vertex[MAXVERTEX];
int edges, vertices;
} ALGraph;
```
```
int Locate_vertex(const ALGraph *G, VertexType v);
void print_ALG_unweighted(const ALGraph *G);
void print_ALG_weighted(const ALGraph *G);
void Creat_unALGraph_unweighted(ALGraph *G);
void Creat_ALGraph_unweighted(ALGraph *G);
void Creat_unALGraph_weighted(ALGraph *G);
void Creat_ALGraph_weighted(ALGraph *G);
void DFS_AL(ALGraph *G, int v, bool *visit);
void DFS_ALGraph(ALGraph *G, VertexType v);
```
```
void BFS_AL(ALGraph *G, int v, bool *visit);
void BFS_ALGraph(ALGraph *G, VertexType v);
```
```
void MST_Prime(ALGraph *G, VertexType v);
```
```
void InitEset(Eset *E, ALGraph *G);
void MST_Krusal(ALGraph *G);
```
```
void InDegree(ALGraph *G, int *a);
int *Get_Topo(ALGraph *G);
void TopoSort(ALGraph *G);
```

void CriticalPath(ALGraph *G);
#endif


