---
layout: pub_detail
title: "Disassembly-Augmented Root Cause Analysis for C/C++ Segmentation Faults in SAP HANA"
authors: "Jihoon Jung, Chansong You, Jingun Hong, Thomas Bach, Gabin An"
booktitle: "41st IEEE/ACM International Conference on Automated Software Engineering (ASE'26) - To appear 🇩🇪"
year: 2026
month: 2026-10
track: "Industry Showcase"
keywords: "Root Cause Analysis, Fault Localization, Crash Debugging, Segmentation Faults, Disassembly, Stack Traces, Large Language Models, Coding Agents, Industrial Software, SAP HANA (C/C++)"
---

# Abstract

Production failures in large-scale systems are inherently difficult to diagnose, and crash dumps are often the only artifact available for debugging. In C++ programs, this difficulty is further compounded by misleading crash locations in stack traces caused by compiler optimizations such as function inlining. In our dataset of production SIGSEGV crashes from SAP HANA, 66% exhibit such misleading crash locations, which can misdirect both developers and LLMbased debugging agents to the source code of inlined functions rather than the true execution context of the faulting instruction. In this work, we investigate whether explicitly providing disassembly information that reveals the faulting instruction and recovers inlining chains improves bug diagnosis quality in both autonomous agent and tool-disabled LLM modes. Experiments on 91 real-world SIGSEGV crashes show that disassembly context improves RCA quality and generally improves FL, especially for misleading crash locations. Moreover, in agent mode, the additional disassembly context does not increase total session cost of diagnosis, as its added input-token cost is offset by reduced exploration of the codebase.
