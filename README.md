# LLM Scratch Scratch

## Intro

This is a scratchpad project that implements different LLM parts from scratch, also builds and trains small model variants of popular LLM architectures.

## Contents

### [LLM algo components](./llm_algo_components/)
- Attention
  - [scaled dot-product attention](./llm_algo_components/attention/scaled_dot_product_attention/)
  - Multi-head variants
    - [Multi-Head Attention (MHA)](./llm_algo_components/attention/MHA/)
    - [Multi-Query Attention (MQA)](./llm_algo_components/attention/MQA/)
    - [Grouped-Query Attention (GQA)](./llm_algo_components/attention/GQA/)
    - [Multi-head Latent Attention (MLA)](./llm_algo_components/attention/MLA/)

### Models From Scratch

### Training / Fine-tuning 

### Optimization / Distributed


## Acknowledgments

### Book
- [Sebastian Raschka](https://sebastianraschka.com/) 's amazing book [Build a Large Language Model From Scratch](https://www.manning.com/books/build-a-large-language-model-from-scratch)

### Papers
- Transformer paper [Attention Is All You Need (arxiv.org/abs/1706.03762)](https://arxiv.org/abs/1706.03762)
- MQA paper [Fast Transformer Decoding: One Write-Head is All You Need (arxiv.org/abs/1911.02150)](https://arxiv.org/abs/1911.02150)
- GQA paper [GQA: Training Generalized Multi-Query Transformer Models from Multi-Head Checkpoints (arxiv.org/abs/2305.13245)](https://arxiv.org/abs/2305.13245)
- DeepSeek-v2 paper (proposed MLA) [DeepSeek-V2: A Strong, Economical, and Efficient Mixture-of-Experts Language Model](https://arxiv.org/abs/2405.04434)

### Online articles
- [Sebastian Raschka](https://www.linkedin.com/in/sebastianraschka/)'s [The Big LLM Architecture Comparison](https://magazine.sebastianraschka.com/p/the-big-llm-architecture-comparison)

### Code
- [Frank Odom](http://fkodom.substack.com/)'s [GQA PyTorch implementation](https://github.com/fkodom/grouped-query-attention-pytorch/tree/main)

## History

- 2025/06/26 Project start
- 2025/06/27 
  - Add [scaled dot-product attention](./llm_algo_components/attention/scaled_dot_product_attention/)
  - Add [multi-head attention (MHA)](./llm_algo_components/attention/MHA/)
- 2025/06/29
  - Add [multi-query attention (MQA)](./llm_algo_components/attention/MQA/)
  - Add attention and MHA variants explanation in [attention readme](./llm_algo_components/attention/README.md)
- 2025/07/24 
  - Add [multi-head latent attention (MLA)](./llm_algo_components/attention/MLA/)
- 2025/08/05
  - Update MLA implementation to follow DeepSeek-v2 official formula