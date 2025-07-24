# Attention Variants

The attention mechanism, multi-head attention and its variants' implemenations in this folder are recommended to be read and understood in the following order as the complexity grows:

- [Scaled Dot-Product Attention](./scaled_dot_product_attention/scaled_dot_product_attention.ipynb)
  - The basic attention mechanism 
    $$Attention(Q,K,V) = Softmax(\frac{QK^T}{\sqrt{d_k}})V$$ 
    that is used in all multi-head attention variants. 
  - This implementation supports a mask for causal attention
- [Multi-Head Attention (MHA)](./MHA/MHA.ipynb)
  - Split Q, K, V into multiple attention heads for more expressive learning. Using matrix multiplication the multi-head attention compute can be batched.
  - High quality at the cost of large compute and memory consumption.
- [Multi-Query Attention (MQA)](./MQA/MQA.ipynb)
  - Share K and V across all Q heads to greatly decrase compute and memory usage, making decoding much more efficient.
  - Good for infernece as the KV cache is greatly decrased. The cost is a minor quality degradation. 
- [Grouped-Query Attention (GQA)](./GQA/GQA.ipynb)
  - Share K and V in groups of Qs heads. Strike a balance between MHA and MQA. 
- [Multi-head Latent Attention (MLA)](./MLA/MLA.ipynb)
  - Drastically reduce KV cache memory footprint at inference by down-projecting K, V matrices to a smaller latent matrix.