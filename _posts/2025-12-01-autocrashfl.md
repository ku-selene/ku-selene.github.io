---
layout: post
title:  "Our AutoCrashFL (AutoFL Series) Paper Is Accepted to the ICSE'26 SEIP Track 🇧🇷"
date:   2025-12-01 09:00:00 +0900
categories: selene paper
tags: [Korea University, SELENE, Software Engineering]
---

Our industry collaboration with SAP Labs Korea, “**Finding the Needle in the Crash Stack: Industrial-Scale Crash Root Cause Localization with AutoCrashFL,”** has been accepted to ICSE-SEIP 2026 and will appear at the 48th ICSE in Rio 🇧🇷!

This work is an industry-oriented adaptation of our previous work, AutoFL [[link](https://dl.acm.org/doi/10.1145/3660771)][[preprint](https://arxiv.org/abs/2308.05487)], tailored specifically for **large-scale crash debugging**. 

To address the practical challenges of (1) missing coverage information, (2) extremely large crash dumps, and (3) the need for efficient navigation of industrial C/C++ codebases, AutoCrashFL performs crash-dump parsing to reduce noise and narrow the search space, and grants the LLM direct access to both the source code and the `clangd` Language Server for precise code exploration.

Our results show that AutoCrashFL significantly outperforms a crash-stack-only baseline across all crash types, highlighting its strong industrial applicability.

Check out more details at our preprint! 👉 [https://arxiv.org/abs/2510.22530](https://arxiv.org/abs/2510.22530)