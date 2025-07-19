# Awesome Text Generation Evaluation
Awesome Text Generation Evaluation: a curated list of evaluation metrics for natural language generation (NLG)

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/SuperBruceJia/Awesome-Text-Generation-Evaluation) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Made With Love](https://img.shields.io/badge/Made%20With-Love-red.svg)](https://github.com/SuperBruceJia/Awesome-Text-Generation-Evaluation)

This repository, called **Awesome Text Generation Evaluation**, contains a collection of resources and papers 
on _reference-based_ and _reference-free_ evaluation metrics for **Natural Language Generation** (NLG). 

"*If you can't measure it, you can't improve it*. " - British Physicist William Thomson

*Welcome to share your papers, thoughts, and ideas by [submitting an issue](https://github.com/SuperBruceJia/Awesome-Text-Generation-Evaluation/issues/new)!*

## Contents
- [Presentations](#Presentations)
- [Survey](#Survey)
- [Benchmarks](#Benchmarks)
- [Lexical Overlap as Evaluator](#Lexical-Overlap-as-Evaluator)
  - [N-gram based Metrics](#N-gram-based-Metrics)
  - [Edit-distance based Metrics](#Edit-distance-based-Metrics)
- [Learned Metrics as Evaluator](#Learned-Metrics-as-Evaluator)
  - [Supervised Learned Metrics](#Supervised-Learned-Metrics)
    - [Supervised Regression with Human Judgment Data](#Supervised-Regression-with-Human-Judgment-Data)
    - [Ranking Hypothesis Sentences](#Ranking-Hypothesis-Sentences)
    - [Sequence-to-sequence Learning and Probability Estimation](#Sequence-to-sequence-Learning-and-Probability-Estimation)
  - [Unsupervised Learned Metrics](#Unsupervised-Learned-Metrics)
    - [Embedding-based Metrics](#Embedding-based-Metrics)
    - [Text Generation-based Metrics](#Text-Generation-based-Metrics)
- [Explainability-driven Metrics as Evaluator](#Explainability-driven-Metrics-as-Evaluator)
  - [Error Measurement](#Error-Measurement)
  - [Adversarial Samples](#Adversarial-Samples)
  - [Multi-dimension Disentanglement](#Multi-dimension-Disentanglement)
- [Citation](#Citation)
- [Acknowledgement](#Acknowledgement)

# Presentations

# Survey
**Reference-free Evaluation Metrics for Text Generation: A Survey**\
*Takumi Ito, Kees van Deemter, Jun Suzuki*\
arXiv 2025, [[Paper](https://arxiv.org/pdf/2501.12011)]\
21 Jan 2025

**Text Generation: A Systematic Literature Review of Tasks, Evaluation, and Challenges**\
*Jonas Becker, Jan Philip Wahle, Bela Gipp, Terry Ruas*\
arXiv 2024, [[Paper](https://arxiv.org/pdf/2405.15604)]\
29 Aug 2024

**Repairing the Cracked Foundation: A Survey of Obstacles in Evaluation Practices for Generated Text**\
*Sebastian Gehrmann, Elizabeth Clark, Thibault Sellam*\
Journal of Artificial Intelligence Research 2022, [[Paper](https://dl.acm.org/doi/pdf/10.1613/jair.1.13715)]\
14 Feb 2022

**Evaluation of Text Generation: A Survey**\
*Asli Celikyilmaz, Elizabeth Clark, Jianfeng Gao*\
arXiv 2021, [[Paper](https://arxiv.org/pdf/2006.14799)]\
18 May 2021

# Benchmarks
**A Critical Evaluation of Evaluations for Long-form Question Answering**\
*Fangyuan Xu, Yixiao Song, Mohit Iyyer, Eunsol Choi*\
ACL 2023, [[Paper](https://aclanthology.org/2023.acl-long.181.pdf)] [[GitHub](https://github.com/carriex/lfqa_eval)] [[Dataset](https://github.com/carriex/lfqa_eval/tree/main/preference_data)]\
29 May 2023
