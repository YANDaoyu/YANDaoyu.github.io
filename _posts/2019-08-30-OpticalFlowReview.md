---
layout: post
title: "Optical FLow in DeepLearning (Chinese&English)"
author: "Island"
mathjax: true
categories: PaperReview
tags: [algorithm, DeepLearning]
---

## Table of Review Papers

0. [Introduction](#Introduction)
1. [FlowNet](#flownet)
2. [FlowNet 2.0](#flownet-2.0)
3. [SpyNet](#spynet)
4. [PWC-Net](#pwc-net)


## Introduction

Based on the definition that introduced by James J. Gibson in the 1940s, 
Optical Flow is the apparent velocities of 
movement of brightness pattern in an image.    
根据James J. Gibson最初在1940s提出时的定义，光流反映的是观测平面上图案亮度的移动速度。最理想的情况是，在给定一个图像和对应的光流时，我们可以得到短时间后这个图像内物体的运动结果，此时光流场也是一个完美的运动场。

基于此种定义，我们不难得知，至少在**两张图物体像素强度不剧烈变化，且相邻像素变化趋势相似**的情况下我们才可以考虑计算光流。无论是传统方法（限制更多）还是深度学习方法，如果两张图像来自完全不同的场景，比如从哈利波特的一幕切换到了小黄人的一幕，这必然是完全不能计算光流的。简单而言，如果你自己都无法估计这两幕之间的转换，深度学习的方法也会面临同样的难题。

本文不会解释光流的传统算法，作者关于传统算法的学习笔记请点击[此处](need-to-be-written)跳转。

Ps. Gibson居然还提出过Affordance....吃惊。

## FlowNet
- [论文连接 Paper Link](https://arxiv.org/abs/1504.06852)

Summary: 

点击[此处](#table-of-review-papers)跳回**目录** /
Click [here](#table-of-review-papers) to jump back to 
the **CONTENT**.

## FlowNet 2.0

## SpyNet

## PWC-Net