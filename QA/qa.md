<div style="max-width: 820px; margin: 0 auto; padding: 24px 24px;">

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

#### Q3. Explain the concept of temperature in LLM text generation.
Temperature is a hyperparameter that controls the randomness of text generation by adjusting the probability distribution over possible next tokens. 

A low temperature (close to 0) makes the model highly deterministic, favoring the most probable tokens. Conversely, a high temperature (above 1) encourages more diversity by flattening the distribution, allowing less probable tokens to be selected. For instance, a temperature of 0.7 strikes a balance between creativity and coherence, making it suitable for generating diverse but sensible outputs.

---

#### Q4. What is masked language modeling, and how does it contribute to model pretraining?

Masked language modeling (MLM) is a training objective where some tokens in the input are randomly masked, and the model is tasked with predicting them based on context. This forces the model to learn contextual relationships between words, enhancing its ability to understand language semantics. MLM is commonly used in models like BERT, which are pretrained using this objective to develop a deep understanding of language before fine-tuning on specific tasks.

| Pros                                   | Cons                          |
|-----------------------------------------|-------------------------------|
| Enhances contextual understanding      | Requires large amount of data |
| Improves language semantics            | Computationally expensive     |
| Pretraining for fine-tuning            | Potential for overfitting     |
| Widely used in BERT                    | Masking randomness           |

---

#### Q5. What are Sequence-to-Sequence Models?
Sequence-to-Sequence (Seq2Seq) Models are a type of neural network architecture designed to transform one sequence of data into another sequence. These models are commonly used in tasks where the input and output have variable lengths, such as in machine translation, text summarization, and speech recognition.

---

#### Q6. How do autoregressive models differ from masked models in LLM training?
Autoregressive models, such as GPT, generate text one token at a time, with each token predicted based on the previously generated tokens. This sequential approach is ideal for tasks like text generation. Masked models, like BERT, predict randomly masked tokens within a sentence, leveraging both left and right context. Autoregressive models excel in generative tasks, while masked models are better suited for understanding and classification tasks.

---

</div>