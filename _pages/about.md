---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a 5th-year Ph.D. student in Computer Science at North Carolina State University, advised by [Dr. Jiajia Li](https://fruitfly1026.github.io/) and [Dr. Xu Liu](https://xl10.github.io/), and expect to graduate in May 2027. My research focuses on GPU performance analysis, profiling, and optimization: I build binary-level tools that expose hidden memory inefficiencies in GPU programs and turn them into concrete optimizations.

Before NC State, I received my M.S. (advised by Dr. Lei Ju) and B.S. in Software Engineering from Shandong University.

## News

- **2026.05**: Joined **Google** as a Student Researcher (Durham, NC), working on fast, zero-shot type annotation for C++ binaries.
- **2026**: *TIDES* (tiered block-sparse tensor contraction on GPUs) accepted to **SC 2026** (to appear).
- **2026.06**: *[SparseZETA](https://pldi26.sigplan.org/details/pldi-2026-papers/70/SparseZETA-Intelligent-Auto-tuner-for-Designing-High-Performance-SpMV-Programs)* (SpMV auto-tuner) presented at **PLDI 2026**.
- **2026.06**: Presented our PNNL internship work, *[Leveraging AI Ecosystem for Portable and Sustainable GPU Kernels in HPC](https://pldi26.sigplan.org/details/ARRAY-2026-papers/3/Leveraging-AI-Ecosystem-for-Portable-and-Sustainable-GPU-Kernels-in-HPC)*, at **ARRAY 2026** (co-located with PLDI).
- **2026**: Serving on the Program Committees of **SC 26**, **ICS 27**, **ISC 26**, and **IEEE BigData 26**.
- **2025.11**: *[RedSan: A Redundant Memory Instruction Sanitizer for GPU Programs](https://dl.acm.org/doi/10.1145/3712285.3759830)* presented at **SC 2025**.
- **2025.06**: Research intern at **Pacific Northwest National Laboratory (PNNL)**.

## Research Interests

My research lies at the intersection of high-performance computing, GPU architecture, and system performance optimization:

- **GPU Performance Analysis & Profiling**: Dynamic binary instrumentation tools (NVBit, Compute Sanitizer) that find bottlenecks in GPU binaries without source code
- **Memory System Optimization**: Detecting redundant memory operations, analyzing reuse distance and in-kernel data flow, and improving memory access patterns
- **Compilation & Code Generation**: Bridging AI ecosystems (Triton) and traditional HPC codebases for portable, sustainable GPU kernels
- **Binary Analysis**: Type recovery for optimized binaries to support production-scale profiling

## Selected Projects

- **cuVein** *(under review)*: Introduces *Topology Distance*, a metric linking a program's logical data flow to the physical communication cost of GPU hardware. A lock-free parallel analyzer enables full-volume shadow memory analysis with under 10× end-to-end overhead.
- **[RedSan](https://dl.acm.org/doi/10.1145/3712285.3759830)** *(SC 2025)*: A sanitizer that detects and quantifies redundant memory instructions in GPU binaries, guiding up to **6.27×** speedups and uncovering a compiler correctness issue with CUDA's `__restrict__`.
- **[cuThermo](https://arxiv.org/abs/2507.18729)** *(arXiv)*: A heat-map GPU memory profiler built on a warp-count metric that detects five classes of memory inefficiency, guiding up to **721.79%** speedups.
- **TypeCraft++** *(Google, ongoing)*: A single-pass register type coloring algorithm for C++ binaries with partial DWARF, reaching over 60% coverage on SPEC CPU2017 with 5× lower annotation overhead.

## Technical Skills

**Programming**: C/C++, Python, Shell

**Parallel Computing & Architecture**: CUDA (PTX, SASS), OpenMP, Triton, ROCm, GPU Architecture

**Profiling & Analysis Tools**: Nsight Compute/System, NVBit, CUPTI, Compute Sanitizer API, HPCToolkit

**Systems & Performance**: GPU/CPU co-scheduling, Memory redundancy detection
