---
title: SLAM
type: 术语
topic: 计算机视觉/几何与重建
aliases: ["Simultaneous Localization and Mapping", "同步定位与建图", "同时定位与地图构建"]
tags: [计算机视觉/术语, 术语/几何与重建]
status: 精进中
created: 2026-11-16
updated: 2026-11-17
source: "[[Szeliski-Computer-Vision-Algorithms-and-Applications-1st-draft-2010.pdf]]；具体节号、解释性质与核查范围见正文出处"
---

# SLAM

> [!abstract] 简明定义
> Simultaneous Localization and Mapping，同时定位与建图：在估计自身位姿的同时建立或更新环境表示的问题。

## 一、直观例子

> [!example] 教学情形
> 机器人进入未知房间，利用观测判断自身移动，并把新的环境结构加入地图；位姿和地图的估计相互影响。

## 二、易混与边界

不同系统可采用不同传感器与地图表示。回环检测常帮助约束漂移，但不能把某一具体模块作为所有 SLAM 定义中的必要实现。

## 三、出处与范围

[[Szeliski-Computer-Vision-Algorithms-and-Applications-1st-draft-2010.pdf]] 第 7 章导航应用讨论，PDF 第 390 页。 本轮定向核对相关段落，不认证该方向的全部算法或实现。
