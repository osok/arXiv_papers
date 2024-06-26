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
- PFT methods keep most base model parameters fixed, fine-tuning a small subset.
- Adapter method inserts a small feed-forward module after each multi-head attention layer.
- Prompt tuning adds trainable soft tokens to input embeddings, reducing trainable parameters.
- LoRA limits weight matrix updates to a low-rank subspace, enhancing efficiency.
- LoRA outperforms prompt tuning for single downstream datasets.
- S-LoRA uses LoRA-based experts for each new dataset, unlike S-prompts.
- Learning to prompt (L2P) uses a fixed pool of prompts shared across datasets.
- Learning to LoRA (L2L) combines LoRA modules additively using weight matrices.
- Experiments compared S-prompts and L2P with their LoRA-based variants on benchmarks.
- Benchmarks included Core 50, DomainNet, Split CIFAR100, and Split Tiny ImageNet.
- ViT-B16 model pre-trained on ImageNet-21k was used for fair comparison.
- Memory-free methods like EWC and LwF were employed in experiments.
- LoRA variants outperformed prompt tuning variants across different benchmarks.
- Expert selection is more crucial for LoRA-based methods than for S-prompts.
- SX Plus+ updates the feature extractor on data from the first task, improving performance.
- Sharing the classification layer led to higher average accuracy in experiments.
- Fine-tuning for continual learning can lead to catastrophic forgetting.
- Regularization terms or adding new parameters can address catastrophic forgetting.
- Transformer models have a significant impact on continual learning.

# INSIGHTS:
- Continual learning efficiently updates models without retraining from scratch each time.
- Parameter-efficient fine-tuning makes large-scale models accessible on less powerful hardware.
- LoRA's low-rank subspace updates enhance Transformer model efficiency significantly.
- S-LoRA and L2L combine LoRA with existing algorithms for better continual learning.
- Expert selection is critical for LoRA-based methods in class incremental problems.

# QUOTES:
- "Continual learning means training machine learning models on a sequence of data sets."
- "Joint training is considered the best in terms of performance."
- "Parameter efficient fine-tuning methods involve keeping most of the parameters of a base model fixed."
- "Prompt tuning introduces trainable soft tokens in the input embedding space."
- "LoRA limits the update of a weight matrix to a low-rank subspace."
- "LoRA outperforms prompt tuning significantly for a single downstream data set."
- "S-LoRA does not require prompt tuning; instead, we use LoRA-based experts."
- "We conducted experiments comparing S-prompts and L2P with their LoRA-based variant."
- "LoRA variants outperformed prompt tuning variants across different benchmarks."
- "Expert selection is more crucial for LoRA-based methods like S-LoRA than for S-prompts."

# HABITS:
- Conducting experiments on Amazon EC2 G5 instances with Nvidia A10G Tensor Core GPU.
- Allocating new LoRA modules and output heads for each new dataset in S-LoRA.
- Using memory-free methods like EWC and LwF in continual learning experiments.

# FACTS:
- Continual learning trains models on sequential datasets without forgetting past knowledge.
- Joint training starts from scratch on each dataset, offering the best performance.
- Vision Transformer (ViT) is known for strong feature representations in vision tasks.
- Adapter method inserts a small feed-forward module after each multi-head attention layer.
- LoRA limits weight matrix updates to a low-rank subspace, enhancing efficiency.

# REFERENCES:
- Vision Transformer (ViT)
- Core 50
- DomainNet
- Split CIFAR100
- Split Tiny ImageNet
- ImageNet-21k
- EWC (Elastic Weight Consolidation)
- LwF (Learning without Forgetting)

# ONE-SENTENCE TAKEAWAY
LoRA-based methods significantly enhance efficiency and performance in continual learning scenarios compared to prompt tuning.

# RECOMMENDATIONS:
- Use parameter-efficient fine-tuning to adapt large-scale models on less powerful hardware.
- Employ LoRA for efficient weight matrix updates in Transformer models.
- Combine LoRA with existing algorithms for better continual learning performance.
- Focus on expert selection in class incremental problems for LoRA-based methods.