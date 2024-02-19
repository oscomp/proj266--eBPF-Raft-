## 标题

基于eBPF的Raft协议加速

## 项目描述

Raft协议为当前国际广泛采用的分布式共识算法，用在etcd等分布式存储系统中实现数据复制。目前，Raft协议在用户态实现，执行过程中会引发用户态和核心态的频繁切换，且需经过内核网络协议栈，产生较大的性能开销。

eBPF是Linux内核的新特性，支持用户在内核里安全运行自定义的功能。可以采用eBPF在内核态实现Raft协议中关键流程，从而提高性能。

## 预期目标

- 基于Raft协议的开源实现Dragonboat，实现通过eBPF程序将Raft协议的消息转发和接收流程卸载到内核运行，从而加速Raft协议的性能

## 特征

- 掌握Dragonboat的相关代码
- 掌握eBPF的基本原理和编程方法
- 掌握Linux内核网络协议栈报文收发相关代码

## 已有参考资料

- Zhou, Yang et al. “Electrode: Accelerating Distributed Protocols with eBPF”. Symposium on Networked Systems Design and Implementation (2023).
- [Dragonboat](https://github.com/lni/dragonboat)
- [eBPF](https://ebpf:io)

## 赛题分类

2.3 操作系统内核大类  -->  2.3.4 新型模块化组件

## 参赛要求

- 请遵循“2024全国大学生操作系统比赛”的章程和技术方案要求
- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生或研究生
- 允许学生参加大赛的多个不同题目，最终自己选择一个题目参与评奖

## 难度

- 难度等级：高等

## License

GPL-3.0 License

## 所属赛道

2024全国大学生操作系统比赛的“OS功能挑战”赛道

## 项目导师

- 姓名：任怡
- 单位：国防科技大学
- github ID：[https://github.com/Ren-Xiaoyi](https://github.com/Ren-Xiaoyi)
- email：[renyi@nudt.edu.cn](mailto:renyi@nudt.edu.cn)
