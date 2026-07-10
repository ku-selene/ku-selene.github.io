---
layout: pub_detail
title: "Is Three the Magic Number? An Empirical Evaluation of LLM-Based Repair Loops"
authors: "Tobias Kiecker, Eik Reichmann, Hosung Kang, Gabin An, Lars Grunske"
booktitle: "41st IEEE/ACM International Conference on Automated Software Engineering (ASE'26) - To appear 🇩🇪"
year: 2026
month: 2026-10
track: "NIER Track"
preprint: "https://arxiv.org/abs/2607.05197"
keywords: "LLM-based Repair Loops, Feedback-Driven Repair, Repair Iteration Limits"
---

# Abstract

Iterative repair loops have become a core design pattern in LLM-based software engineering systems. These workflows repeatedly generate, validate, and repair artifacts using feedback such as compiler errors or test failures. Despite their widespread use, the impact of repair-loop iteration limits remains poorly understood, as most prior work adopts fixed, often arbitrary, repair budgets. We study repair-loop effectiveness across multiple software engineering tasks, including code generation, test generation, and code translation. Across several representative workflows, datasets, and contemporary low-cost LLMs, we observe a consistent pattern of diminishing returns: the first three to four repair iterations account for most achievable gains, while later iterations contribute only marginal improvements. We further find that repair behavior is influenced more strongly by workflow orchestration and feedback design than by the underlying model itself. These results suggest that repair budgets should be treated as an explicit experimental variable, as they directly affect evaluation outcomes, computational cost, runtime, and reproducibility in LLM-based software engineering research.