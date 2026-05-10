---
layout: page
title: DeduBB
description: Binary Code Size Reduction via Post-Link Basic Block De-duplication.
img: assets/img/publication_preview/dedubb.jpg
importance: 2
category: work
---

**DeduBB** is a post-link optimization technique that de-duplicates basic blocks of an application across procedure boundaries to reduce binary size.

### Key Features
- **Inter-Module Optimization**: Exploits inter-module opportunities and de-duplicates more code patterns than prior techniques.
- **Save-and-Jump Mechanism**: Uses a novel `save-and-jump` code sequence to execute de-duplicated code blocks, enabling outlining of stack-manipulating code.
- **Scalable**: Designed to work on state-of-the-art post-link optimizers like BOLT and Propeller, scaling to large warehouse-scale applications.
- **Profile-Guided**: Applied selectively to infrequently executed cold basic blocks to avoid affecting performance.
