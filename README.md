<!-- # Zhibin Wang (王智彬) -->
## Biography
I am a assistant researcher in School of Intelligent Software and Engineering, Nanjing University.
I received my Ph.D. degree in School of Computer Science, Nanjing University, advised by [Prof. Chen Tian](https://cs.nju.edu.cn/tianchen/index.htm) and [Prof. Sheng Zhong](https://cosec.nju.edu.cn/ae/82/c47361a568962/page.htm). I have been interning at [GraphScope](https://graphscope.io/) team in Alibaba DAMO Academy from 2021 to 2024, supervised by [Longbin Lai](https://lai.me/). 
My research interests include accelerating subgraph matching and other graph algorithms using new hardware, especially GPUs. Recently, I am engaged in accelerating LLM inference. 
Related research has been published in top-tier conferences, such as SIGMOD, PPoPP and ATC.

<!-- 王智彬，南京大学智能软件与工程学院助理研究员。2018年至2024年在南京大学计算机科学与技术学院攻读博士学位，导师为[田臣](https://cs.nju.edu.cn/tianchen/index.htm)教授和[仲盛](https://cosec.nju.edu.cn/ae/82/c47361a568962/page.htm)教授。2021年至2024年在阿里巴巴达摩院[GraphScope](https://graphscope.io/)团队实习，导师为[赖龙彬](https://lai.me/)。研究方向包括加速图计算和大模型推理。作为第一作者发表了南大第一篇SIGMOD（数据库顶会）论文和南大第一篇PPoPP（高性能计算顶会）论文。 -->

## Prospective Students
__We are looking for self-motivated students who are interested in graph algorithms and LLM systems. We welcome students with strong algorithmic, mathematical, and programming skills. Please contact me by email with your CV.__

## Education

`Sept. 2018 - Sept. 2024`
__Nanjing University__
- Ph.D. in Computer Science and Technology

`May 2021 - July 2024`
__Alibaba DAMO Academy__
- Research intern in GraphScope team

<!-- `Sept. 2014 - June 2018`
__Nanjing University of Aeronautics and Astronautics__
- B.E. in Computer Science and Technology -->


## Research
    
  - `April 2021 - April 2022` __Zhibin Wang__, Longbin Lai, Yixue Liu, Bing Shui, Chen Tian, Sheng Zhong.
    _I/O-Efficient Butterfly Counting at Scale_
    SIGMOD 23
    - Derive a new I/O lower bound of butterfly counting on hierarchical memory by proposing a new class of algorithms called the semi-witnessing algorithm.
    - Develop IOBufs algorithm that approaches the I/O lower bound.
    - Parallelize IOBufs with a fine-grained approach that carefully trade-off the the I/O-efficiency and parallelism.

  - `Nov. 2019 - Feb. 2021` Santosh Pandey, __Zhibin Wang (co-first author)__, Sheng Zhong, Chen Tian, Bolong Zheng, Xiaoye Li, Lingda Li, Adolfy Hoisie, Caiwen Ding, Dong Li, Hang Liu.
    _TRUST: Triangle Counting Reloaded on GPUs_
    TPDS
    - Implement a vertex-centric hashing-based triangle counting on GPUs with GPU-friendly hashtable layout.
    - Propose graph reordering to reduce collision in hashtable, virtual combination to balance intra-vertex workload, and degree-aware resources allocation to further reduce collision and balance inter-vertex workload.
    - Scale triangle counting to 1024 GPUs via a graph and workload collaborative partitioning.
    
  - `April 2021 - April 2022` __Zhibin Wang__, Zizhao Zhang, Ziwei Zhang, Shihui Ying, Yue  Gao, Yuan Zhang, Sheng Zhong
    _Privacy-preserving Joint Hypergraph Learning_
    Submitted to TPAMI
    - Design two protocols to help multiple parties aggregating their private hypergraph data and conduct joint hypergraph learning in a privacy-preserving manner.
    - Protocols based on light-weight cryptographic primitives, including pseudo-random number generators, sum-preserving matrix confusions, and matrix multiplication-based encryptions.


  - `June 2022 - Dec. 2022` Longbin Lai, Yufan Yang, __Zhibin Wang__, Yuxuan Liu, Haotian Ma, Sijie Shen, Bingqing Lyu, Xiaoli Zhou, Wenyuan Yu, Zhengping Qian, Chen Tian, Sheng Zhong, Yeh-Ching Chung, Jingren Zhou
    _GLogS: Interactive Graph Pattern Matching Query At Large Scale_
    Submitted to ATC 23
    - Design a compilation stack that compiles declarative GPM queries into distributed programs.
    - Propose an optimizer that can automatically derive optimal execution plans for GPM queries.
    - Implement a system that allows users to interactively submit and efficiently execute GPM queries at large scale.

## Honors & Awards
- `2015` __Gold Medal__ ACM-ICPC Asia Regional Contest(Chang Chun Site)
- `2015` __China National Scholarship__ 
- `2016` __Outstanding Undergraduate Award__ CCF(China Computer Federation)
