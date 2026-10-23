---
title: "cuThermo: Understanding GPU Memory Inefficiencies with Heat Map Profiling"
collection: publications
category: preprints
permalink: /publication/2025-cuthermo-arxiv
excerpt: 'A novel GPU memory profiler utilizing dynamic binary instrumentation and heat map visualization to identify runtime inefficiencies, achieving speedups of up to 721.79%.'
date: 2025-07-24
venue: 'arXiv Preprint (Under Review)'
paperurl: 'https://arxiv.org/abs/2507.18729'
citation: '<b>Yanbo Zhao</b>, Jinku Cui, Zecheng Li, Shuyin Jiao, Xu Liu, and Jiajia Li. (2025). &quot;cuThermo: Understanding GPU Memory Inefficiencies with Heat Map Profiling.&quot; <i>arXiv:2507.18729</i>.'
---

## Abstract

cuThermo is a novel GPU memory profiler that utilizes dynamic binary instrumentation (NVBit) to identify runtime inefficiencies from compiled binaries without source code modification. The tool pioneers a heat map visualization methodology based on a distinct warp count metric, enabling the precise detection of five critical performance bottlenecks.

## Key Contributions

- **Novel Profiling Tool**: Designed and developed cuThermo using dynamic binary instrumentation (NVBit) to analyze GPU memory behavior without requiring source code modifications.

- **Heat Map Visualization**: Pioneered a heat map visualization methodology based on a distinct warp count metric, enabling the precise detection of five critical performance bottlenecks including false sharing, memory misalignment, and shared memory abuse.

- **Real-World Impact**: Applied the tool to guide the optimization of seven applications, achieving performance speedups of up to 721.79% on NVIDIA RTX 4090 (Ada) and A4500 (Ampere) GPUs, demonstrating significant portability across architectures.

## Status

Preprint available on [arXiv:2507.18729](https://arxiv.org/abs/2507.18729). Currently under review.

