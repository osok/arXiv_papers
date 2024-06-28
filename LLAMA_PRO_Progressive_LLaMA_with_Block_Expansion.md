# SUMMARY
The introduction of large language models (LLMs) has transformed natural language processing, but they still face limitations in specific domains. This paper proposes a post-pre-training method called block expansion to enhance LLMs' capabilities while preserving their general abilities. The extended model, Llama Pro, demonstrates improved performance in both general and domain-specific tasks, making it versatile for programming, coding, and reasoning.

# IDEAS:
- Large language models (LLMs) have transformed natural language processing but still face domain-specific limitations.
- Enhancing LLMs with specific data strategies demands significant computational resources and large data volumes.
- Domain-adaptive pre-training focuses on post-pre-training with domain-specific data to improve performance.
- Catastrophic forgetting is a challenge in post-pre-training, reducing the model's original general abilities.
- Block expansion is a method to infuse domain-specific knowledge while maintaining general abilities.
- Block expansion involves adding duplicated Transformer blocks initialized to zero for identity mapping.
- Llama Pro is an extended model with 8.3 billion parameters, excelling in programming, coding, and reasoning.
- Llama Pro's expanded blocks are pre-trained on 80 billion tokens using open-source code and math data.
- Supervised instruction tuning (SFT) fine-tunes all blocks of Llama Pro with approximately 80 million tokens.
- Llama Pro Instruct achieves top performance across general code and math tasks.
- Llama Pro Instruct is evaluated as a language agent across various scenarios using GP4 automatic evaluation.
- Block expansion allows the injection of new knowledge while preserving initial capabilities.
- Llama Pro and Llama Pro Instruct integrate natural and programming languages effectively.
- Progressive learning speeds up training by doubling model depth or expanding hidden size features.
- The Llama block consists of multi-head self-attention and a position-wise feed-forward network.
- Block expansion adds identity blocks after each original block to maintain output behavior.
- Identity blocks initialized to zero preserve the output from the initial model during training.
- Block expansion fine-tunes newly added blocks while freezing original blocks to retain general abilities.
- Experiments use code and math datasets for pre-training and multiple data sources for instruction fine-tuning.
- Evaluation includes benchmarks for code-related tasks, general language understanding, and multi-turn interactions.
- Llama Pro outperforms other models in both general and domain-specific tasks after fine-tuning.
- Block expansion training shows superior task-specific adaptability compared to sequential fine-tuning and LoRA.

# INSIGHTS:
- Block expansion enhances LLMs' domain-specific knowledge while preserving general abilities.
- Catastrophic forgetting is a significant challenge in post-pre-training, reducing general performance.
- Llama Pro excels in both general and domain-specific tasks, making it versatile for various applications.
- Progressive learning methods can speed up training by expanding model depth or hidden size features.
- Identity blocks initialized to zero preserve the initial model's output during block expansion training.
- Block expansion fine-tunes only newly added blocks, retaining the original model's general abilities.
- Llama Pro Instruct achieves top performance across a wide range of tasks, including programming and reasoning.
- Evaluation using GP4 automatic scoring shows Llama Pro Instruct's potential as an effective assistant.
- Block expansion training outperforms other strategies in task-specific adaptability and continual learning.
- Adding identity blocks interleaved maintains structural characteristics and improves domain-specific performance.

# QUOTES:
- "Large language models (LLMs) have transformed natural language processing but still face domain-specific limitations."
- "Enhancing LLMs with specific data strategies demands significant computational resources and large data volumes."
- "Domain-adaptive pre-training focuses on post-pre-training with domain-specific data to improve performance."
- "Catastrophic forgetting is a challenge in post-pre-training, reducing the model's original general abilities."
- "Block expansion is a method to infuse domain-specific knowledge while maintaining general abilities."
- "Block expansion involves adding duplicated Transformer blocks initialized to zero for identity mapping."
- "Llama Pro is an extended model with 8.3 billion parameters, excelling in programming, coding, and reasoning."
- "Llama Pro's expanded blocks are pre-trained on 80 billion tokens using open-source code and math data."
- "Supervised instruction tuning (SFT) fine-tunes all blocks of Llama Pro with approximately 80 million tokens."
- "Llama Pro Instruct achieves top performance across general code and math tasks."
- "Llama Pro Instruct is evaluated as a language agent across various scenarios using GP4 automatic evaluation."
- "Block expansion allows the injection of new knowledge while preserving initial capabilities."
- "Llama Pro and Llama Pro Instruct integrate natural and programming languages effectively."
- "Progressive learning speeds up training by doubling model depth or expanding hidden size features."
- "The Llama block consists of multi-head self-attention and a position-wise feed-forward network."
- "Block expansion adds identity blocks after each original block to maintain output behavior."
- "Identity blocks initialized to zero preserve the output from the initial model during training."
- "Block expansion fine-tunes newly added blocks while freezing original blocks to retain general abilities."
- "Experiments use code and math datasets for pre-training and multiple data sources for instruction fine-tuning."
- "Evaluation includes benchmarks for code-related tasks, general language understanding, and multi-turn interactions."

# HABITS:
- Fine-tuning newly added blocks while freezing original blocks to retain general abilities.
- Using multiple data sources for instruction fine-tuning to create comprehensive models.
- Employing progressive learning methods to speed up training by expanding model depth or hidden size features.
- Evaluating models using benchmarks for code-related tasks, general language understanding, and multi-turn interactions.
- Pre-training expanded blocks on large datasets using open-source code and math data.

# FACTS:
- Large language models (LLMs) have transformed natural language processing but still face domain-specific limitations.
- Enhancing LLMs with specific data strategies demands significant computational resources and large data volumes.
- Domain-adaptive pre-training focuses on post-pre-training with domain-specific data to improve performance.
- Catastrophic forgetting is a challenge in post-pre-training, reducing the model's original general abilities.
- Block expansion involves adding duplicated Transformer blocks initialized to zero for identity mapping.

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

# ONE-SENTENCE TAKEAWAY
Block expansion enhances large language models' domain-specific knowledge while preserving their general abilities.

# RECOMMENDATIONS:
- Use block expansion to enhance LLMs' domain-specific knowledge while preserving general abilities.
- Fine-tune newly added blocks while freezing original blocks to retain general abilities.
- Employ progressive learning methods to speed up training by expanding model depth or hidden size features.
- Evaluate models using benchmarks for code-related tasks, general language understanding, and multi-turn interactions.
- Pre-train expanded blocks on large datasets using open-source code and math data.