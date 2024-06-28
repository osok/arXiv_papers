# SUMMARY
The introduction of large language models (LLMs) has transformed natural language processing, but they still face limitations in specific domains. This paper proposes a post-pre-training method called block expansion to enhance LLMs' capabilities without excessive computational resources. The method involves adding new Transformer blocks to pre-trained LLMs, preserving their general abilities while improving domain-specific performance. The extended model, Llama Pro, demonstrates enhanced performance in general and domain-specific tasks, making it versatile for programming, coding, and reasoning.

# IDEAS:
- Block expansion adds new Transformer blocks to pre-trained LLMs, preserving general abilities.
- Llama Pro excels in both general and domain-specific tasks like programming and reasoning.
- Domain adaptive pre-training focuses on post-pre-training with domain-specific data.
- Catastrophic forgetting is a challenge in post-pre-training, reducing general abilities.
- Block expansion method enlarges pre-trained LLM using duplicated Transformer blocks.
- Newly added blocks are fine-tuned with domain-specific data, keeping original blocks unchanged.
- Llama Pro instruct achieves top performance across general code and math tasks.
- Llama Pro instruct evaluated as a language agent across various scenarios.
- Comprehensive experimental results show Llama Pro instruct outperforms other Llama family models.
- Progressive learning speeds up training of large-scale models in computer vision and NLP.
- Depth growth maintains overall performance while adapting to specific domains.
- Multi-head self-attention mechanism is key in the Transformer model.
- Identity block ensures expanded model maintains same output after expansion.
- Block expansion increases model depth while maintaining output behavior.
- Fine-tuning newly added blocks preserves general abilities of the model.
- Pre-training on code and math data sets enhances model's capacity for domain knowledge.
- Flash attention mechanism speeds up training process.
- Evaluation includes benchmarks for code-related tasks and general language understanding.
- Llama Pro shows strong general performance along with coding capabilities.
- Supervised fine-tuning adapts expansion strategy to traditional training pipeline.
- Mint bench evaluates multi-turn interactions using tools and natural language feedback.
- Block expansion training shows superior task-specific adaptability compared to other strategies.
- Adding blocks interleaved provides optimal performance with minimal cost.
- Position of identity blocks impacts evaluation performance and domain-specific tasks.
- Llama Pro consistently outperforms base model across all tasks.

# INSIGHTS:
- Block expansion enhances LLMs without sacrificing general abilities or requiring excessive resources.
- Catastrophic forgetting remains a significant challenge in post-pre-training methods.
- Depth growth in progressive learning maintains overall performance while adapting to specific domains.
- Identity blocks ensure expanded models maintain output behavior during block expansion.
- Fine-tuning only newly added blocks preserves the general abilities of the original model.
- Flash attention mechanism significantly speeds up the training process for large-scale models.
- Comprehensive evaluation benchmarks are crucial for assessing LLMs' performance across various tasks.
- Supervised fine-tuning adapts well to the block expansion strategy, enhancing model capabilities.
- Mint bench provides valuable insights into multi-turn interactions and tool usage in LLMs.
- Positioning of identity blocks affects both general and domain-specific task performance.

# QUOTES:
- "Block expansion adds new Transformer blocks to pre-trained LLMs, preserving general abilities."
- "Llama Pro excels in both general and domain-specific tasks like programming and reasoning."
- "Domain adaptive pre-training focuses on post-pre-training with domain-specific data."
- "Catastrophic forgetting is a challenge in post-pre-training, reducing general abilities."
- "Block expansion method enlarges pre-trained LLM using duplicated Transformer blocks."
- "Newly added blocks are fine-tuned with domain-specific data, keeping original blocks unchanged."
- "Llama Pro instruct achieves top performance across general code and math tasks."
- "Llama Pro instruct evaluated as a language agent across various scenarios."
- "Comprehensive experimental results show Llama Pro instruct outperforms other Llama family models."
- "Progressive learning speeds up training of large-scale models in computer vision and NLP."
- "Depth growth maintains overall performance while adapting to specific domains."
- "Multi-head self-attention mechanism is key in the Transformer model."
- "Identity block ensures expanded model maintains same output after expansion."
- "Block expansion increases model depth while maintaining output behavior."
- "Fine-tuning newly added blocks preserves general abilities of the model."
- "Pre-training on code and math data sets enhances model's capacity for domain knowledge."
- "Flash attention mechanism speeds up training process."
- "Evaluation includes benchmarks for code-related tasks and general language understanding."
- "Llama Pro shows strong general performance along with coding capabilities."
- "Supervised fine-tuning adapts expansion strategy to traditional training pipeline."

# HABITS:
- Fine-tuning only newly added blocks while freezing original blocks preserves general abilities.
- Using flash attention mechanism to speed up the training process for large-scale models.
- Combining multiple data sources to create comprehensive instruction datasets for fine-tuning.
- Evaluating models using a wide range of benchmarks for thorough performance assessment.
- Employing depth growth to maintain overall performance while adapting to specific domains.

# FACTS:
- Block expansion adds new Transformer blocks to pre-trained LLMs, preserving general abilities.
- Catastrophic forgetting is a challenge in post-pre-training, reducing general abilities.
- Flash attention mechanism significantly speeds up the training process for large-scale models.
- Comprehensive evaluation benchmarks are crucial for assessing LLMs' performance across various tasks.
- Positioning of identity blocks affects both general and domain-specific task performance.

# REFERENCES:
- Llama 2
- Code LLaMA
- Stack Dup dataset
- Proof Pile 2 dataset
- Shared GPT
- Wizard LM Evolution instruction dataset
- Evolution Code Alpaca dataset
- Metamath
- Open Orca dataset
- AI2 Reasoning Challenge
- H Swag
- MML
- Truthful QA
- WinR
- GSM 8K
- Program of Thought (PoT) setting
- Human Eval
- MBPP

# ONE-SENTENCE TAKEAWAY
Block expansion enhances large language models' capabilities without sacrificing general abilities or requiring excessive resources.

# RECOMMENDATIONS:
- Use block expansion to enhance LLMs without sacrificing general abilities or requiring excessive resources.
- Fine-tune only newly added blocks while freezing original blocks to preserve general abilities.
- Employ flash attention mechanism to speed up the training process for large-scale models.
- Combine multiple data sources to create comprehensive instruction datasets for fine-tuning.
- Evaluate models using a wide range of benchmarks for thorough performance assessment.