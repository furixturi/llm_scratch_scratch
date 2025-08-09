# Positional Encoding Variants

Self-attention is permutation-invariatnt. Each query token attends to all its context tokens simultaneously, meaning, unlike RNN/CNNs, Transformers have no built-in notion of word order. 

Postional encoding injects position information. It can be fixed (sinusoidal), learned, relative, or functional (RoPE, ALiBi, etc.)

In this folder we implement three variants of positional encoding

- [sinusoidal positional encoding](./SinPosEncoding/SinPosEncoding.ipynb)
  - Fixed (absolute) encoding. Used in the original Transformer.
  - Injected to input embeddings
- [learned absolute positional embeddings](./LearnedAbsolutePosEncoding/LearnedAbsolutePosEncoding.ipynb)
- [relative positional encoding](./RelativePosEncoding/RelativePosEncoding.ipynb)
  - Use relative position instead of absolute index. Used in Transformer-XL, T5, DeBERTa, etc. 
  - Inside attention logits
- [rotary position encoding (RoPE)](./RoPE/RoPE.ipynb)
  - Apply a rotation to the query and key vectors in a high-dimensional space according to the position, using complex exponentials. Preserve absolute and relative positional relationships
  - The de facto especially for long contexts: GPT-NeoX, GPT-J, LLaMA 1/2/3, Qwen, BLOOM, Phi
  - In each attention's K/V 
- [Rope - YaRN](./RoPE/YaRN.ipynb)
  - Scale the frequencies used in RoPE's angle calculation to stretch the context window
  - LLaMA long, Qwen long