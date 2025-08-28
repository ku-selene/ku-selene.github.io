---
layout: pub_detail
title: "Learning Test-Mutant Relationship for Accurate Fault Localisation"
authors: "Jinhan Kim, Gabin An, Robert Feldt, Shin Yoo"
booktitle: "Information and Software Technology"
year: 2023
doi: "10.1016/J.INFSOF.2023.107272"
arxiv: "https://arxiv.org/abs/2306.02319"
---

# Abstract

**Context**:
Automated fault localisation aims to assist developers in the task of identifying the root cause of the fault by narrowing down the space of likely fault locations. Simulating variants of the faulty program called mutants, several Mutation Based Fault Localisation (MBFL) techniques have been proposed to automatically locate faults. Despite their success, existing MBFL techniques suffer from the cost of performing mutation analysis after the fault is observed.

**Method**:
To overcome this shortcoming, we propose a new MBFL technique named SIMFL (Statistical Inference for Mutation-based Fault Localisation). SIMFL localises faults based on the past results of mutation analysis that has been done on the earlier version in the project history, allowing developers to make predictions on the location of incoming faults in a just-in-time manner. Using several statistical inference methods, SIMFL models the relationship between test results of the mutants and their locations, and subsequently infers the location of the current faults.

**Results**:
The empirical study on Defects4J dataset shows that SIMFL can localise 113 faults on the first rank out of 224 faults, outperforming other MBFL techniques. Even when SIMFL is trained on the predicted kill matrix, SIMFL can still localise 95 faults on the first rank out of 194 faults. Moreover, removing redundant mutants significantly improves the localisation accuracy of SIMFL by the number of faults localised at the first rank up to 51.

**Conclusion**:
This paper proposes a new MBFL technique called SIMFL, which exploits ahead-of-time mutation analysis to localise current faults. SIMFL is not only cost-effective, as it does not need a mutation analysis after the fault is observed, but also capable of localising faults accurately.