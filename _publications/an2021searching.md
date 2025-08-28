---
layout: pub_detail
title: "Searching for Multi-Fault Programs in Defects4J"
authors: "Gabin An, Juyeon Yoon, Shin Yoo"
booktitle: "13th International Symposium on Search Based Software Engineering (SSBSE'21)"
year: 2021
track: "Challenge Track"
doi: "10.1007/978-3-030-88106-1_11"
arxiv: "https://arxiv.org/abs/2108.04455"
---

# Abtract

Defects4J has enabled numerous software testing and debugging research work since its introduction. A large part of its contribution, and the resulting popularity, lies in the clear separation and distillation of the root cause of each individual test failure based on careful manual analysis, which in turn allowed researchers to easily study individual faults in isolation. However, in a realistic debugging scenario, multiple faults can coexist and affect test results collectively. Study of automated debugging techniques for these situations, such as failure clustering or fault localisation for multiple faults, would significantly benefit from a reliable benchmark of multiple, coexisting faults. We search for versions of Defects4J subjects that contain multiple faults, by iteratively transplanting fault-revealing test cases across Defects4J versions. Out of 326 studied versions of Defects4J subjects, we report that over 95% (311 versions) actually contain from two to 24 faults. We hope that the extended, multi-fault Defects4J can provide a platform for future research of testing and debugging techniques for multi-fault programs.