---
layout: pub_detail
title: "Reducing the Search Space of Bug Inducing Commits using Failure Coverage"
authors: "Gabin An, Shin Yoo"
booktitle: "29th ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE'21)"
year: 2021
month: 2021-08
track: "Ideas, Visions, and Reflections Track"
doi: "10.1145/3468264.3473129"
keywords: "Bug Inducing Commit, Test Coverage, Commit History, Defects4J (Java)"
---

# Abstract

Knowing how exactly a bug has been introduced into the code can help developers debug the bug efficiently. However, techniques currently used to retrieve Bug Inducing Commits (BICs) from the repository timeline are limited in their accuracy. Automated bisection of the version history depends on the bug revealing test case being executable against all candidate previous versions, whereas blaming the last commits that touched the same parts as the fixing commit (à la SZZ) requires that the bug has already been fixed. We show that filtering commits using the coverage of the bug revealing test cases can effectively reduce the search space for both bisection and SZZ-like blame models by 87.6% and 27.9%, respectively, significantly reducing the cost of BIC retrieval. The application of our approach to bugs in Defects4J also reveals inconsistencies in some of their BICs known in the literature.