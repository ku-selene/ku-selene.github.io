---
layout: pub_detail
title: "COSMosFL: Ensemble of Small Language Models for Fault Localisation"
authors: "Hyunjoon Cho, Sungmin Kang, Gabin An, Shin Yoo"
booktitle: "2th International Workshop on Large Language Models for Code (LLM4Code@ICSE'25)"
year: 2025
doi: "10.1109/LLM4Code66737.2025.00007"
arxiv: "https://arxiv.org/abs/2502.02908"
---

# Abstract

LLMs are rapidly being adopted to build powerful tools and agents for software engineering, but most of them rely heavily on extremely large closed-source models. This, in turn, can hinder wider adoption due to security issues as well as financial cost and environmental impact. Recently, a number of open source Small Language Models (SLMs) are being released and gaining traction. While SLMs are smaller, more energy-efficient, and therefore easier to locally deploy, they tend to show worse performance when compared to larger closed LLMs. We present COSMos, a task-level LLM ensemble technique that uses voting mechanism, to provide a broader range of choice between SLMs and LLMs. We instantiate COSMos with an LLM-based Fault Localisation technique, AutoFL, and report the cost-benefit trade-off between LLM accuracy and various costs such as energy consumption, inference time, and the number of tokens used. An empirical evaluation using Defects4J shows that COSMos can build effective ensembles that can achieve Pareto-optimality in terms of FL accuracy and inference cost, when compared to individual models.