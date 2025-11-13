---
title: "RedSan: Redundant Memory Instruction Sanitizer for GPU Programs"
collection: publications
category: conferences
permalink: /publication/2025-11-redsan-sc
excerpt: 'A novel dynamic binary instrumentation tool to automatically detect and quantify redundant memory instructions in fully optimized GPU applications, achieving up to 6.27x performance speedup.'
date: 2025-11-01
venue: 'SC 2025 (International Conference for High Performance Computing, Networking, Storage and Analysis)'
paperurl: ''
citation: '<b>Yanbo Zhao</b>, Yueming Hao, Zecheng Li, Shuyin Jiao, Xu Liu, and Jiajia Li. (2025). &quot;RedSan: Redundant Memory Instruction Sanitizer for GPU Programs.&quot; <i>SC 2025</i>.'
---

## Abstract

RedSan is a dynamic binary instrumentation tool that operates without source code to automatically detect and quantify redundant memory instructions in GPU applications. By pinpointing these inefficiencies, the tool guided targeted code optimizations that achieved up to a 6.27× performance speedup and a 3.00× reduction in memory operations across HPC and AI benchmarks.

## Key Contributions

- **Core Functionality**: RedSan automatically detects and quantifies redundant memory instructions (dead stores, dead loads, and oversync) in GPU applications without requiring source code access.

- **Performance Impact**: Enabled performance gains of up to 6.27× speedup and 3.00× reduction in memory operations across various HPC and AI benchmarks through guided optimizations.

- **Broader Discoveries**: Uncovered a previously undocumented compiler correctness issue with CUDA's `__restrict__` keyword and identified optimization opportunities within NVIDIA's highly-tuned cuSPARSE and cuSOLVER libraries.

## Venue

SC 2025 - The International Conference for High Performance Computing, Networking, Storage and Analysis (Accepted, to appear)

