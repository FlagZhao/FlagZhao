---
title: "Leveraging AI Ecosystem for Portable and Sustainable GPU Kernels in HPC"
collection: publications
category: workshops
permalink: /publication/2026-06-triton-hpc-array
excerpt: 'An AOT compilation framework that integrates Triton with C/C++ HPC codebases, producing standalone shared libraries with the performance of hand-tuned CUDA.'
date: 2026-06-16
venue: 'ARRAY 2026 (ACM SIGPLAN International Workshop on Libraries, Languages and Compilers for Array Programming)'
paperurl: 'https://pldi26.sigplan.org/details/ARRAY-2026-papers/3/Leveraging-AI-Ecosystem-for-Portable-and-Sustainable-GPU-Kernels-in-HPC'
citation: '<b>Yanbo Zhao</b>, Zhaonan Meng, Teja Manthena, Xu Liu, Ajay Panyala, and Jiajia Li. (2026). &quot;Leveraging AI Ecosystem for Portable and Sustainable GPU Kernels in HPC.&quot; <i>ARRAY 2026</i>.'
---

## Abstract

This work, conducted during a research internship at Pacific Northwest National Laboratory (PNNL), presents an ahead-of-time (AOT) compilation framework that integrates Triton with C/C++ HPC codebases. The framework auto-generates optimized GPU code together with a C++ wrapper and packages them into standalone shared libraries, delivering performance on par with hand-tuned CUDA. Triton kernels compiled this way run across NVIDIA and AMD GPUs without modification and achieve near-parity performance with native implementations on tile-friendly workloads, while irregular kernels reveal current limitations of the tile-based programming model.

## Venue

ARRAY 2026 - ACM SIGPLAN International Workshop on Libraries, Languages and Compilers for Array Programming (co-located with PLDI 2026). [Program page](https://pldi26.sigplan.org/details/ARRAY-2026-papers/3/Leveraging-AI-Ecosystem-for-Portable-and-Sustainable-GPU-Kernels-in-HPC)
