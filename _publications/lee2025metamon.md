---
layout: pub_detail
title: "METAMON: Finding Inconsistencies between Program Documentation and Behavior using Metamorphic LLM Queries"
authors: "Hyeonseok Lee, Gabin An, Shin Yoo"
booktitle: "2th International Workshop on Large Language Models for Code (LLM4Code@ICSE'25)"
year: 2025
doi: "10.1109/LLM4Code66737.2025.00020"
arxiv: "https://arxiv.org/abs/2502.02794"
---

# Abstract

Code documentation can, if written precisely, help developers better understand the code they accompany. However, unlike code, code documentation cannot be automatically verified via execution, potentially leading to inconsistencies between documentation and the actual behavior. While such inconsistencies can be harmful for the developer’s understanding of the code, checking and finding them remains a costly task due to the involvement of human engineers. This paper proposes Metamon, which uses an existing search-based test generation technique to capture the current program behavior in the form of test cases, and subsequently uses LLM-based code reasoning to identify the generated regression test oracles that are not consistent with the program specifications in the documentation. Metamon is supported in this task by metamorphic testing and self-consistency. An empirical evaluation against 9,482 pairs of code documentation and code snippets, generated using five open-source projects from Defects4J v2.0.1, shows that Metamon can classify the code-and-documentation inconsistencies with a precision of 0.72 and a recall of 0.48.
