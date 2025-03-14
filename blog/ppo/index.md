---
layout: default
permalink: /blog/ppo
---

# PPO算法

## 整体流程
![Overview](overview.png){: style="max-width: 100%; height: auto; display: block; margin: 0 auto;" }

## 强化学习
![alt text](image.png){: style="max-width: 100%; height: auto; display: block; margin: 0 auto;" }

### 一些基本概念
- __action space__：动作空间，即agent可以采取的动作的集合
- __state space__：状态空间，即agent可以观察到的状态的集合
- __policy__：策略，即agent在某个状态下采取某个动作的概率分布

$$\pi(a|s)$$

表示在状态$s$下，agent采取动作$a$的概率。这个策略一般是要学习的对象。

- __trajectory__：轨迹，即agent在环境中的一次交互序列

$$\tau = (s_0, a_0, s_1, a_1, \cdots)$$

其中$s_i$表示第$i$个状态，$a_i$表示第$i$个动作。

- __reward__：奖励，即agent在某个状态下采取某个动作后得到的奖励

$$r(s, a)$$

表示在状态$s$下，agent采取动作$a$后得到的奖励。

- __return__：回报，对于一个轨迹$\tau$，其回报定义为

$$R(\tau) = \sum_{t=0}^{\infty} r(s_t, a_t)$$

即轨迹中所有奖励的和。

### 强化学习的目标
强化学习的目标是找到一个策略$\pi$，使得agent在环境中的return最大。这个return最大可以用两种方式来定义：

对于任意的状态$s$，$\pi$给出相应的动作$a$，使得agent的 _期望_ 回报最大：




