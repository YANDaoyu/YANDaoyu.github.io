---
layout: post
title: "Optical FLow in DeepLearning (Chinese&English)"
author: "Island"
mathjax: true
categories: PaperReview
tags: [algorithm, DeepLearning]
image: /OpticalFlow/OP.GT.png
---

## 目录 Table of Review Papers

0. [引言 Introduction](#引言-introduction)   
   0. [数据集一览 Datasets OverView](#数据集一览-datasets-overview)
1. [FlowNet](#flownet)
2. [FlowNet 2.0](#flownet-2.0)
3. [SpyNet](#spynet)
4. [PWC-Net](#pwc-net)
5. [Devon](#devon)

本文不会解释光流的传统算法，作者关于传统算法的学习笔记请点击[此处(还没有写)]()跳转。  
In this blog, there won't be any illustration about traditional methods of Optical Flow. The note of traditional methods is [here(not exist yet)]().

## 引言 Introduction

重点：先问光流在这些场景存不存在，再考虑光流怎么估计。  
KEY: Ask yourself if the Optical Flow **EXIST OR NOT** in such scenes before considering the estimation of the Optical Flow in these scenes.
   
根据James J. Gibson最初在1940s提出时的定义，光流反映的是观测平面上图案亮度的移动速度。最理想的情况是，在给定一个图像和对应的光流时，我们可以得到短时间后这个图像内物体的运动结果，此时光流场也是一个完美的运动场。   
Based on the definition that introduced by James J. Gibson in the 1940s, 
Optical Flow is the apparent velocities of 
movement of brightness pattern in an image.
Ideally, we can get the motion of the object in an image 
after a short time when given an initial image 
and corresponding optical flow, 
then the optical flow field is also a perfect motion field. 

基于此种定义，我们不难得知，至少在**两张图物体像素强度不剧烈变化，且相邻像素变化趋势相似**的情况下我们才可以考虑计算光流。无论是传统方法（限制更多）还是深度学习方法，如果两张图像来自完全不同的场景，比如从哈利波特的一幕切换到了小黄人的一幕，这必然是完全不能计算光流的。简单而言，如果你自己都无法脑内演变这两幕之间的转换，深度学习的方法也会面临同样的难题。   
Based on this definition, it is not difficult to notice that 
we can consider estimate the optical flow at least in the case 
where **the pixel intensity of the two image objects doesn't change a lot and the neighboring pixels have similar trends**. 
Whether it's a traditional method (which has more restrictions) or a deep learning method, if the two images come from completely different scenes, such as switching from Harry Potter to Despicable Me, 
the optical flow cannot be calculated at all. 
In short, if you can't image the transition between the two scenes in your own mind, the deep learning method will face the same difficulties.

> 写到这里我想起《数字乌托邦》中提到过的一句：“如果你想让人工智能超过人类智能，有两种方法可供选择：让机器变聪明或让人类变蠢。” 希望人工智能最后不是以第二种方式成熟完善。   
> 有一说一，我在这里瞎希望其实一点儿用也没有。当代人类都愿意使用完全没有研究透的技术去“创造”新的技术了，还有什么懒是不会去躲的。：）   
> 再扯远一点，我希望未来神经网络的每一个参数的选择都可以**被严格证明最优性**。

在万物皆可深度学习的荒谬时代，当下的*科学家/工程师*必然不会放过这个角落。接下来我会浅谈*我认为*这些论文都尝试了些什么，以及达到了什么效果。当然，请不要被我的浅薄思想所限制，我欢迎一切条理清晰的反驳。

Ps. Gibson居然还提出过Affordance....吃惊。被UID支配的恐惧kkkkk

### 数据集一览 Datasets Overview
- [Middlebury](http://vision.middlebury.edu/flow/)
- [KITTI](http://www.cvlibs.net/datasets/kitti/)
- [MPI Sintel](http://sintel.is.tue.mpg.de/downloads)
- [Flying Chairs](https://lmb.informatik.uni-freiburg.de/resources/datasets/FlyingChairs.en.html)

![Sintel](/assets/img/OpticalFlow/Sintel.png)

| 数据集 dataset | 数量 size | 描述 description | 真值说明 GT notes |
| -------       | ---- | ----------- | ------------ |
| Middlebury    | 3+4+1 | 共三种情景的数据和真值，在网站上还可以测试8组 | 部分由LK法计算得到，部分是合成场景，少量通过结构化照明得到|
| | | contains 3 types of data with GT, and the website also provides 8 pairs data for testing | 3 of them were calculated by LK method, 4 of them were synthetic data, and 1 of them got the GT by structured light |
| KITTI         | 194+200 | 车辆驾驶相关的数据，测试数据有395组 | 采集时有深度，可以直接计算 |
| | | driving scenes data, the website provides 395 pairs of image for testing | the data is recorded with depth information, which means the optical flow can be computed directly |
| MPI Sintel    | 1041 | 来自3D动画Sintel | 根据对应点的二维坐标计算 |
| | | made from Sintel movie | GT based on the point's 2D-coordinate |
| Flying Chairs | 22872 | 根据仿射变换合成结果 | 基于仿射变换得到，和之前的合成场景相同 |
| | | affine transformation | same as previous methods |






## FlowNet
- [论文连接 Paper Link](https://arxiv.org/abs/1504.06852)

总览：


点击[此处](#目录-table-of-review-papers)跳回**目录** /
Click [here](#目录-table-of-review-papers) to jump back to 
the **CONTENT**.

## FlowNet 2.0
- [论文连接 Paper Link](https://arxiv.org/abs/1612.01925)

## SpyNet
- [论文连接 Paper Link](https://arxiv.org/abs/1611.00850)

## PWC-Net
- [论文连接 Paper Link](https://arxiv.org/abs/1709.02371)

## Devon
- [论文连接 Paper Link](https://arxiv.org/abs/1802.07351)