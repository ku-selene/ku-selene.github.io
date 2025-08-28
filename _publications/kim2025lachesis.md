---
layout: pub_detail
title: "Lachesis: Predicting LLM Inference Accuracy using Structural Properties of Reasoning Paths"
authors: "Naryeong Kim, Sungmin Kang, Gabin An, Shin Yoo"
booktitle: "6th International Workshop on Deep Learning for Testing and Testing for Deep Learning (DeepTest@ICSE'25)"
year: 2025
doi: "10.1109/DEEPTEST66595.2025.00008"
arxiv: "https://arxiv.org/abs/2412.08281"
---

# Abstract

Large Language Models are increasingly used to build agents to perform more complex tasks. As LLMs perform more complicated reasoning through longer interactions, self-consistency, i.e., the idea that the answer obtained from sampling and marginalising a number of multiple independent inferences is more likely to be correct, has been received much attention as a simple validation technique. This paper aims to empirically verify this intuitive hypothesis by predicting the correctness of answers obtained using self-consistency from properties of the samples of reasoning paths. We introduce Lachesis, a predictive model for self-consistency based LLM inferences, and empirically evaluate it using AutoFL, a recently proposed LLM-based fault localisation technique, as the target technique that uses self-consistency. Lachesis converts collected reasoning paths from AutoFL using specifically designed reasoning path representations, and trains LSTM and GCN models to predict whether a given set of reasoning paths would result in a correct answer. The results suggest that Lachesis can predict the correctness of answers with a precision of up to 0.8136, highlighting the possibility of training a predictive model that can allow early termination of inferences that are not likely to be successful.
