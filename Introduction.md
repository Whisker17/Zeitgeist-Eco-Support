# Zeitgeist 需求文档

## 简介

Zeitgeist 是一个用于预测市场和 Futarchy 的不断发展的区块链。Zeitgeist 是为 Polkadot 和 Kusama 生态系统设计的，它将自己设想为 Web3 上预测市场的枢纽。Zeitgeist 不仅要打造一个平台，还要打造一个预测市场的生态系统。

### 什么是预测市场？

预测市场是一个交易与未来事件的潜在结果相关的资产的开放市场。它们是一种整合来自不同参与者的信息工具，并为未来事件创建强大的概率信号。

预测市场已被证明是创造准确概率信号的极好工具，胜过民调等其他常用方法。它们通过激励参与者通过资产交易揭示他们对事件的了解来实现这一点。这些信息是高保真的，因为参与者必须确保自己的信息的可信度，如果他们在结果中处于失败的一方，就会蒙受损失。

### 什么是Futarchy？

Futarchy 是一种治理系统，它根据预测市场产生的信号做出政策决定。

它的概念最初是由 Robin Hanson在题为 ”为价值投票，为信仰下注“ 的短篇文章被提出来的，在文章中他阐明了 Futarchy 可能如何改善当前民主运作的某些方面——最显著的是通过创造一种更好的方式来判断政策决定的潜在利益。

然而，在公司治理、公共政策决策或城市规划等场景下，futarchy 通常是以一个不适合应用的且相当陌生的概念存在的。

### 技术介绍

从上层看，其架构非常简单：预测市场上的不同结果由交易者可以买卖的股权表示。因此，每一股都代表着对结果的质押。一旦事件被“解决”，并且结果已知，“获胜”的股权可以兑换为代币，而代表落败的那一方的股份则失去价值。

争议系统以一种去中心化法院的形式存在，随机选择先前在法院系统中抵押代币的陪审员，对“实际”结果进行投票。如果市场对投票结果不满意，可以通过将所需的押金加倍来升级挑战，以吸引更多的陪审员。最终，要么第一批陪审员被惩罚（如果他们的裁决与后来加入的更大规模的委员会不同），要么挑战者将被惩罚。这个过程可以通过进一步增加押金和吸引更广泛的陪审员来重复。

![](https://raw.githubusercontent.com/Whisker17/ImageStoreService/main/image-20211121231452884.png)

如果深入一些，建立一个好的预测市场需要结构良好的自动化做市商 (AMM) 和足够的激励结构，因为在最佳架构中，预测市场应该代表对每个结果的公共信心水平。大家可以在 Zeitgeist 博客上找到对 AMM 机制的[深入研究](https://blog.zeitgeist.pm/introducing-zeitgeists-rikiddo-scoring-rule/)。

### 一图了解Zeitgeist

![](https://raw.githubusercontent.com/Whisker17/ImageStoreService/main/image-20211121231502402.png)

## 生态扩展计划

目前还没有针对生态扩展的官方计划放出，应该会在 2022 年上半年颁布，但是会提前开始布局整个预测市场生态，目前希望能有一些类似于针对市场的**套利机器人**或者对**市场数据的分析**等的小工具作为生态的基础工具，我们也会为优秀的项目提供 grant，以支持这些项目的后续迭代。

### SDK

https://github.com/zeitgeistpm/tools/tree/main/packages/sdk

### SDK 文档

即将推出

### RPC 试用

https://polkadot.js.org/apps/?rpc=wss://bsr.zeitgeist.pm#/chainstate

### 更多信息

官网：https://zeitgeist.pm/

官方博客：https://blog.zeitgeist.pm/

官方 Repo：https://github.com/ZeitgeistPM

