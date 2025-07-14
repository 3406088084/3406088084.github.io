---
layout: default
title: 算法精要
parent: computer-science
grand_parent: ——docs
nav_order: 2
date: 2023-10-15
---

# 算法精要

## 引言
算法是计算机科学的核心，本文探讨几种基础算法及其应用。

## 排序算法
### 快速排序
快速排序是一种分而治之的算法...

```python
def quicksort(arr):
    if len(arr) <= 1:
        return arr
    pivot = arr[len(arr) // 2]
    left = [x for x in arr if x < pivot]
    middle = [x for x in arr if x == pivot]
    right = [x for x in arr if x > pivot]
    return quicksort(left) + middle + quicksort(right)
复杂度分析
算法	平均复杂度	最坏复杂度
快速排序	O(n log n)	O(n²)
归并排序	O(n log n)	O(n log n)
应用案例
数据库索引

大数据处理

机器学习特征排序
