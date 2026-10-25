---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

[Download PDF Version](/files/Yanbo_Zhao_CV_2026.pdf)

Education
======
* **Ph.D. in Computer Science** (Ph.D. Candidate), North Carolina State University, Sept 2022 - Present (Expected: May 2027)
  * Advisors: [Dr. Jiajia Li](https://fruitfly1026.github.io/) and [Dr. Xu Liu](https://xl10.github.io/)
  * Focus: GPU Performance Analysis, Profiling, and Optimization

* **M.S. in Software Engineering**, Shandong University, Sept 2019 - Jun 2022
  * Advisor: [Dr. Lei Ju](https://ieeexplore.ieee.org/author/37544824100)

* **B.S. in Software Engineering**, Shandong University, Sept 2015 - Jun 2019

Work Experience
======
* **May 2026 - Aug 2026: Student Researcher**
  * Google, Durham, NC
  * Project: TypeCraft++ - fast, zero-shot type annotation for C++ binaries
  * Mentors: Dr. Xu Liu and Namhyung Kim

* **Jun 2025 - Aug 2025: Research Intern**
  * Pacific Northwest National Laboratory (PNNL), Richland, WA
  * Project: Leveraging the AI ecosystem (Triton) for portable and sustainable GPU kernels in HPC
  * Mentor: [Dr. Ajay Panyala](https://www.pnnl.gov/people/ajay-panyala)

* **Aug 2022 - Present: Teaching/Research Assistant**
  * North Carolina State University, Raleigh, NC
  * Teaching Assistant for CSC246 (Operating Systems), Fall 2022 - Spring 2024
  * Research Assistant supervised by Dr. Jiajia Li and Dr. Xu Liu

Research Experience
======
* **cuVein: Understanding In-kernel Data Flow with Cross Grained Memory Centric Topology Distance Analysis** (Under Review) @ NCSU, Jun 2025 - Present
  * Proposed Topology Distance, a metric linking a program's logical data flow to the physical communication costs of the underlying GPU hardware.
  * Root-caused previously hidden performance bottlenecks in complex HPC kernels, providing guidance not surfaced by official profilers.
  * Enabled full-volume shadow memory analysis without sampling via a lock-free parallel analyzer and a contention-free shared-memory analyzer, keeping end-to-end overhead under 10×.

* **TypeCraft++: Fast, Zero-Shot Type Annotation for C++ Binaries** (Ongoing) @ Google, May 2026 - Present
  * Designed a single-pass register type coloring algorithm that builds a PC-indexed register type table and propagates types from DWARF-known PCs, achieving over 60% coverage on SPEC CPU2017 with only partial DWARF.
  * Replaced the prior per-instruction forward-propagation approach, cutting annotation overhead by 5× for PCs collected via live Linux perf sampling.

* **Leveraging AI Ecosystem for Portable and Sustainable GPU Kernels** (ARRAY 2026) @ PNNL, Jun 2025 - Aug 2025
  * Developed an AOT compilation framework that integrates Triton with C/C++ HPC codebases, auto-generating optimized GPU code and a C++ wrapper into standalone shared libraries with the performance of hand-tuned CUDA.

* **RedSan: Redundant Memory Instruction Sanitizer for GPU Programs** (SC 2025) @ NCSU, Dec 2024 - May 2025
  * A dynamic binary instrumentation tool that detects and quantifies redundant memory instructions in GPU applications without source code.
  * Guided optimizations achieving up to 6.27× speedup and 3.00× fewer memory operations across HPC and AI benchmarks.
  * Uncovered a previously undocumented compiler correctness issue with CUDA's `__restrict__` keyword and optimization opportunities in NVIDIA's cuSPARSE and cuSOLVER libraries.

* **cuThermo: Understanding GPU Memory Inefficiencies with Heat Map Profiling** (Under Review) @ NCSU, Feb 2025 - Apr 2025
  * Developed a GPU memory profiler using dynamic binary instrumentation (NVBit) to identify runtime inefficiencies from compiled binaries.
  * Designed a heat map visualization based on a warp count metric, detecting five bottlenecks such as false sharing, memory misalignment, and shared memory abuse.
  * Guided optimization of seven applications, achieving speedups of up to 721.79% on NVIDIA RTX 4090 (Ada) and A4500 (Ampere) GPUs.

* **Memogent: Exploring Reuse Distance Patterns in GPU Accelerated Applications** @ NCSU, Jan 2023 - Jan 2024
  * Captured every GPU-kernel memory access using independent analysis kernels, identifying four reuse-distance inefficiency patterns; optimized 6 Rodinia/LULESH cases, cutting load memory traffic by 16.13% on average.

* **A Profiling Tool for Cache Persisting in NVIDIA GPUs** @ SDU, Jan 2021 - Jul 2022
  * Built an Ampere L2 persistence-cache tool that uses reuse-distance and memory-utilization analysis to suggest data to lock into L2, improving L2 hit rate and execution time.

* **Low Power Object Detection Challenge (DAC-SDC 2018)** @ SDU, Dec 2017 - May 2018
  * Optimized a darknet YOLOv2 detector for NVIDIA Jetson TX2 via multi-threaded pre-processing, pruning, and quantization, reaching 68.4% IoU at 23.64 FPS — 3rd place worldwide in the GPU category.

Skills & Expertise
======
* **Programming Languages**: C/C++, Python, Shell
* **Parallel & Architecture**: CUDA (PTX, SASS), OpenMP, Triton, ROCm, GPU Architecture
* **Profiling Tools**: Nsight Compute/System, NVBit, CUPTI, Compute Sanitizer API, HPCToolkit
* **Systems & Performance**: GPU/CPU co-scheduling, Memory redundancy detection

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service
======
* **SC 26** (Int'l Conf. for High Performance Computing, Networking, Storage, and Analysis): Program Committee, Student Volunteer
* **ICS 27** (Int'l Conf. on Supercomputing): Program Committee
* **ISC 26** (ISC High Performance): Program Committee
* **IEEE BigData 26** (IEEE Int'l Conf. on Big Data): Program Committee
* **SPAA 25** (Symp. on Parallelism in Algorithms and Architectures): Junior Program Committee
* **PPoPP 25** (Symp. on Principles and Practice of Parallel Programming): Artifact Evaluation Committee

Honors & Awards
======
* 2025 NCSU GSA Conference Travel Awards
* 2018 World third prize of DAC-SDC: Lower Power Object Detection Challenge
* 2016 Provincial third prize of China Undergraduate Mathematical Contest in Modeling
