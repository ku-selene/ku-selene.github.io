---
layout: pub_detail
title: "Comparing Line and AST Granularity Level for Program Repair using PyGGI"
authors: "Gabin An, Jinhan Kim, Shin Yoo"
booktitle: "4th Genetic Improvement Workshop (GI@ICSE'18)"
year: 2018
doi: "10.1145/3194810.3194814"
---

# Abstract

PyGGI is a lightweight Python framework that can be used to implement generic Genetic Improvement algorithms at the API level. The original version of PyGGI only provided lexical modifications, i.e., modifications of the source code at the physical line granularity level. This paper introduces new extensions to PyGGI that enables syntactic modifications for Python code, i.e., modifications that operates at the AST granularity level. Taking advantage of the new extensions, we also present a case study that compares the lexical and syntactic search granularity level for automated program repair, using ten seeded faults in a real world open source Python project. The results show that search landscapes at the AST granularity level are more effective (i.e. eventually more likely to produce plausible patches) due to the smaller sizes of ingredient spaces (i.e., the space from which we search for the material to build a patch), but may require longer time for search because the larger number of syntactically intact candidates leads to more fitness evaluations.