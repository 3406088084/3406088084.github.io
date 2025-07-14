---
layout: default
title: 交通流理论
parent: transportation
grand_parent: _docs
nav_order: 1
date: 2023-10-10
---

# 交通流理论与模型

## 基本参数
交通流理论中的三个基本参数：

- 流量 (Q): 单位时间内通过某点的车辆数
- 密度 (K): 单位长度内的车辆数
- 速度 (V): 车辆行驶速度

## 格林希尔治模型
格林希尔治线性模型描述速度-密度关系：

$$
V = V_f \left(1 - \frac{K}{K_j}\right)
$$

其中：
- $V_f$ = 自由流速度
- $K_j$ = 阻塞密度

## 交通流模拟
```mermaid
graph TD
    A[交通需求] --> B(路网结构)
    B --> C{交通分配模型}
    C --> D[用户均衡]
    C --> E[系统最优]
实际应用
交通拥堵预测

信号配时优化

路网容量分析
