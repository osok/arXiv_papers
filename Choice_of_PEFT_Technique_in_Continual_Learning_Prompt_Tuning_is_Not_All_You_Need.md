# SUMMARY
The paper discusses continual learning and parameter-efficient fine-tuning (PFT) for Transformers, focusing on methods like prompt tuning and low-rank adaptation (LoRA).

# IDEAS:
- Continual learning trains models on sequential datasets without forgetting past knowledge.
- Joint training starts from scratch on each dataset, offering the best performance.
- Continual learning aims to match joint training performance without inefficiency.
- Class incremental learning introduces new classes with each dataset.
- Domain incremental learning changes data distribution while keeping labels fixed.
- Parameter-efficient fine-tuning (PFT) methods reduce resource intensity in fine-tuning Transformers.
- Vision Transformer (ViT) is known for strong feature representations in vision tasks.
- Prompt tuning adds trainable soft tokens to input embeddings, reducing trainable parameters.
- LoRA limits weight matrix updates to a low-rank subspace, enhancing efficiency.
- LoRA outperforms prompt tuning for single downstream datasets.
- S-LoRA uses LoRA-based experts for each new dataset, unlike S-prompts.
- Learning to prompt (L2P) uses a fixed pool of prompts shared across datasets.
- Learning to LoRA (L2L) uses a pool of LoRA modules selected via key-based retrieval.
- Experiments compared S-prompts and L2P with their LoRA-based variants on benchmarks.
- Benchmarks included Core 50, DomainNet, Split CIFAR100, and Split Tiny ImageNet.
- Experiments used a ViT-B16 model pre-trained on ImageNet-21k.
- Performance was evaluated using the micro-average of all datasets.
- Hyperparameters included prompt length for prompt-based methods and rank for LoRA-based methods.
- Amazon EC2 G5 instances with Nvidia A10G GPUs were used for experiments.
- LoRA variants outperformed prompt tuning variants across different benchmarks.
- Expert selection is more crucial for LoRA-based methods than for S-prompts.
- SX Plus+ updates the feature extractor on data from the first task, improving performance.
- Sharing the classification layer led to higher average accuracy in L2X methods.
- Fine-tuning for continual learning can lead to catastrophic forgetting.
- Regularization terms or adding new parameters can address catastrophic forgetting.
- Memory-free methods were the focus of the study.

# INSIGHTS:
- Continual learning efficiently updates models without retraining from scratch.
- Parameter-efficient fine-tuning makes large-scale models accessible on less powerful hardware.
- LoRA's low-rank subspace updates enhance Transformer model efficiency.
- S-LoRA and L2L combine LoRA with existing algorithms for better performance.
- Expert selection is critical for LoRA-based methods in class incremental problems.

# QUOTES:
- "Continual learning means training machine learning models on a sequence of data sets."
- "Joint training is considered the best in terms of performance."
- "Parameter efficient fine-tuning methods have been developed to address resource intensity."
- "Prompt tuning introduces trainable soft tokens in the input embedding space."
- "LoRA limits the update of a weight matrix to a low-rank subspace."
- "LoRA outperforms prompt tuning significantly for a single downstream data set."
- "S-LoRA does not require prompt tuning; instead, we use LoRA-based experts."
- "We conducted experiments comparing S-prompts and L2P with their LoRA-based variants."
- "LoRA variants outperformed prompt tuning variants across different benchmarks."
- "Expert selection is more crucial for LoRA-based methods like S-LoRA."

# HABITS:
- Conducting experiments on Amazon EC2 G5 instances with Nvidia A10G GPUs.
- Using pre-trained models like ViT-B16 on ImageNet-21k for fair comparison.
- Evaluating performance using the micro-average of all datasets.

# FACTS:
- Continual learning involves training models on sequential datasets without forgetting past knowledge.
- Joint training starts from scratch on each dataset, offering the best performance.
- Vision Transformer (ViT) is known for strong feature representations in vision tasks.
- Prompt tuning adds trainable soft tokens to input embeddings, reducing trainable parameters.
- LoRA limits weight matrix updates to a low-rank subspace, enhancing efficiency.

# REFERENCES:
- Vision Transformer (ViT)
- ImageNet-21k
- Core 50
- DomainNet
- Split CIFAR100
- Split Tiny ImageNet
- Amazon EC2 G5 instances
- Nvidia A10G GPUs

# ONE-SENTENCE TAKEAWAY
LoRA-based methods significantly enhance efficiency and performance in continual learning scenarios compared to prompt tuning.

# RECOMMENDATIONS:
- Use LoRA for efficient Transformer model fine-tuning in resource-constrained environments.
- Apply continual learning to maintain model performance without retraining from scratch.
- Consider expert selection methods crucial for class incremental problems in LoRA-based approaches.