---
layout: pub_detail
title: "Automatically Identifying Shared Root Causes of Test Breakages in SAP HANA"
authors: "Gabin An*, Juyeon Yoon*, Jeongju Sohn, Jingun Hong, Dongwon Hwang, Shin Yoo"
booktitle: "44th IEEE/ACM International Conference on Software Engineering (ICSE'22)"
year: 2022
track: "SEIP Track"
doi: "10.1145/3510457.3513051"
---

# Abstract

Continuous Integration (CI) of a large-scale software system such as SAP HANA can produce a non-trivial number of test breakages. Each breakage that newly occurs from daily runs needs to be manually inspected, triaged, and eventually assigned to developers for debugging. However, not all new breakages are unique, as some test breakages would share the same root cause; in addition, human errors can produce duplicate bug tickets for the same root cause. An automated identification of breakages with shared root causes will be able to significantly reduce the cost of the (typically manual) post-breakage steps. This paper investigates multiple similarity functions between test breakages to assist and automate the identification of test breakages that are caused by the same root cause. We consider multiple information sources, such as static (i.e., the code itself), historical (i.e., whether the test results have changed in a similar way in the past), as well as dynamic (i.e., whether the coverage of test cases are similar to each other), for the purpose of such automation. We evaluate a total of 27 individual similarity functions, using real-world CI data of SAP HANA from a six-month period. Further, using these individual similarity functions as input features, we construct a classification model that can predict whether two test breakages share the same root cause or not. When trained using ground truth labels extracted from the issue tracker of SAP HANA, our model achieves an F1 score of 0.743 when evaluated using a set of unseen test breakages collected over three months. Our results show that a classification model based on test similarity functions can successfully support the bug triage stage of a CI pipeline.