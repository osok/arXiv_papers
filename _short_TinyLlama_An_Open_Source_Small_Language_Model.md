# SUMMARY
The paper presents the pre-training and architecture of Tiny Llama, a language model combining natural language and code data, achieving superior performance and efficiency.

# IDEAS:
- Tiny Llama combines natural language data from Slim Pajama and code data from Star Coder.
- Approximately 950 billion tokens were used for pre-training Tiny Llama.
- Slim Pajama, derived from Red Pajama, contains over 1.2 trillion tokens.
- Star Coder data includes approximately 250 billion tokens across 86 programming languages.
- Llama's tokenizer processes the data for training Tiny Llama.
- Tiny Llama was trained on these tokens for approximately three epochs.
- Rotary positional embedding (RoPE) injects positional information into the model.
- RMS Norm is applied before each Transformer sublayer to improve training efficiency.
- S Glue activation function combines Swish and gated linear unit (GLU).
- 32 heads for query attention and four groups of key-value heads reduce memory bandwidth overhead.
- Fully sharded data parallel (FSDP) leverages multi-GPU and multi-node setups efficiently.
- Flash Attention 2 boosts computational throughput in Tiny Llama.
- Fused layer norm, cross entropy loss, and rotary positional embedding enhance efficiency.
- Original Sweet Glue module from Xformer repository further enhances efficiency.
- Training throughput of 24,000 tokens per second per A140 G GPU is achieved.
- Tiny Llama requires fewer GPU hours for training compared to Pythia 1.0B and MPT 1.3B models.
- Tiny Llama outperforms baseline models on common sense reasoning tasks like HellaSwag and OpenBookQA.
- Accuracy improves with increased computational resources, surpassing Pythia 1.4B in most benchmarks.
- Superior problem-solving skills demonstrated on tasks like Massive Multitask Language Understanding (MMLU).
- Tiny Llama excels in Big Bench Hard (BBH) and Discrete Reasoning Over Paragraphs (DROP).
- Human evaluation shows Tiny Llama's superior performance compared to existing models.

# INSIGHTS:
- Combining natural language and code data enhances language model performance.
- Rotary positional embedding improves positional information injection in models.
- RMS Norm before each Transformer sublayer boosts training efficiency.
- S Glue activation function offers advantages over traditional ReLU nonlinearity.
- Grouped query attention reduces memory bandwidth overhead and speeds up inference.
- Fully sharded data parallelism optimizes multi-GPU and multi-node setups.
- Flash Attention 2 significantly increases computational throughput.
- Fused techniques enhance codebase efficiency and reduce memory footprint.
- Training throughput of 24,000 tokens per second per GPU is highly efficient.
- Fewer GPU hours required for training indicate effective optimization.

# QUOTES:
- "We combine natural language data from the Slim Pajama Corpus and code data from the Star Coder Data Corpus."
- "Approximately 950 billion tokens were used for pre-training."
- "Rotary positional embedding (RoPE) injects positional information into the model."
- "RMS Norm is applied as the normalization technique before each Transformer sublayer."
- "We introduce the S Glue activation function, a combination of Swish and gated linear unit (GLU)."
- "32 heads for query attention and four groups of key-value heads reduce memory bandwidth overhead."
- "Fully sharded data parallel (FSDP) leverages multi-GPU and multi-node setups efficiently."
- "Flash Attention 2 boosts computational throughput in Tiny Llama."
- "Fused layer norm, cross entropy loss, and rotary positional embedding enhance efficiency."
- "Original Sweet Glue module from Xformer repository further enhances efficiency."
- "Training throughput of 24,000 tokens per second per A140 G GPU is achieved."
- "Tiny Llama requires fewer GPU hours for training compared to Pythia 1.0B and MPT 1.3B models."
- "Tiny Llama outperforms baseline models on common sense reasoning tasks like HellaSwag and OpenBookQA."
- "Accuracy improves with increased computational resources, surpassing Pythia 1.4B in most benchmarks."
- "Superior problem-solving skills demonstrated on tasks like Massive Multitask Language Understanding (MMLU)."
- "Tiny Llama excels in Big Bench Hard (BBH) and Discrete Reasoning Over Paragraphs (DROP)."
- "Human evaluation shows Tiny Llama's superior performance compared to existing models."

# HABITS:
- Combining diverse data sources for comprehensive model training.
- Utilizing advanced normalization techniques to improve training efficiency.
- Implementing innovative activation functions for better model performance.
- Leveraging multi-GPU and multi-node setups for optimized training.

# FACTS:
- Slim Pajama contains over 1.2 trillion tokens derived from Red Pajama Corpus.
- Star Coder data includes approximately 250 billion tokens across 86 programming languages.
- Training throughput of 24,000 tokens per second per A140 G GPU is achieved.

# REFERENCES:
- Slim Pajama Corpus
- Star Coder Data Corpus
- Red Pajama Corpus
- Xformer repository

# ONE-SENTENCE TAKEAWAY
Combining diverse data sources with advanced techniques results in highly efficient and superior-performing language models.

# RECOMMENDATIONS:
- Combine natural language and code data for enhanced language model performance.
- Use rotary positional embedding to improve positional information injection in models.
- Apply RMS Norm before each Transformer sublayer to boost training efficiency.
- Implement S Glue activation function for better model performance over traditional ReLU nonlinearity.
- Reduce memory bandwidth overhead with grouped query attention to speed up inference.