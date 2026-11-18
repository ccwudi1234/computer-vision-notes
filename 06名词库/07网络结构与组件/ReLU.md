---
title: ReLU
type: 术语
topic: 计算机视觉/网络结构与组件
aliases: ["Rectified Linear Unit", "修正线性单元", "rectifier"]
tags: [计算机视觉/术语, 术语/网络结构与组件]
status: 精进中
created: 2026-11-17
updated: 2026-11-17
source: "[[Krizhevsky2012-AlexNet-ImageNet-Classification.pdf]]；具体节号、解释性质与核查范围见正文出处"
---

# ReLU

> [!abstract] 简明定义
> Rectified Linear Unit，整流线性单元：对正输入保留其值，对负输入输出零的激活函数。

## 一、公式与例子

$$
f(x)=\max(0,x).
$$

教学示例：$f(3)=3$，$f(-2)=0$。它作用于各个输入元素，不是计算整个向量中的最大元素。

## 二、易混与边界

正输入处导数为 1，负输入处为 0；零点不可微，算法需要相应的实现约定。因此“不饱和”不意味着处处有非零梯度，也不保证所有深网络都容易优化。

在 [[论文-Krizhevsky-AlexNet]] 中，它是具体训练系统的一部分；原文图 1 的速度对照发生在 CIFAR-10 特定四层网络上，不能作为所有模型的通用加速比。

## 三、出处

[[Krizhevsky2012-AlexNet-ImageNet-Classification.pdf]] 第 3.1 节及图 1；本卡定义与函数值直接对应原式。
