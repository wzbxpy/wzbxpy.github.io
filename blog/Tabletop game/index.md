---
layout: default
title: 数据结构与算法-桌游
math: true
---

# 印加宝藏
![印加宝藏](inca.png){: style="max-width: 100%; height: auto; display: block; margin: 0 auto;" }

印加宝藏是一个经典的桌游，主要考验玩家的策略规划和资源管理能力。在游戏中，玩家共同进入祭坛或矿道，逐张抽取宝物与陷阱卡，依次决定“继续冒险”或“撤离带宝”。若触发重复陷阱，留下的玩家将失去本轮所有宝物；而撤离者则安全存入帐篷，并且单独撤退者还可获取神器。

## 极致简化版
在极致简化版中，玩家只需抽取宝物卡和陷阱卡，所有的宝物卡得分都设为1分。此外，为了避免陷阱卡的复杂性，我们假设只存在一张陷阱卡，一旦抽取就会触发陷阱。最后，我们先假设只有一名玩家参与游戏。

### 问题描述

- 输入
  - 给定n张卡片
    - n-1张得分为1的宝物卡
    - 1张陷阱卡
  - 已经翻开的卡片数量k
- 输出
  - 玩家是否应该继续冒险

### 建模

我们定义在第$k$张卡片翻开时，玩家继续冒险的期望收益为$E(k,continue)$，撤离的期望收益为$E(k,leave)$。当$E(k,continue) > E(k,leave)$时，玩家应该继续冒险；否则，玩家应该撤离。

- 如果玩家选择撤离，期望收益为$E(k,leave) = k$（因为已经翻开的卡片都是宝物卡，得分为1）。
- 如果玩家继续冒险，下一张卡片可能是陷阱卡或宝物卡：
  - 如果是陷阱卡，玩家将失去所有宝物，期望收益为0。
  - 如果是宝物卡，需要考虑剩余卡片的情况：
    - 继续冒险的期望收益为$E(k+1, continue)$（当前宝物得分加上后续的期望收益）。
    - 撤离的期望收益为$E(k+1, leave)$（当前宝物得分加上后续的期望收益）。

接下来，我们分析在第$k$张卡片翻开时，发生陷阱卡的概率为$\frac{1}{n-k}$，发生宝物卡的概率为$\frac{n-1-k}{n-k}$。
因此，继续冒险的期望收益可以表示为：
