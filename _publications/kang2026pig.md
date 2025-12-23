---
layout: pub_detail
title: "Pig: Leveraging Large Language Models for Python Library Migrations"
authors: "Miryeong Kang, Wonseok Oh, Gabin An, Hakjoo Oh"
booktitle: "ACM International Conference on the Foundations of Software Engineering (FSE'26) - To appear 🇨🇦"
year: 2026
month: 2026-07
track: "Research Track"
keywords: "Library Migration, Python, Large Language Models, Code Transformation"
---

# Abstract

We present Pig, a novel approach to automating Python library migration by leveraging large language models (LLMs). Library migration is an increasingly common task in modern Python development, yet it remains tedious and error-prone due to the lack of general solutions that can handle diverse libraries without relying on documentation or code examples. To address this challenge, Pig employs a four-step pipeline that effectively harnesses the capabilities of LLMs. First, Pig decomposes the migration task into smaller units by performing API-level slicing, allowing the LLM to focus on minimal, relevant context. Second, it guides LLMs using prompts informed by common failure patterns in naive LLM-based migrations and plausible API candidates. Third, Pig selectively extracts the migration-related code fragments from the LLM outputs. Finally, it transplants the migrated code back into the original program with post-processing to ensure semantic correctness and consistency. We demonstrate the effectiveness of Pig by evaluating it on 364 API-level migration tasks, where it improves the average success rate of the baseline approach by 53.5% across seven different LLM models.
