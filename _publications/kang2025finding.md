---
layout: pub_detail
title: "Finding the Needle in the Crash Stack: Industrial-Scale Crash Root Cause Localization with AutoCrashFL"
authors: "Sungmin Kang, Sumi Yun, Jingun Hong, Shin Yoo, Gabin An"
booktitle: "Under Review 📝"
year: 2025 
month: 2025-10
preprint: "https://arxiv.org/abs/2510.22530"
keywords: "Fault Localization, Crash Debugging, Large Language Models, Industrial Software, Root Cause Analysis, SAP HANA (C/C++)"
---

# Abstract

Fault Localization (FL) aims to identify root causes of program failures. FL typically targets failures observed from test executions, and as such, often involves dynamic analyses to improve accuracy, such as coverage profiling or mutation testing. However, for large industrial software, measuring coverage for every execution is prohibitively expensive, making the use of such techniques difficult. To address these issues and apply FL in an industrial setting, this paper proposes AutoCrashFL, an LLM agent for the localization of crashes that only requires the crashdump from the Program Under Test (PUT) and access to the repository of the corresponding source code. We evaluate AutoCrashFL against real-world crashes of SAP HANA, an industrial software project consisting of more than 35 million lines of code. Experiments reveal that AutoCrashFL is more effective in localization, as it identified 30% crashes at the top, compared to 17% achieved by the baseline. Through thorough analysis, we find that AutoCrashFL has attractive practical properties: it is relatively more effective for complex bugs, and it can indicate confidence in its results. Overall, these results show the practicality of LLM agent deployment on an industrial scale.
