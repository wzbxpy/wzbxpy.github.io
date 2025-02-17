---
layout: default
title: learning
---
# 各个方向的学习内容

因为这个网页做的匆忙，所以内容还不全，但我会努力更新的！！！
同学们有什么问题可以随时联系我，微信：wzbxpy

__ACK：感谢林夕，周宇航，李世鹏，张中辉对这个网页的帮助__

## 高性能计算 (HPC)

- __GPU课程__：
  
一个比较老的课程：[链接](https://youtube.com/playlist?list=PLAwxTw4SYaPnFKojVQrmyOGFCqHTxfdv2&si=a26iDjQSZrHaQu3U) 

最新的课程：[链接](https://canvas.illinois.edu/courses/49985/assignments/syllabus)

ppt在：[链接](https://github.com/jiadong5/ECE408_FA23_UIUC/tree/master/Lecture%20Notes%20and%20Exam%20Samples/lectures)

- __并行/分布式算法__：6.506 Algorithm Engineering Spring 2024 
[链接](https://jshun.csail.mit.edu/6506-s24/)

## 数据库以及图计算 (DB)

- 图计算：[链接](https://jshun.csail.mit.edu/6886-s18/) （但说实话和并行算法有点像，可以学并行算法）

## 大模型系统 (LLM System)

__入门视频__

【Transformer论文逐段精读【论文精读】】 [链接](https://www.bilibili.com/video/BV1pu411o7BE/?share_source=copy_web&vd_source=3cd0b30eec09a569a546f443e016f6cc)

【68 Transformer【动手学深度学习v2】】 [链接](https://www.bilibili.com/video/BV1Kq4y1H7FL/?share_source=copy_web&vd_source=3cd0b30eec09a569a546f443e016f6cc)

- __算法课程__：[链接](https://web.stanford.edu/class/cs25/index.html) 不过没有lab，都是视频

- __系统课程__：[链接](https://dlsyscourse.org/lectures/)，[链接](https://hanlab.mit.edu/courses/2024-fall-65940) 有lab和视频


## 近似算法

### 图采样算法
[链接](https://www.usenix.org/conference/atc23/presentation/lai)
可以看一下这个论文以及附录的证明，特别是那个采样的分析，看看对这种数学的分析感不感兴趣

### 向量数据库
- __系统方向__ [Glogs](https://www.usenix.org/conference/nsdi24/presentation/zhang-zili-pipelining) 这个是向量数据库最新的论文，可以看一下，看看对这种系统的设计感不感兴趣
- __算法方向__ 先简单学一下这个课程 [链接](https://www.youtube.com/watch?v=sKyvsdEv6rk)

_除了上述内容，也可以学习数据挖掘的内容，有很大一部分是向量数据库的内容_

### 数据挖掘

建议学习课程 CS246W: Mining Massive Datasets, Stanford University

课程：[链接](http://cs246w.stanford.edu/) (不过好像打不开了)

视频在：[链接](https://www.youtube.com/playlist?list=PLLssT5z_DsK9JDLcT8T62VtzwyW9LNepV)

## AI算法, 图神经网络 (GNN)

建议学习课程 CS224W: Machine Learning with Graphs, Stanford University

课程：[链接](http://cs224w.stanford.edu/)

视频在：[链接](https://www.youtube.com/playlist?list=PLoROMvodv4rPLKxIpqhjhPgdQy7imNkDn)


# 一些项目

### Leiden算法在GPU上的实现 （HPC，图计算，近似算法，DB）
社区检测的一些介绍: [链接](https://www.zhihu.com/question/29042018/answer/2216618374)

Leiden算法的论文：[链接](https://www.nature.com/articles/s41598-019-41695-z)

__进度__：我们基于Leiden算法的前置算法Louvain已经在GPU上实现了（发表在PPoPP， CCF A，南大第一篇），扩展到Leiden算法应该不难

__目标__：扩展到Leiden可以再发一篇A类期刊，另外可以把这个项目拿去参加挑战杯（如果要参加请尽快联系我）

### 使用GPU加速向量数据库的查询 （HPC，近似算法，DB）

__进度__：我们已经在GPU上实现了一个简单的向量数据库

__任务__：参与查询算法的优化，以及GPU上的实现

### Fault Tolerance in LLM Training （LLM System，HPC）

已完成相关论文：[Unicron: Economizing self-healing llm training at scale.](https://arxiv.org/pdf/2401.00134)

__正在和华为合作做这个topic__

__有一个博士生在做这个方向，可以和他一起做__

### ASPLOS的比赛

[链接](https://github.com/asplos-contest/2025/tree/main)

__有个ACM金牌的大四学长在做，可以一起做__

### Multi-Agent （AI算法，LLM System）

论文：[链接](https://arxiv.org/pdf/2402.01680)

__进度__：刚刚开始

### LLM inference中Decoding阶段复用kv cache （LLM System，HPC）

__相关论文__

Flash attention: [链接](https://github.com/Dao-AILab/flash-attention)
- Describe how to decompose the attention operation

SpecInfer: Accelerating Large Language Model Serving with Tree-based Speculative Inference and Verification
- How to verify tree-based decoding token

__最新进展__

Bifurcated Attention: Accelerating Massively Parallel Decoding with Shared Prefixes in LLMs

Hydragen: High-Throughput LLM Inference with Shared Prefixes

