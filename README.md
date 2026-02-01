# Stealthy Backdoors in RAG-Based LLM Systems

## Abstract

Retrieval-Augmented Generation (RAG) combines a Large Language Model (LLM) with an external corpus, retrieving passages that condition the LLM’s outputs. While this grounds responses in relevant information, it also creates security risks. We study retrieval-time poisoning in which an adversarial corpus passage is paired with a trigger phrase that must appear in a user query to activate the attack, causing the retriever to surface attacker-controlled content that can steer the LLM toward incorrect or misleading outputs. We propose two complementary attack strategies: (C1) learning multi-token trigger phrases that manipulate retrieval toward existing corpus passages; and (C2) injecting fluent, LLM-generated misinformation into the corpus that is selectively retrieved only when a secret trigger appears in the query. Our attacks achieve near-perfect retrieval success, showing that stealthy, targeted poisoning of RAG pipelines is feasible and underscoring the urgent need for effective defences.

## Usage

Create and activate the conda environment.

```
conda env create -f environment.yml
conda activate ICLR-Trustworthy-AI
```

Download the Natural Questions dataset from [https://drive.google.com/drive/folders/1ORuqznzMf9Xv6y7epjdIVl28PwgUKZnn?usp=sharing](https://drive.google.com/drive/folders/1ORuqznzMf9Xv6y7epjdIVl28PwgUKZnn?usp=sharing). Extract the contents of the ZIP file into the repository root.

## License

Stealthy Backdoors in RAG-Based LLM Systems © 2026 by [REDACTED] is licensed under CC BY 4.0. To view a copy of this license, visit [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/).
