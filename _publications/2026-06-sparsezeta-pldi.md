---
title: "SparseZETA: Intelligent Auto-tuner for Designing High-Performance SpMV Programs"
collection: publications
category: conferences
permalink: /publication/2026-06-sparsezeta-pldi
excerpt: 'An intelligent auto-tuner for designing high-performance sparse matrix-vector multiplication (SpMV) programs.'
date: 2026-06-19
venue: 'PLDI 2026 (ACM SIGPLAN Conference on Programming Language Design and Implementation)'
paperurl: 'https://pldi26.sigplan.org/details/pldi-2026-papers/70/SparseZETA-Intelligent-Auto-tuner-for-Designing-High-Performance-SpMV-Programs'
citation: 'Zhen Du, Ying Liu, Xionghui Chen, <b>Yanbo Zhao</b>, Xiaobing Feng, Huimin Cui, and Jiajia Li. (2026). &quot;SparseZETA: Intelligent Auto-tuner for Designing High-Performance SpMV Programs.&quot; <i>PLDI 2026</i>.'
---

## Abstract

SparseZETA is an intelligent auto-tuner that designs high-performance SpMV programs by imitating and combining the actions of human experts. It formulates program design as behavior cloning, predicting design actions step by step from the state of the partially built program instead of exploring costly alternatives, and uses a self-training mechanism to accelerate training data collection. On NVIDIA A100 and RTX 2080 Ti GPUs, SparseZETA outperforms existing auto-tuners, human-designed programs, and a sparse compiler, while reducing design time from days or months to tens of milliseconds per matrix.

## Venue

PLDI 2026 - ACM SIGPLAN Conference on Programming Language Design and Implementation ([program page](https://pldi26.sigplan.org/details/pldi-2026-papers/70/SparseZETA-Intelligent-Auto-tuner-for-Designing-High-Performance-SpMV-Programs))
