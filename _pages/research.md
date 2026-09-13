---
layout: page
title: Research
permalink: /research/
description: A summary of my research projects.
nav: true
nav_order: 3
---

<div class="research-projects">

  <div class="card mb-4">
    <div class="card-body">
      <h3 class="card-title">Performance Optimization for Heap-Intensive Applications</h3>
      <div class="row">
        <div class="col-sm-12 mt-3 mt-md-0 mb-3">
          {% include figure.liquid loading="eager" path="assets/img/publication_preview/prefix.png" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-12">
          <p>A small fraction of heap objects often accounts for most memory accesses and data cache misses. PreFix improves data locality by identifying these hot objects precisely and placing them together in a preallocated memory region. Profile-guided instrumentation uses allocation context derived from dynamic object identifiers to select predetermined locations, allowing objects to be reordered across allocations according to their access patterns. PreFix also reuses preallocated space for objects whose lifetimes are not expected to overlap. Across 13 heap-intensive applications, it reduces execution time by 21.7% on average, compared with 7.3% for HDS and 14% for HALO.</p>
          <p>PreFix identifies hot objects and places them together in a profile-guided order.</p>
          <p><a href="https://dl.acm.org/doi/10.1145/3696443.3708960" target="_blank">Paper</a> · <a href="https://research.google/pubs/prefix-optimizing-the-performance-of-heap-intensive-applications/" target="_blank">Abstract</a></p>
        </div>
      </div>
    </div>
  </div>

  <div class="card mb-4">
    <div class="card-body">
      <h3 class="card-title">Binary Code Size Reduction</h3>
      <div class="row">
        <div class="col-sm-12 mt-3 mt-md-0 mb-3">
          {% include figure.liquid loading="eager" path="assets/img/publication_preview/dedubb.png" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-12">
          <p>DeduBB reduces binary code size by sharing repeated basic blocks across functions and modules after linking. Its save-and-jump mechanism supports code patterns, including stack-manipulating instructions, that conventional function outlining cannot readily handle. Implemented in BOLT and Propeller, DeduBB scales to large applications and uses execution profiles to focus deduplication on cold blocks, limiting performance overhead. Experiments on Arm and x86 show code size reductions of 1.55% to 18.63% on benchmarks already optimized for size. Profile-guided selection retains more than 80% of the maximum savings without affecting performance in the reported experiments.</p>
          <p>Repeated code becomes one shared copy; each execution resumes at its original continuation.</p>
          <p><a href="https://dl.acm.org/doi/10.1145/3814943.3816169" target="_blank">Paper</a> · <a href="https://research.google/pubs/dedubb-binary-code-size-reduction-via-post-link-basic-block-de-duplication/" target="_blank">Abstract</a></p>
        </div>
      </div>
    </div>
  </div>

  <div class="card mb-4">
    <div class="card-body">
      <h3 class="card-title">AI-Guided Interprocedural Code Layout Optimization</h3>
      <div class="row">
        <div class="col-sm-12 mt-3 mt-md-0 mb-3">
          {% include figure.liquid loading="eager" path="assets/img/publication_preview/ai-propeller.png" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm-12">
          <p>Frequently executed code can remain scattered across functions even after conventional code layout optimization. AI-Propeller improves instruction locality by placing frequently connected basic blocks from different functions close together. Built on Propeller, it uses the Magellan framework to combine AlphaEvolve's evolution of layout heuristics with Vizier's tuning of their numerical parameters. Candidate layouts are evaluated on real hardware, and measured performance guides the search. This enables fine-grained interprocedural layouts while preserving call-return semantics and build scalability. AI-Propeller improves performance by 1.6% on LLVM Clang and 0.23% on a warehouse-scale Search workload over Ext-TSP, extracting additional gains from binaries already optimized with feedback-directed optimization and ThinLTO.</p>
          <p><a href="https://arxiv.org/abs/2606.00131" target="_blank">arXiv</a> · <a href="https://research.google/pubs/ai-propeller-warehouse-scale-inter-procedural-code-layout-optimization-with-alphaevolve/" target="_blank">Abstract</a></p>
        </div>
      </div>
    </div>
  </div>

</div>
