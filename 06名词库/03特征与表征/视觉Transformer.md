---
title: 视觉Transformer
type: 术语
topic: 计算机视觉/特征与表征
aliases: ["vision transformer", "ViT"]
tags: [计算机视觉/术语, 术语/特征表征]
status: 精进中
created: 2026-11-16
updated: 2026-11-17
source: "[[Dosovitskiy2020-An-Image-is-Worth-16x16-Words-Transformers-for-Image-Recognition-at-Scale.pdf]]；具体节号、解释性质与核查范围见正文出处"
---

# 视觉Transformer

> [!abstract] 简明定义
> 以 Transformer 处理视觉 token 表示的一类模型；原始 ViT 将图像块嵌入为序列，通过自注意力及 MLP 处理，再读取图像表示。

## 一、直观例子

> [!example] 教学计算
> 把图像切成许多固定大小的块，每块得到一个向量。模型计算块与块之间的信息关系，而不是把每个像素的 RGB 值直接当作一个类别。

## 二、易混与边界

图像块的数量、展平维度和嵌入维度是三个量。原始 ViT 有可学习位置嵌入，不是完全没有空间先验。Transformer 架构也不自动等于基础模型或多模态模型。

## 三、出处

[[Dosovitskiy2020-An-Image-is-Worth-16x16-Words-Transformers-for-Image-Recognition-at-Scale.pdf]] 第 3.1 节、图 1；详解见 [[论文-Dosovitskiy-ViT]]。
