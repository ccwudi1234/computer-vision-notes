---
title: BRDF
type: 术语
topic: 计算机视觉/成像与物理
aliases: ["双向反射分布函数"]
tags: [计算机视觉/术语, 术语/成像物理]
status: 精进中
created: 2026-11-16
updated: 2026-11-17
source: "[[Szeliski-Computer-Vision-Algorithms-and-Applications-1st-draft-2010.pdf]]；具体节号、解释性质与核查范围见正文出处"
---

# BRDF

> [!abstract] 简明定义
> 双向反射分布函数，描述给定表面局部位置和波长时，反射怎样随入射与出射方向变化的模型。

## 一、直观例子

> [!example] 教学情形
> 观察一张光滑桌面时，移动视角可能让高光出现或消失；同一材质在不同方向的反射响应不能只用一个固定颜色解释。

## 二、必要原理与边界

原文写作 $f_r(\theta_i,\phi_i,\theta_r,\phi_r;\lambda)$。两组角度分别描述入射和出射方向，$\lambda$ 为波长。

**不要混淆：** BRDF 不是随意取值于 0 到 1 的“颜色比例”。局部表面反射模型也不自动涵盖所有空间变化、次表面散射或大气效应。

## 三、出处与范围

[[Szeliski-Computer-Vision-Algorithms-and-Applications-1st-draft-2010.pdf]] 第 2.2.2 节、式 2.81、图 2.15，PDF 第 84 页。
