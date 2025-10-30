---
layout: pub_detail
title: "BUGSC++: A Highly Usable Real World Defect Benchmark for C/C++"
authors: "Gabin An, Minhyuk Kwon, Kyunghwa Choi, Jooyong Yi, Shin Yoo"
booktitle: "38th IEEE/ACM International Conference on Automated Software Engineering (ASE'23)"
year: 2023
month: 2023-09
track: "Tool Demos"
doi: "10.1109/ASE56229.2023.00208"
keywords: "Software Testing, Defect Benchmark, C/C++"
---

# Abstract

As software systems grow larger and more complex, debugging takes up an increasingly significant portion of developers' time and efforts during software maintenance. To aid software engineers in debugging, many automated debugging and repair techniques have been proposed. Both the development and evaluation of these automated techniques depend on benchmarks of bugs. While many different defect benchmarks have been developed, only a few benchmarks are widely used due to the origin of the collected bugs as well as the usability of the benchmarks themselves, risking a biased research landscape. This paper presents BUGSC++, a new benchmark that contains 209 real-world bugs collected from 22 open-source C/C++ projects. BugsC++ aims to provide high usability by providing a similar user interface to the widely used Defects4J. Further, BugsC++ ensures the replicability of the bugs in its collection by encapsulating each buggy program in a Docker container. By providing a highly usable real-world defect benchmark for C/C++, we hope to promote debugging research for C/C++.