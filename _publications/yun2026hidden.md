---
layout: pub_detail
title: "The Hidden Costs of Evaluating Automated CI Repair at SAP HANA"
authors: "Sumi Yun, Jingun Hong, Somin Kim, Hyunjoon Cho, Gabin An and Shin Yoo"
booktitle: "19th IEEE International Conference on Software Testing, Verification and Validation (ICST'26)"
booktitle: "6th CI/CD Industry Workshop (CCIW@ICST'26)"
year: 2026
month: 2026-05
keywords: "Continuous Integration, Integration Testing, Automated Program Repair, Industrial Software, SAP HANA (C/C++)"
---

# Abstract

Test Case Prioritization (TCP) aims to find orderings of regression test suite execution so that failures can be detected as early as possible. Recently, Machine Learning (ML) based techniques have been proposed and evaluated using open-source projects and their test histories. We report our evaluation of these ML-based TCP techniques, both Reinforcement Learning (RL) and Supervised Learning (SL) based ones, using the industrial testing data collected from SAP HANA, a large-scale database management system. Specifically, our study compares 37 different TCP techniques, including 14 RL models on two datasets, 4 SL models, and 5 non-ML baselines, using real-world testing data of SAP HANA collected over eight months. Our evaluation focuses on both the performance and cost-efficiency of these techniques in the context of Continuous Integration for large-scale industrial projects. The results reveal that while RL models show promising performance, they require significant training time. RL models with sampled data offer a balance between performance and efficiency. Interestingly, the best-performing RL model outperformed or matched non-ML baselines. However, the gradient-boosted SL technique consistently outperformed both RL models and baselines in terms of effectiveness and efficiency, even with complete retraining at each test cycle. Despite RL's capability for incremental learning, it demands substantial training time and still falls short in accuracy compared to SL. Our findings suggest that, even in a large-scale industrial setting, fully retraining an SL model for each cycle proves to be the most effective and efficient approach for TCP, offering superior performance and cost-efficiency compared to RL and traditional methods.
