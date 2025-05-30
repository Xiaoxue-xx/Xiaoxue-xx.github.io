---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
Hi, welcome to my website! I am Xiaoxue Cheng (成晓雪), a second-year master’s student in Artificial Intelligence at Renmin University of China, under the supervision of [Prof. Xin Zhao](http://aibox.ruc.edu.cn/). I completed my undergraduate studies at Tianjin University, where I majored in Artificial Intelligence. My research interests include natural language processing, particularly with large language models (LLMs).

# Experiences

* Feb. 2025 – May. 2025: Internship at Ant Group
* Mar. 2024 – Feb. 2025: Internship at Kuaishou

## Education

- Master student, Artificial Intelligence, Renmin University of China, Sept. 2023 - Jul. 2026 (Expected)
- Bachelor of Engineering, Artificial Intelligence, Tianjin University, Sept. 2019 - Jul. 2023

# Publications

[**ACL 2025 Findings**] **Think More, Hallucinate Less: Mitigating Hallucinations via Dual Process of Fast and Slow Thinking**[[paper](https://arxiv.org/abs/2501.01306)]

**Xiaoxue Cheng†**, Junyi Li†, Wayne Xin Zhao, Ji-Rong Wen

Large language models (LLMs) demonstrate exceptional capabilities, yet still face the hallucination issue. Typical text generation approaches adopt an auto-regressive generation without deliberate reasoning, often leading to untrustworthy and factually inaccurate responses. In this paper, we propose **HaluSearch**, a novel framework that incorporates tree search-based algorithms (e.g., MCTS) to enable an explicit slow thinking generation process for mitigating hallucinations during inference. Specifically, HaluSearch frames text generation as a step-by-step reasoning process, using a self-evaluation reward model to score each generation step and guide the tree search towards the most reliable generation pathway. To balance efficiency and quality, we introduce a hierarchical system switch mechanism inspired by the dual process theory in cognitive science, which dynamically switches between fast and slow thinking modes at both instance and step levels. We conduct extensive experiments on both English and Chinese datasets, and the results show that our approach significantly outperforms baseline approaches.

[**EMNLP 2024 Main**] **Small Agent Can Also Rock! Empowering Small Language Models as Hallucination Detector**[[paper](https://arxiv.org/abs/2406.11277)] [[code](https://github.com/RUCAIBox/HaluAgent)]

**Xiaoxue Cheng†**, Junyi Li†, Wayne Xin Zhao, Hongzhi Zhang, Fuzheng Zhang, Di Zhang, Kun Gai, Ji-Rong Wen

Hallucination detection is a challenging task for large language models (LLMs), and existing studies heavily rely on powerful closed-source LLMs such as GPT-4. In this paper, we propose an autonomous LLM-based agent framework, called HaluAgent, which enables relatively smaller LLMs (e.g. Baichuan2-Chat 7B) to actively select suitable tools for detecting multiple hallucination types such as text, code, and mathematical expression. In HaluAgent, we integrate the LLM, multi-functional toolbox, and design a fine-grained three-stage detection framework along with memory mechanism. To facilitate the effectiveness of HaluAgent, we leverage existing Chinese and English datasets to synthesize detection trajectories for fine-tuning, which endows HaluAgent with the capability for bilingual hallucination detection. Extensive experiments demonstrate that only using 2K samples for tuning LLMs, HaluAgent can perform hallucination detection on various types of tasks and datasets, achieving performance comparable to or even higher than GPT-4 without tool enhancements on both in-domain and out-of-domain datasets.

[**ACL 2024 Main**] **The Dawn After the Dark: An Empirical Study on Factuality Hallucination in Large Language Models** [[paper](https://arxiv.org/abs/2401.03205)] [[code](https://github.com/RUCAIBox/HaluEval-2.0)]

Junyi Li,  Jie Chen,  Ruiyang Ren,  **Xiaoxue Cheng**,  Wayne Xin Zhao,  Jian-Yun Nie, Ji-Rong Wen

In the era of large language models (LLMs), hallucination (i.e., the tendency to generate factually incorrect content) poses great challenge to trustworthy and reliable deployment of LLMs in real-world applications. To tackle the LLM hallucination, three key questions should be well studied: how to detect hallucinations (detection), why do LLMs hallucinate (source), and what can be done to mitigate them (mitigation). To address these challenges, this work presents a systematic empirical study on LLM hallucination, focused on the the three aspects of hallucination detection, source and mitigation. Specially, we construct a new hallucination benchmark HaluEval 2.0, and designs a simple yet effective detection method for LLM hallucination. Furthermore, we zoom into the different training or utilization stages of LLMs and extensively analyze the potential factors that lead to the LLM hallucination. Finally, we implement and examine a series of widely used techniques to mitigate the hallucinations in LLMs. Our work has led to several important findings to understand the hallucination origin and mitigate the hallucinations in LLMs.

[**LREC-COLING  2024**] **ChainLM: Empowering Large Language Models with Improved Chain-of-Thought Prompting** [[paper](https://arxiv.org/abs/2403.14312)] [[code](https://github.com/Xiaoxue-xx/ChainLM)]

**Xiaoxue Cheng**,  Junyi Li,  Wayne Xin Zhao, Ji-Rong Wen

Chain-of-Thought (CoT) prompting can enhance the reasoning capabilities of large language models (LLMs), establishing itself as a primary approach to solving complex reasoning tasks. Existing CoT synthesis approaches usually focus on simpler reasoning tasks and thus result in low-quality and inconsistent CoT prompts. In response to this challenge, we present an empirical investigation of CoT prompting and introduce CoTGenius, a novel framework designed for the automatic generation of superior CoT prompts. CoTGenius is developed based on three major evolution strategies, i.e., complicate, diversify, and specify-alongside two filtering mechanisms: evolutionary success judgement and correctness verification. We further employ CoTGenius to create an extensive CoT dataset, and subsequently fine-tune the Llama 2-Chat 7B and 13B models on this dataset. We call the resulting model ChainLM. To deal with the cumulative error issue in reasoning steps, we propose a step-level debating method, wherein multiple debaters discuss each reasoning step to arrive at the correct answer. Extensive experiments demonstrate that our ChainLM models exhibit enhanced proficiency in addressing a spectrum of complex reasoning problems compared to existing models. In addition, we conduct an in-depth analysis of the impact of data categories within CoTGenius on the model performance.

[**EMNLP 2023 Main**] **HaluEval: A Large-Scale Hallucination Evaluation Benchmark for Large Language Models** [[paper](https://arxiv.org/abs/2305.11747)] [[code](https://github.com/RUCAIBox/HaluEval)]

Junyi Li †,  **Xiaoxue Cheng** †,  Wayne Xin Zhao ,  Jian-Yun Nie , Ji-Rong Wen

Large language models (LLMs), such as ChatGPT, are prone to generate hallucinations, i.e., content that conflicts with the source or cannot be verified by the factual knowledge. To understand what types of content and to which extent LLMs are apt to hallucinate, we introduce the Hallucination Evaluation benchmark for Large Language Models (HaluEval), a large collection of generated and human-annotated hallucinated samples for evaluating the performance of LLMs in recognizing hallucination. To generate these samples, we propose a ChatGPT-based two-step framework, i.e., sampling-then-filtering. Besides, we also hire some human labelers to annotate the hallucinations in ChatGPT responses. The empirical results suggest that ChatGPT is likely to generate hallucinated content in specific topics by fabricating unverifiable information (i.e., about **19.5**% responses). Moreover, existing LLMs face great challenges in recognizing the hallucinations in texts. However, our experiments also prove that providing external knowledge or adding reasoning steps can help LLMs recognize hallucinations.

# Honors

- National Scholarship, 2020
