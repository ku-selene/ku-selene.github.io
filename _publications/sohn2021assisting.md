---
layout: pub_detail
title: "Assisting Bug Report Assignment Using Automated Fault Localisation: An Industrial Case Study"
authors: "Jeongju Sohn*, Gabin An*, Jingun Hong, Dongwon Hwang, Shin Yoo"
booktitle: "14th IEEE International Conference on Software Testing, Verification and Validation (ICST'21)"
year: 2021
month: 2021-04
track: "Industry Track"
doi: "10.1109/ICST49551.2021.00041"
keywords: "Fault Localization, Spectrum-based Fault Localization, Test Suite Diagnosability, Voting, Industrial Software, SAP HANA (C/C++)"
---

# Abstract

We present a case study of an industry scale application of automated fault localisation to SAP HANA2 database. When a test breaks in the Continuous Integration (CI) pipeline, the bug needs to be triaged and assigned to the appropriate development team. Given the scale and complexity of SAP HANA2, the assignment itself can be a challenging task. The current practice depends on the static mapping between test scripts and software components, as well as human domain knowledge. We apply automated fault localisation to aid the issue allocation in the CI pipeline: once a test failure is observed, the automated fault localisation technique identifies the suspicious software component using the information from the test failure. The localisation result can be used by the issue manager to allocate the incoming test failure issues more efficiently. We have analysed 137 CI test executions with at least one failing test script using Spectrum Based Fault Localisation. The results show that automated fault localisation can identify the faulty software component for 61 out of 137 studied test failures within top 10 places out of over 200 components. Out of the 61 faults, 36 faults were not identifiable based on the static mapping between test script and software components at all.
