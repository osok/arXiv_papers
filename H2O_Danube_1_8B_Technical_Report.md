# SUMMARY
H2O introduces the H2O danu 1.8B language model, built on Llama 2 and Mistol principles, excelling in various benchmarks.

# IDEAS:
- H2O danu 1.8B is a language model with 1.8 billion parameters trained on 1 trillion tokens.
- The model is based on foundational ideas from Llama 2 and Mistol, fine-tuned for efficiency.
- Despite fewer training tokens, H2O danu 1.8B performs well across a wide range of benchmarks.
- A chat model version has been developed, improved through supervised fine-tuning and direct preference optimization.
- Advanced language models use decoder attention architecture, benefiting from large pre-training datasets.
- Performance improves with larger model sizes, more data, and greater computational power.
- Smaller models are important for efficiency on consumer hardware and specific tasks.
- H2O danu 1.8B adopts key principles from Llama 2 and Mistol, trained on diverse data excluding coding data.
- The model architecture includes a hidden size of 2560, intermediate size of 6,912, and 24 hidden layers.
- Uses the original Llama 2 tokenizer with a vocabulary size of 32,000 and context length of 16,384 tokens.
- Features include a sliding window approach for local attention with a fixed window of 4,096 tokens.
- Rotary positional embedding (RoPE) helps the model understand sequence positions.
- Grouped query attention reduces memory usage with 32 attention heads and eight key-value heads.
- Root mean square layer normalization (RMS Norm) ensures stable training.
- No bias in linear layers or token embeddings is used in the model.
- Training utilized a single node with 8 H100 GPUs employing distributed data parallel (DDP).
- Training sequences increased from 248 to 16,384 tokens using a total of 700 billion tokens.
- Used 8-bit floating point calculations to speed up training with certain layers in FP8 precision.
- The AdamW optimizer with specific beta values and cosine learning rate scheduler was used.
- Achieved an average throughput of 292.50 tokens per second on a single node.
- H2O danu 1.8B is openly available under the Apache 2.0 license.
- Benchmarks include common sense reasoning, world knowledge, reading comprehension, and overall performance.
- Outperformed most competitors except for Stable LM2 in some areas.
- Chat model version trained with supervised fine-tuning on conversational input-output pairs.
- Direct preference optimization (DPO) used for fine-tuning with various data sets totaling 177,000 samples.
- Evaluated using Mt Bench for multi-turn questions excluding coding questions.
- Strong performance in natural language tasks, best in five out of seven categories for single-turn conversations.
- Weights of both intermediate and final DPO models are available online for community use.

# INSIGHTS:
- Smaller models can efficiently run on consumer hardware and are faster for specific tasks.
- Rotary positional embedding (RoPE) enhances the model's ability to handle various input types.
- Grouped query attention design reduces memory usage while processing information efficiently.
- Root mean square layer normalization (RMS Norm) ensures stable training without bias in linear layers.
- Training sequences increased gradually to improve model performance and stability.
- Direct preference optimization (DPO) fine-tunes models using diverse data sets for better conversational performance.
- Open-source availability under Apache 2.0 license encourages community adaptation and improvement.
- Achieving high performance with fewer training tokens demonstrates efficient model design and training techniques.
- Supervised fine-tuning on conversational data sets enhances chat model utility across benchmarks.
- Continuous improvement through community feedback and more complex conversation data is planned.

# QUOTES:
- "H2O danu 1.8B is a language model with 1.8 billion parameters trained on 1 trillion tokens."
- "Despite fewer training tokens, H2O danu 1.8B performs well across a wide range of benchmarks."
- "Advanced language models use decoder attention architecture, benefiting from large pre-training datasets."
- "Smaller models are important for efficiency on consumer hardware and specific tasks."
- "The model architecture includes a hidden size of 2560, intermediate size of 6,912, and 24 hidden layers."
- "Rotary positional embedding (RoPE) helps the model understand sequence positions."
- "Grouped query attention reduces memory usage with 32 attention heads and eight key-value heads."
- "Root mean square layer normalization (RMS Norm) ensures stable training."
- "Training utilized a single node with 8 H100 GPUs employing distributed data parallel (DDP)."
- "Used 8-bit floating point calculations to speed up training with certain layers in FP8 precision."
- "Achieved an average throughput of 292.50 tokens per second on a single node."
- "H2O danu 1.8B is openly available under the Apache 2.0 license."
- "Benchmarks include common sense reasoning, world knowledge, reading comprehension, and overall performance."
- "Outperformed most competitors except for Stable LM2 in some areas."
- "Chat model version trained with supervised fine-tuning on conversational input-output pairs."
- "Direct preference optimization (DPO) used for fine-tuning with various data sets totaling 177,000 samples."
- "Evaluated using Mt Bench for multi-turn questions excluding coding questions."
- "Strong performance in natural language tasks, best in five out of seven categories for single-turn conversations."
- "Weights of both intermediate and final DPO models are available online for community use."

# HABITS:
- Gradually increase training sequences to improve model performance and stability.
- Use rotary positional embedding to enhance the model's ability to handle various input types.
- Employ grouped query attention design to reduce memory usage while processing information efficiently.
- Apply root mean square layer normalization (RMS Norm) for stable training without bias in linear layers.
- Utilize direct preference optimization (DPO) for fine-tuning models using diverse data sets.

# FACTS:
- H2O danu 1.8B is a language model with 1.8 billion parameters trained on 1 trillion tokens.
- The model architecture includes a hidden size of 2560, intermediate size of 6,912, and 24 hidden layers.
- Uses the original Llama 2 tokenizer with a vocabulary size of 32,000 and context length of 16,384 tokens.
- Training utilized a single node with 8 H100 GPUs employing distributed data parallel (DDP).
- Achieved an average throughput of 292.50 tokens per second on a single node.

# REFERENCES:
- Llama 2
- Mistol
- AdamW optimizer
- Apache 2.0 license
- Mt Bench

# ONE-SENTENCE TAKEAWAY
H2O danu 1.8B excels in benchmarks despite fewer training tokens, demonstrating efficient design and open-source accessibility.

# RECOMMENDATIONS:
- Gradually increase training sequences to improve model performance and stability over time.
- Use rotary positional embedding to enhance the model's ability to handle various input types effectively.
- Employ grouped query attention design to reduce memory usage while processing information efficiently.
- Apply root mean square layer normalization (RMS Norm) for stable training without bias in linear layers.
- Utilize direct preference optimization (DPO) for fine-tuning models using diverse data sets effectively.