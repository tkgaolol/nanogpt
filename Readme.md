# NanoGPT Study Repository

This repository contains my study implementation and notes for [@karpathy's build-nanogpt](https://github.com/karpathy/build-nanogpt) tutorial. It's a from-scratch reproduction of GPT-2.

## Repository Structure

### Core Training Files
- **`train.py`** - Main training script with complete GPT implementation including:
  - Multi-head self-attention with Flash Attention optimization
  - MLP blocks with GELU activation
  - Layer normalization and residual connections
  - Data loading and distributed training support
  - HellaSwag evaluation integration

### Data Processing
- **`fineweb.py`** - FineWeb-Edu dataset downloader and tokenizer
  - Downloads 10B token dataset for pretraining
  - GPT-2 tokenization using tiktoken
  - Efficient data sharding for large-scale training

- **`input.txt`** - Sample text data for quick experiments

### Evaluation
- **`hellaswag.py`** - HellaSwag benchmark evaluation script
  - Common sense reasoning evaluation
  - Multiple choice completion task
  - Model performance comparison utilities

### Exploration
- **`play.ipynb`** - Jupyter notebook for interactive experimentation
  - Model testing and inference
  - Training visualization
  - Architecture exploration


## References

- [Original Tutorial](https://github.com/karpathy/build-nanogpt) by Andrej Karpathy
- [Attention Is All You Need](https://arxiv.org/abs/1706.03762) - Original Transformer paper
- [GPT-2 Paper](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)
- [HellaSwag Benchmark](https://arxiv.org/abs/1905.07830)



 

