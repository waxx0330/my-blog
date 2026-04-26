---
title: "构建一个论文辅助阅读智能体：从 RAG 到 Reflection"
description: "如何让智能体稳定总结论文、回答问题、比较多篇论文观点，并尽可能忠于原文。"
date: "2026-04-26"
category: "Agent"
tags: ["RAG", "Reflection", "Paper Reading"]
draft: false
---

# 构建一个论文辅助阅读智能体：从 RAG 到 Reflection

这篇文章记录我对论文辅助阅读智能体的设计思考。

## 为什么需要 RAG？

学术论文通常很长，直接塞进模型上下文并不稳定。

## 系统结构

一个比较稳妥的结构是：

1. 文档解析
2. 分块
3. 向量检索
4. 引用定位
5. 回答生成
6. 自我检查