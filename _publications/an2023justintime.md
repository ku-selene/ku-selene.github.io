---
layout: pub_detail
title: "Just-in-Time Flaky Test Detection via Abstracted Failure Symptom Matching"
authors: "Gabin An, Juyeon Yoon, Thomas Bach, Jingun Hong, Shin Yoo"
booktitle: "40th International Conference on Software Maintenance and Evolution (ICSME'24)"
year: 2024
track: "Industry Track"
doi: "10.1109/ICSME58944.2024.00078"
award: "Best Industry Paper Award"
arxiv: "https://arxiv.org/abs/2310.06298"
---

# Abstract

We report our experience of using failure symptoms, such as error messages or stack traces, to identify flaky test failures in a Continuous Integration (CI) pipeline for a large industrial software system, SAP HANA. Although failure symptoms are commonly used to identify similar failures, they have not previously been employed to detect flaky test failures. Our hypothesis is that flaky failures will exhibit symptoms distinct from those of non-flaky failures. Consequently, we can identify recurring flaky failures, without rerunning the tests, by matching the failure symptoms to those of historical flaky runs. This can significantly reduce the need for test reruns, ultimately resulting in faster delivery of test results to developers. To facilitate the process of matching flaky failures across different execution instances, we abstract newer test failure symptoms before matching them to the known patterns of flaky failures, inspired by previous research in the fields of failure deduplication and log analysis. We evaluate our symptom-based flakiness detection method using actual failure symptoms gathered from CI data of SAP HANA during a six-month period. Our method shows the potential of using failure symptoms to identify recurring flaky failures, achieving a precision of at least 96%, while saving approximately 58% of the machine time compared to the traditional rerun strategy. Analysis of the false positives and the feedback from developers underscore the importance of having descriptive and informative failure symptoms for both the effective deployment of this symptom-based approach and the debugging of flaky tests.