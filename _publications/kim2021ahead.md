---
layout: pub_detail
title: "Ahead of Time Mutation Based Fault Localisation using Statistical Inference"
authors: "Jinhan Kim, Gabin An, Robert Feldt, Shin Yoo"
booktitle: "32nd International Symposium on Software Reliability Engineering (ISSRE'21)"
year: 2021
track: "Research Track"
doi: "10.1109/ISSRE52982.2021.00036"
---

# Abstract

Mutation analysis can effectively capture the de-pendency between source code and test results. This has been exploited by Mutation Based Fault Localisation (MBFL) techniques. However, MBFL techniques suffer from the need to expend the high cost of mutation analysis after the observation of failures, which may present a challenge for its practical adoption. We introduce SIMFL (Statistical Inference for Mutation-based Fault Localisation), an MBFL technique that allows users to perform the mutation analysis in advance before a failure is observed, allowing the amortisation of the analysis cost. SIMFL uses mutants as artificial faults and aims to learn the failure patterns among test cases against different locations of mutations. Once a failure is observed, SIMFL requires either almost no or very small additional cost for analysis, depending on the used inference model. An empirical evaluation using DEFECTS4J shows that SIMFL can successfully localise up to 113 out of 203 studied faults (55%) at the top, and 159 (78%) faults within the top five, significantly outperforming existing MBFL techniques while using the results of mutation analysis that has been undertaken before the test failure. The amortised cost of mutation analysis can be further reduced by mutation sampling: SIMFL retains 80 % of its localisation accuracy at the top rank when using only 10% of generated mutants, compared to results obtained without sampling.
