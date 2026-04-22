
#### Q1. What is tokenization, and why is it important in LLMs?
Tokenization is the process of splitting text into smaller units called **tokens**, which can be words, subwords, or even characters. This step is crucial because LLMs do not understand raw text directly — they process sequences of numbers representing these tokens.

Effective tokenization allows models to:
- Handle various languages and scripts
- Manage rare or out-of-vocabulary words
- Reduce vocabulary size, improving both efficiency and performance

---

#### Q2. What is LoRA and QLoRA?
LoRA and QLoRA are techniques designed to optimize the fine-tuning of Large Language Models (LLMs), focusing on reducing memory usage and enhancing efficiency without compromising performance in Natural Language Processing (NLP) tasks.

**LoRA** is a parameter-efficient fine-tuning method that introduces new trainable parameters to modify a model's behavior without increasing its overall size. By doing so, LoRA maintains the original parameter count, reducing the memory overhead typically associated with training large models. It works by adding low-rank matrix adaptations to the model's existing layers, allowing for significant performance improvements while keeping resource consumption in check.

**QLoRA** builds on LoRA by incorporating quantization to further optimize memory usage. It uses techniques such as 4-bit Normal Float, Double Quantization, and Paged Optimizers to compress the model's parameters and improve computational efficiency. This method is particularly useful when scaling large models, as it maintains performance levels comparable to full-precision models while significantly reducing resource consumption.

---

