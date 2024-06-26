# SUMMARY
Adam Mini aims to reduce high memory consumption in training large language models by optimizing Adam's second-order momentum component, improving efficiency and performance.

# IDEAS:
- Adam Mini reduces memory requirements of Adam's second-order momentum component in large language model training.
- It cuts down the number of learning rates used, alleviating CPU offloading and parameter sharding.
- Reduces communication overhead among GPUs and CPUs, lowering the threshold for training large models.
- Encourages researchers with limited GPU resources to participate in training large models.
- Maintains or improves Adam's performance while drastically reducing memory usage.
- Partitions model parameters into blocks based on the Hessian structure for Transformers.
- Assigns a single learning rate to each parameter block outside the embedding layer.
- Uses the mean of Adam's second-order values to determine learning rates for each block.
- Ensures different heads receive distinct learning rates by partitioning based on the smallest dense subblock in the Hessian.
- Achieves significant memory savings, up to 45% to 50% of Adam's memory cost.
- Higher throughput due to reduced communication among CPUs and GPUs and absence of extra computation.
- Potential for further optimization in learning rate design through fine-grained analysis of each dense Hessian subblock.
- Shows low sensitivity to hyperparameters, ensuring robust performance across different settings.
- Validated through experiments on various tasks including pre-training, supervised fine-tuning, and reinforcement learning.
- Tested on non-language model tasks like training diffusion models, vision models, and graph neural networks.
- Achieved comparable or better performance than Adam W on various tasks.
- Saved 33.1% wall clock time during pre-training LLaMA 2 7B on 6 A100-80GB GPUs.
- Demonstrated effectiveness, efficiency, and memory optimization compared to Adam W.
- Does not address memory consumption of Adam's first-order momentum component.
- Focuses primarily on reducing memory usage of Adam's second-order momentum component.

# INSIGHTS:
- Adam Mini significantly reduces memory usage without compromising performance in large language model training.
- Encourages broader participation in training large models by lowering resource requirements.
- Optimizes learning rate assignment by partitioning model parameters into blocks based on Hessian structure.
- Achieves higher throughput by reducing communication overhead among CPUs and GPUs.
- Shows potential for further optimization through fine-grained analysis of dense Hessian subblocks.

# QUOTES:
- "Adam Mini aims to solve the problem of high memory consumption in training large language models."
- "Significantly cutting down the number of learning rates used in Adam Mini aims to alleviate the need for CPU offloading."
- "Adam Mini reduces the number of learning rates used in Adam, especially for Transformers."
- "Adam Mini can achieve higher throughput than Adam W due to reduced communication among CPUs and GPUs."
- "Adam Mini shows low sensitivity to hyperparameters, ensuring robust performance across different settings."
- "Adam Mini was validated and tested through a series of experiments on various tasks."
- "Adam Mini achieved comparable or even better performance than Adam W on various language models."
- "Adam Mini reached better performance on non-language model tasks such as training diffusion models."
- "Adam Mini significantly reduced the memory cost of Adam, cutting down 45% to 50% of the memory required."
- "Adam Mini demonstrated effectiveness, efficiency, and memory optimization compared to Adam W."

# HABITS:
- Partition model parameters into blocks based on Hessian structure for efficient learning rate assignment.
- Use mean values of second-order momentum components to determine learning rates for parameter blocks.
- Conduct fine-grained analysis of dense Hessian subblocks for potential optimization in learning rate design.
- Validate new methods through extensive experiments on various tasks including pre-training and fine-tuning.

# FACTS:
- Adam Mini reduces memory requirements by up to 45% to 50% compared to Adam.
- Achieved higher throughput than Adam W, saving 33.1% wall clock time during pre-training LLaMA 2 7B.
- Validated through experiments on mainstream English corpus and various non-language model tasks.
- Demonstrated comparable or better performance than Adam W on tasks like training diffusion models and vision models.

# REFERENCES:
- GPT2 series
- LLaMA series
- AdaFactor
- SM3
- ResNet18
- ImageNet
- CelebA
- Graph Convolution Network (GCN)
- Graph Attention Network (GAT)
- OGB archive

# ONE-SENTENCE TAKEAWAY
Adam Mini optimizes memory usage in large language model training, enabling broader participation and improved efficiency.

# RECOMMENDATIONS:
- Reduce the number of learning rates used in optimizers to save memory resources.
- Partition model parameters into blocks based on Hessian structure for efficient learning rate assignment.
- Use mean values of second-order momentum components to determine learning rates for parameter blocks.
- Conduct fine-grained analysis of dense Hessian subblocks for potential optimization in learning rate design.
- Validate new methods through extensive experiments on various tasks including pre-training and fine-tuning.