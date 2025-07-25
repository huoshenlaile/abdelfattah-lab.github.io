---
title: 'Learning from Students: Applying t-Distributions to Explore Accurate and Efficient Formats for LLMs'
authors:
  - key: jordan
  - key: yuzong
  - key: bahaa
  - key: sushma
  - key: gang
  - key: sheng
  - key: mohamed
  - key: zhiru
venue: icml
year: 2024
date: 2024-08-01
teaser: ''
tags:
  - dnn compression
  - llm
  - quantization
materials:
  - name: PDF
    url: https://arxiv.org/pdf/2405.03103
    type: file-pdf
---
The increasing size of large language models (LLMs) traditionally requires low-precision integer formats to meet strict latency and power demands. Yet recently, alternative formats such as Normal Float (NF4) have increased model accuracy at the cost of increased chip area. In this work, we first conduct a large-scale analysis of LLM weights and activations across 30 networks and conclude that most distributions follow a Student's t-distribution. We then derive a new theoretically optimal format, Student Float (SF4), that improves over NF4 across modern LLMs, for example increasing the average accuracy on LLaMA2-7B by 0.76% across tasks. Using this format as a high-accuracy reference, we then propose augmenting E2M1 with two variants of supernormal support for higher model accuracy. Finally, we explore the quality and efficiency frontier across 11 datatypes by evaluating their model accuracy and hardware complexity. We discover a Pareto curve composed of INT4, E2M1, and E2M1 with supernormal support, which offers a continuous tradeoff between model accuracy and chip area. For example, E2M1 with supernormal support increases the accuracy of Phi-2 by up to 2.19% with 1.22% area overhead, enabling more LLM-based applications to be run at four bits. The supporting code is hosted at https://github.com/cornell-zhang/llm-datatypes.
