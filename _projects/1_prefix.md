---
layout: page
title: PreFix
description: Optimizing the Performance of Heap-Intensive Applications.
img: assets/img/publication_preview/prefix.png
importance: 1
category: work
---

**PreFix** is a performance optimization technique designed to improve the spatial locality of heap-intensive applications. It focuses on identifying a small number of "hot" heap objects—which frequently contribute to data cache misses—and segregating them into dedicated, preallocated memory regions.

### Key Features
- **Precision Identification**: Uses a novel context mechanism to identify hot object allocation sites and dynamic hot objects with high precision.
- **Preallocation**: Redirects hot object allocations to predetermined locations within a preallocated memory region.
- **Object Recycling**: Reuses preallocated space for different objects whose lifetimes do not overlap.

[Read the paper on ACM Digital Library](https://dl.acm.org/doi/epdf/10.1145/3696443.3708960)
