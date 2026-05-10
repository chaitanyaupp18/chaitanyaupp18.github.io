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
      <div class="card-text">
        <p>Analyses of heap-intensive applications show that a small fraction of heap objects account for the majority of heap accesses and data cache misses. Prior works like HDS and HALO have shown that allocating hot objects in separate memory regions can improve spatial locality leading to better application performance. However, these techniques are constrained in two primary ways, limiting their gains. First, these techniques have *Imperfect Separation*, polluting the hot memory region with several cold objects. Second, *reordering* of objects across allocations is not possible as the original object allocation order is preserved. This paper presents a novel technique that achieves near perfect separation of hot objects via a new context mechanism that efficiently identifies hot objects with high precision. This technique, named **PreFix**, is based upon **Pre**allocating memory for a **Fix**ed small number of hot objects. The program, guided by profiles, is instrumented to compute context information derived from dynamic object identifiers, that precisely identifies hot object allocations that are then placed at predetermined locations in the preallocated memory. The preallocated memory region for hot objects provides the flexibility to reorder objects across allocations and allows colocation of objects that are part of a hot data stream (HDS), improving spatial locality. The runtime overhead of identifying hot objects is not significant as this optimization is only focused on a small number of static hot allocation sites and dynamic hot objects. While there is an increase in the program's memory foot-print, it is manageable and can be controlled by limiting the size of the preallocated memory. In addition, **PreFix** incorporates an object recycling optimization that reuses the same preallocated space to store different objects whose lifetimes are not expected to overlap. Our experiments with **13** heap-intensive applications yield reductions in execution times ranging from **2.77%** to **74%**. On average **PreFix** reduces execution time by **21.7%** compared to **7.3%** by HDS and **14%** by HALO. This is due to **PreFix**'s precision in hot object identification, hot object colocation, and low runtime overhead.</p>
      </div>
    </div>
  </div>

  <div class="card mb-4">
    <div class="card-body">
      <h3 class="card-title">Binary Code Size Reduction</h3>
      <div class="card-text">
        <p>Binary sizes of upgraded versions of software applications tend to be larger, primarily due to feature bloat. This poses various challenges, particularly for mobile applications. It affects upgrade rates directly impacting revenues, increases maintenance costs of supporting multiple versions, and prevents some users from getting critical security fixes. Code bloat also poses a problem for large warehouse-scale applications. Such applications experience performance degradation when their code size exceeds what smaller and more efficient code models can handle.</p>
        <p>In this paper, we introduce a post-link optimization technique called *DeduBB*, which deduplicates basic blocks of an application across procedure boundaries. As the prior techniques used function outlining to deduplicate identical code sequences, they missed out on many opportunities such as duplicate code patterns that manipulate the program stack. In addition, previous techniques were either limited to the scope of a module or lacked scalable implementations required to handle large warehouse-scale applications. Our technique, *DeduBB*, exploits inter-module opportunities and de-duplicates more code patterns than prior techniques as it uses a novel *save-and-jump* code sequence to execute deduplicated code blocks. In addition, *DeduBB* has been designed to work on scalable post-link optimizers and can even be applied to large warehouse-scale data center applications. Finally, *DeduBB* is profile-guided and can be applied selectively to infrequently executed cold basic blocks to not affect application performance. In fact, in several cases, the performance of the smaller application binary improves slightly due to reductions in its hot working set size. We have designed our technique for the state-of-the-art post-link optimizers, BOLT and Propeller. Experiments show that we can significantly reduce the code size of several benchmarks by 1.55% to 18.63%, on both Arm and x86 platforms, even on binaries that have already been heavily optimized for size using existing code size reduction features. For warehouse-scale binaries, *DeduBB* reduces code size by up to 25.8%. Finally, aided by profiles, our technique can retain over 82% of the maximal code size savings without affecting performance.</p>
      </div>
    </div>
  </div>

</div>
