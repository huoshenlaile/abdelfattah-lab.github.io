---
title: 'Encodings for Prediction-based Neural Architecture Search'
authors:
  - key: yash
  - key: mohamed
venue: icml
year: 2024
date: 2024-08-01
teaser: ''
tags:
  - automl
materials:
  - name: PDF
    url: https://arxiv.org/pdf/2403.02484
    type: file-pdf
  - name: Code
    url: https://github.com/abdelfattah-lab/flan_nas
    type: code
---
Predictor-based methods have substantially enhanced Neural Architecture Search (NAS) optimization. The efficacy of these predictors is largely influenced by the method of encoding neural network architectures. While traditional encodings used an adjacency matrix describing the graph structure of a neural network, novel encodings embrace a variety of approaches from unsupervised pretraining of latent representations to vectors of zero-cost proxies. In this paper, we categorize and investigate neural encodings from three main types: structural, learned, and score-based. Furthermore, we extend these encodings and introduce \textit{unified encodings}, that extend NAS predictors to multiple search spaces. Our analysis draws from experiments conducted on over 1.5 million neural network architectures on NAS spaces such as NASBench-101 (NB101), NB201, NB301, Network Design Spaces (NDS), and TransNASBench-101. Building on our study, we present our predictor \textbf{FLAN}: \textbf{Fl}ow \textbf{A}ttention for \textbf{N}AS. FLAN integrates critical insights on predictor design, transfer learning, and \textit{unified encodings} to enable more than an order of magnitude cost reduction for training NAS accuracy predictors. Our implementation and encodings for all neural networks are open-sourced at \href{https://github.com/abdelfattah-lab/flan_nas}{https://github.com/abdelfattah-lab/flan\_nas}.
