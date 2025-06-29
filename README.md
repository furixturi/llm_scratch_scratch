# LLM Scratch Scratch

## Intro

This is a scratchpad project that implements different LLM parts from scratch, also builds and trains small model variants of popular LLM architectures.

## Contents

### [LLM algo components](./llm_algo_components/)
- Attention
  - [scaled dot-product attention](./llm_algo_components/attention/scaled_dot_product_attention/)
  - [multi-head attention](./llm_algo_components/attention/MHA/)

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

## History

- 2025/06/26 Project start
- 2025/06/27 
  - Add [scaled dot-product attention](./llm_algo_components/attention/scaled_dot_product_attention/)
  - Add [multi-head attention (MHA)](./llm_algo_components/attention/MHA/)
- 2025/06/29
  - Add [multi-query attention (MQA)](./llm_algo_components/attention/MQA/)
  - Add attention and MHA variants explanation in [attention readme](./llm_algo_components/attention/README.md)
