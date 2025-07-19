# Awesome Text Generation Evaluation
Awesome Text Generation Evaluation: a curated list of evaluation metrics for Natural Language Generation (NLG)

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/SuperBruceJia/Awesome-Text-Generation-Evaluation) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Made With Love](https://img.shields.io/badge/Made%20With-Love-red.svg)](https://github.com/SuperBruceJia/Awesome-Text-Generation-Evaluation)

This repository, called **Awesome Text Generation Evaluation**, contains a collection of resources and papers 
on _reference-based_ and _reference-free_ evaluation metrics for **Natural Language Generation** (NLG). 

"*If you can't measure it, you can't improve it*. " - British Physicist William Thomson

*Welcome to share your papers, thoughts, and ideas by [submitting an issue](https://github.com/SuperBruceJia/Awesome-Text-Generation-Evaluation/issues/new)!*

## Contents
- [Survey](#Survey)
- [Human Judgement Datasets](#Human-Judgement-Datasets)
- [Lexical Overlap as Evaluator](#Lexical-Overlap-as-Evaluator)
  - [N-gram-based Metrics](#N-gram-based-Metrics)
  - [Edit Distance-based Metrics](#Edit-Distance-based-Metrics)
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

# Survey
**Reference-free Evaluation Metrics for Text Generation: A Survey**\
*Takumi Ito, Kees van Deemter, Jun Suzuki*\
arXiv 2025, [[Paper](https://arxiv.org/pdf/2501.12011)]\
21 Jan 2025

**Text Generation: A Systematic Literature Review of Tasks, Evaluation, and Challenges**\
*Jonas Becker, Jan Philip Wahle, Bela Gipp, Terry Ruas*\
arXiv 2024, [[Paper](https://arxiv.org/pdf/2405.15604)]\
29 Aug 2024

**Towards Explainable Evaluation Metrics for Natural Language Generation**\
*Christoph Leiter, Piyawat Lertvittayakumjorn, Marina Fomicheva, Wei Zhao, Yang Gao, Steffen Eger*\
arXiv 2022, [[Paper](https://arxiv.org/pdf/2203.11131)] [[GitHub](https://github.com/Gringham/explainable-metrics-machine-translation)]\
21 Mar 2022

**Repairing the Cracked Foundation: A Survey of Obstacles in Evaluation Practices for Generated Text**\
*Sebastian Gehrmann, Elizabeth Clark, Thibault Sellam*\
Journal of Artificial Intelligence Research 2022, [[Paper](https://dl.acm.org/doi/pdf/10.1613/jair.1.13715)]\
14 Feb 2022

**Evaluation of Text Generation: A Survey**\
*Asli Celikyilmaz, Elizabeth Clark, Jianfeng Gao*\
arXiv 2021, [[Paper](https://arxiv.org/pdf/2006.14799)]\
18 May 2021

# Human Judgement Datasets
**People Overtrust AI-Generated Medical Advice despite Low Accuracy**\
*Shruthi Shekar, Pat Pataranutaporn, Chethan Sarabu, Guillermo A. Cecchi, Pattie Maes*\
NEJM AI 2025, [[Paper](https://arxiv.org/pdf/2408.15266)] [[GitHub](https://github.com/mitmedialab/LLM-MedQA)] [[Dataset](https://github.com/mitmedialab/LLM-MedQA/tree/main/Expert%20Evaluation%20%26%20Dataset%20Generation)]\
11 Aug 2024

**AlpacaEval: An Automatic Evaluator for Instruction-following Language Models**\
*Xuechen Li, Tianyi Zhang, Yann Dubois, Rohan Taori, Ishaan Gulrajani, Carlos Guestrin, Percy Liang, and Tatsunori B. Hashimoto*\
Online Leaderboard, [[Leaderboard](https://tatsu-lab.github.io/alpaca_eval/)] [[GitHub](https://github.com/tatsu-lab/alpaca_eval)] [[Dataset](https://huggingface.co/datasets/tatsu-lab/alpaca_eval/blob/main/alpaca_farm_human_crossannotations.json)]\
2023

**A Critical Evaluation of Evaluations for Long-form Question Answering**\
*Fangyuan Xu, Yixiao Song, Mohit Iyyer, Eunsol Choi*\
ACL 2023, [[Paper](https://aclanthology.org/2023.acl-long.181.pdf)] [[GitHub](https://github.com/carriex/lfqa_eval)] [[Dataset](https://github.com/carriex/lfqa_eval/tree/main/preference_data)]\
29 May 2023

**WebGPT: Browser-assisted Question-answering with Human Feedback**\
*Nisan Stiennon, Long Ouyang, Jeff Wu, Daniel M. Ziegler, Ryan Lowe, Chelsea Voss, Alec Radford, Dario Amodei, Paul Christiano*\
arXiv 2022, [[Paper](https://cdn.openai.com/WebGPT.pdf)] [[Official Dataset](https://huggingface.co/datasets/openai/webgpt_comparisons)] [[Processed Dataset](https://github.com/carriex/lfqa_eval/tree/main/preference_data)]\
1 Jun 2022

**Learning to Summarize From Human Feedback**\
*Reiichiro Nakano, Jacob Hilton, Suchir Balaji, Jeff Wu, Long Ouyang, Christina Kim, Christopher Hesse, Shantanu Jain, Vineet Kosaraju, William Saunders, Xu Jiang, Karl Cobbe, Tyna Eloundou, Gretchen Krueger, Kevin Button, Matthew Knight, Benjamin Chess, John Schulman*\
NeurIPS 2020, [[Paper](https://proceedings.neurips.cc/paper/2020/file/1f89885d556929e98d3ef9b86448f951-Paper.pdf)] [[GitHub](https://github.com/openai/summarize-from-feedback)] [[Dataset](https://github.com/openai/summarize-from-feedback?tab=readme-ov-file#human-feedback-data)]\
15 Feb 2022

**Evaluating Question Answering Evaluation**\
*Anthony Chen, Gabriel Stanovsky, Sameer Singh, and Matt Gardner*\
Proceedings of the Second Workshop on Machine Reading for Question Answering 2019, [[Workshop Paper](https://aclanthology.org/D19-5817.pdf)] [[Symposium Paper]](https://cseweb.ucsd.edu/~jmcauley/workshops/scmls20/papers/scmls20_paper_34.pdf) [[Presentation](https://anthonywchen.github.io/Papers/evaluatingqa/mrqa_slides.pdf)] [[Dataset](https://anthonywchen.github.io/Papers/evaluatingqa/correlation_data.zip)]\
2019

# Lexical Overlap as Evaluator
## N-gram-based Metrics
**chrF: Character _N_-gram F-score for Automatic MT Evaluation**\
*Maja Popovic*\
Workshop on Statistical Machine Translation 2015, [[Paper](https://aclanthology.org/W15-3049.pdf)] [[GitHub](https://github.com/m-popovic/chrF)] [[Hugging Face]](https://huggingface.co/spaces/evaluate-metric/chrf)\
2015

**METEOR: An Automatic Metric for MT Evaluation with Improved Correlation with Human Judgments**\
*Satanjeev Banerjee, Alon Lavie*\
ACL Workshop on Intrinsic and Extrinsic Evaluation Measures for Machine Translation and/or Summarization 2005, [[Paper](https://aclanthology.org/W05-0909.pdf)]\
2005

**ROUGE: A Package for Automatic Evaluation of Summaries**\
*Chin-Yew Lin*\
Proceedings of Workshop on Text Summarization Branches Out 2004, [[Paper](https://aclanthology.org/W04-1013.pdf)]\
2004

**BLEU: A Method for Automatic Evaluation of Machine Translation**\
*Kishore Papineni, Salim Roukos, Todd Ward, Wei-Jing Zhu*\
ACL 2002, [[Paper](https://aclanthology.org/P02-1040.pdf)]\
2002

## Edit Distance-based Metrics
**Sentence Mover’s Similarity: Automatic Evaluation for Multi-Sentence Texts**\
*Elizabeth Clark, Asli Celikyilmaz, Noah A. Smith*\
ACL 2019, [[Paper](https://aclanthology.org/P19-1264v2.pdf)] [[GitHub](https://github.com/eaclark07/sms)]\
2019

**From Word Embeddings To Document Distances**\
*Matt Kusner, Yu Sun, Nicholas Kolkin, Kilian Weinberger*\
ICML 2015, [[Paper](https://proceedings.mlr.press/v37/kusnerb15.pdf)] [[GitHub](https://github.com/mkusner/wmd)]\
2015

# Learned Metrics as Evaluator
## Supervised Learned Metrics
### Supervised Regression with Human Judgment Data
**BLEURT: Learning Robust Metrics for Text Generation**\
*Thibault Sellam, Dipanjan Das, Ankur P. Parikh*\
ACL 2020, [[Paper](https://aclanthology.org/2020.acl-main.704.pdf)]\
21 May 2020 

### Ranking Hypothesis Sentences
**COMET: A Neural Framework for MT Evaluation**\
*Ricardo Rei, Craig Stewart, Ana C Farinha, Alon Lavie*\
EMNLP 2020, [[Paper](https://aclanthology.org/2020.emnlp-main.213.pdf)]\
19 Oct 2020

**BEER: BEtter Evaluation as Ranking**\
*Miloš Stanojević, Khalil Sima’an*\
Workshop on Statistical Machine Translation 2014, [[Paper](https://aclanthology.org/W14-3354.pdf)]\
2014

### Sequence-to-sequence Learning and Probability Estimation
**Paraphrase Generation as Zero-Shot Multilingual Translation: Disentangling Semantic Similarity from Lexical and Syntactic Diversity**\
*Brian Thompson, Matt Post*\
WMT 2020, [[Paper](https://aclanthology.org/2020.wmt-1.67.pdf)]\
28 Oct 2020

## Unsupervised Learned Metrics
### Embedding-based Metrics
**BERTScore: Evaluating Text Generation with BERT**\
*Tianyi Zhang, Varsha Kishore, Felix Wu, Kilian Q. Weinberger, Yoav Artzi*\
ICLR 2020, [[Paper](https://openreview.net/pdf?id=SkeHuCVFDr)] [[GitHub](https://github.com/Tiiiger/bert_score)] [[Hugging Face](https://huggingface.co/spaces/evaluate-metric/bertscore)]\
24 Feb 2020

**MoverScore: Text Generation Evaluating with Contextualized Embeddings and Earth Mover Distance**\
*Wei Zhao, Maxime Peyrard, Fei Liu, Yang Gao, Christian M. Meyer, Steffen Eger*\
EMNLP 2019, [[Paper](https://aclanthology.org/D19-1053.pdf)] [[GitHub](https://github.com/AIPHES/emnlp19-moverscore)]\
26 Sep 2019

### Text Generation-based Metrics
**BARTScore: Evaluating Generated Text as Text Generation**\
*Weizhe Yuan, Graham Neubig, Pengfei Liu*\
NeurIPS 2021, [[Paper](https://proceedings.neurips.cc/paper/2021/file/e4d2b6e6fdeca3e60e0f1a62fee3d9dd-Paper.pdf)] [[GitHub](https://github.com/neulab/BARTScore)]\
27 Oct 2021

# Explainability-driven Metrics as Evaluator
## Error Measurement
**INSTRUCTSCORE: Explainable Text Generation Evaluation with Finegrained Feedback**\
*Wenda Xu, Danqing Wang, Liangming Pan, Zhenqiao Song, Markus Freitag, William Yang Wang, Lei Li*\
EMNLP 2023, [[Paper](https://aclanthology.org/2023.emnlp-main.365.pdf)] [[GitHub](https://github.com/xu1998hz/InstructScore_SEScore3)]\
26 Oct 2023

**Toward Human-Like Evaluation for Natural Language Generation with Error Analysis**\
*Qingyu Lu, Liang Ding, Liping Xie, Kanjian Zhang, Derek F. Wong, Dacheng Tao*\
EMNLP 2023, [[Paper](https://aclanthology.org/2023.emnlp-main.365.pdf)] [[GitHub](https://github.com/Coldmist-Lu/ErrorAnalysis_NLGEvaluation)]\
20 Dec 2022

**Not All Errors are Equal: Learning Text Generation Metrics using Stratified Error Synthesis**\
*Wenda Xu, Yilin Tuan, Yujie Lu, Michael Saxon, Lei Li, William Yang Wang*\
EMNLP 2022, [[Paper](https://aclanthology.org/2022.findings-emnlp.489.pdf)] [[GitHub](https://github.com/xu1998hz/SEScore)]\
26 Oct 2022

**MaTESe: Machine Translation Evaluation as a Sequence Tagging Problem**\
*Stefano Perrella, Lorenzo Proietti, Alessandro Scirè, Niccolò Campolungo, Roberto Navigli*\
WMT 2022, [[Paper](https://aclanthology.org/2022.wmt-1.51.pdf)] [[GitHub](https://github.com/SapienzaNLP/MaTESe)]\
2022

## Adversarial Samples

## Multi-dimension Disentanglement
**Is ChatGPT a Good NLG Evaluator? A Preliminary Study**\
*Jiaan Wang, Yunlong Liang, Fandong Meng, Zengkui Sun, Haoxiang Shi, Zhixu Li, Jinan Xu, Jianfeng Qu, Jie Zhou*\
New Frontiers in Summarization Workshop 2023, [[Paper](https://aclanthology.org/2023.newsum-1.1.pdf)] [[GitHub](https://github.com/krystalan/chatgpt_as_nlg_evaluator)]\
24 Oct 2023

**GPTScore: Evaluate as You Desire**\
*Jinlan Fu, See-Kiong Ng, Zhengbao Jiang, Pengfei Liu*\
NAACL 2024, [[Paper](https://aclanthology.org/2024.naacl-long.365.pdf)] [[GitHub](https://github.com/jinlanfu/GPTScore)]\
13 Feb 2023

**G-Eval: NLG Evaluation using GPT-4 with Better Human Alignment**\
*Yang Liu, Dan Iter, Yichong Xu, Shuohang Wang, Ruochen Xu, Chenguang Zhu*\
EMNLP 2023, [[Paper](https://aclanthology.org/2023.emnlp-main.153.pdf)] [[GitHub](https://github.com/nlpyang/geval)]\
23 May 2023



