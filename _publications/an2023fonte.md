---
layout: pub_detail
title: "Fonte: Finding Bug Inducing Commits from Failures"
authors: "Gabin An, Jingun Hong, Naryeong Kim, Shin Yoo"
booktitle: "45th IEEE/ACM International Conference on Software Engineering (ICSE'23)"
year: 2023
month: 2023-05
track: "Technical Track"
doi: "10.1109/ICSE48619.2023.00059"
preprint: "https://arxiv.org/abs/2212.06376"
keywords: "Bug Inducing Commit, Fault Localization, Git, Commit History, Weighted Bisection, Batch Testing, Industrial Software, Defects4J (Java), SAP HANA (C/C++)"
---

# Abstract

A Bug Inducing Commit (BIC) is a commit that introduces a software bug into the codebase. Knowing the relevant BIC for a given bug can provide valuable information for debugging as well as bug triaging. However, existing BIC identification techniques are either too expensive (because they require the failing tests to be executed against previous versions for bisection) or inapplicable at the debugging time (because they require post hoc artefacts such as bug reports or bug fixes). We propose Fonte, an efficient and accurate BIC identification technique that only requires test coverage. Fonte combines Fault Localisation (FL) with BIC identification and ranks commits based on the suspiciousness of the code elements that they modified. Fonte reduces the search space of BICs using failure coverage as well as a filter that detects commits that are merely style changes. Our empirical evaluation using 130 real-world BICs shows that Fonte significantly outperforms state-of-the-art BIC identification techniques based on Information Retrieval as well as neural code embedding models, achieving at least 39% higher MRR. We also report that the ranking scores produced by Fonte can be used to perform weighted bisection, further reducing the cost of BIC identification. Finally, we apply Fonte to a large-scale industry project with over 10M lines of code, and show that it can rank the actual BIC within the top five commits for 87% of the studied real batch-testing failures, and save the BIC inspection cost by 32% on average.

# Extension

The extended version of this paper is available at: [https://arxiv.org/abs/2502.12922](https://arxiv.org/abs/2502.12922)