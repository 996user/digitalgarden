---
{"dg-publish":true,"permalink":"/data-structure//","tags":["数据结构","线性表"]}
---

# 线性表的逻辑结构和基本操作

## 基本操作

- InitList(&L) 初始化线性表返回一个空的线性表
- ListEmpty(L) 判断线性表是否为空，是则返回 true，否则返回 false
- ClearList(&L) 将线性表清空，即将所有元素删除
- GetElem(L, i, ~~&e~~) 获取线性表第 i 个位置的元素，将其存储在 e 中，若 i 不合法则返回错误信息
- LocateElem(L, e, ~~compare~~) 在线性表中查找值为 e 的元素，并返回其位置，若不存在则返回 0。其中 compare 是一个函数指针，用于比较两个元素是否相等。
- ListInsert(&L, i, e) 在线性表的第 i 个位置插入值为 e 的元素，若 i 不合法则返回错误信息
- ListDelete(&L, i, &e) 删除线性表第 i 个位置的元素，并将其存储在 e 中，若 i 不合法则返回错误信息
- ListLength(L) 返回线性表的长度
- PrintList(L) 遍历输出线性表
- DestoryList(&L) 销毁线性表销毁线性表就是释放线性表所占用的内存空间，让其成为一个空表。具体实现可以通过遍历线性表，逐个释放节点所占用的内存空间，最后将头指针指向 NULL 来实现。
