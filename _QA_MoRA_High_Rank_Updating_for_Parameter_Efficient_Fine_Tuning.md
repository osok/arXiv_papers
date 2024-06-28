# SUMMARY
The proposed method, Mora, aims to solve limitations in low-rank updating in existing PFT methods like Laura, enhancing LLMs' memory and fine-tuning capabilities.

# IDEAS:
- Mora addresses low-rank updating limitations in existing PFT methods like Laura.
- Mora enhances LLMs' memory and fine-tuning capabilities.
- Laura struggles with estimating full-rank updates due to reliance on low-rank matrices.
- Mora employs a square matrix instead of low-rank matrices for high-rank updating.
- Mora maintains the same number of trainable parameters while maximizing rank in weight update matrix Delta W.
- Mora introduces non-parameter operators to reduce input dimensions and increase output dimensions.
- Mora ensures seamless integration back into LLMs like Laura.
- Mora improves performance on memory-intensive tasks by enabling high-rank updating.
- Mora utilizes a square matrix M with dimensions hat R * hat R.
- Non-parameterized operators fcor text comp and fcor text de comp operate in linear time.
- Laura employs two low-rank matrices A and B with D plus g r total trainable parameters.
- Mora's square matrix allows for higher rank updating compared to Laura.
- Mora's compression and decompression functions efficiently increase the rank of Delta W.
- Mora outperformed Laura in memorizing new knowledge in experiments.
- Mora demonstrated comparable performance to Laura in instruction tuning and mathematical reasoning.
- Mora surpassed Laura in biomed and financial domains for continual pre-training.
- Mora showed better performance compared to Laura and rora in pre-training experiments.
- Mora's learned weight updates had a higher number of significant singular values.
- Rotation was identified as the most efficient method for distinguishing input information in Mora.
- Mora achieved significant improvements across different tasks compared to Laura.
- Mora showed better performance in memorizing UUID pairs than Laura.
- Mora demonstrated similar performance to Laura in instruction tuning tasks.
- Mora showed better performance than Laura in mathematical reasoning tasks.
- Mora surpassed Laura in biomedic and financial domains for continual pre-training.
- Mora demonstrated superior performance compared to Laura and rora in pre-training on C4 datasets.
- Mora struggles in memorizing new knowledge compared to FFT even with a large rank.
- Mora performed significantly worse than FFT in a memorization task using pseudo data.
- Mora shows similar performance to Laura in instruction tuning tasks but falls short in mathematical reasoning and continual pre-training.
- Increasing the rank from 8 to 256 in Mora can help bridge the performance gap with FFT.
- Certain methods of compression like truncation can lead to significant information loss in Mora.
- Sharing rows and columns can preserve more input information but may not be efficient for smaller ranks like eight.
- Different fine-tuning tasks have varying requirements for capabilities.

# INSIGHTS:
- Mora enhances LLMs' memory and fine-tuning by addressing low-rank updating limitations.
- Employing a square matrix allows Mora to achieve high-rank updating efficiently.
- Non-parameter operators ensure seamless integration of Mora into existing LLMs.
- High-rank updating improves performance on memory-intensive tasks significantly.
- Compression and decompression functions are crucial for increasing the rank of Delta W in Mora.
- Experiments show Mora outperforms Laura in memorizing new knowledge and continual pre-training.
- Rotation is the most efficient method for distinguishing input information in Mora.
- Different fine-tuning tasks require varying capabilities, impacting Mora's effectiveness.
- Information loss during compression can affect Mora's performance, especially with smaller ranks.
- Increasing the rank from 8 to 256 helps bridge the performance gap with FFT.

# QUOTES:
- "Mora addresses the challenge faced by Laura in handling tasks that require enhancing knowledge."
- "Laura struggles with estimating full-rank updates due to its reliance on low-rank matrices."
- "Mora employs a square matrix instead of low-rank matrices aiming to achieve high-rank updating."
- "Mora introduces non-parameter operators to reduce input dimensions and increase output dimensions."
- "Mora ensures seamless integration back into LLMs like Laura."
- "Mora aims to improve the performance of PFT methods on memory-intensive tasks."
- "Mora utilizes a square matrix M with dimensions hat R * hat R."
- "Non-parameterized operators fcor text comp and fcor text de comp operate in linear time."
- "Laura employs two low-rank matrices A and B with D plus g r total trainable parameters."
- "Mora's square matrix allows for higher rank updating compared to Laura."
- "Mora's compression and decompression functions efficiently increase the rank of Delta W."
- "Mora outperformed Laura in memorizing new knowledge in experiments."
- "Mora demonstrated comparable performance to Laura in instruction tuning and mathematical reasoning."
- "Mora surpassed Laura in biomed and financial domains for continual pre-training."
- "Mora showed better performance compared to Laura and rora in pre-training experiments."
- "Mora's learned weight updates had a higher number of significant singular values."
- "Rotation was identified as the most efficient method for distinguishing input information in Mora."
- "Mora achieved significant improvements across different tasks compared to Laura."
- "Mora showed better performance in memorizing UUID pairs than Laura."
- "Mora demonstrated similar performance to Laura in instruction tuning tasks."

# HABITS:
N/A

# FACTS:
N/A

# REFERENCES:
N/A

# ONE-SENTENCE TAKEAWAY
Mora enhances LLMs' memory and fine-tuning by addressing low-rank updating limitations through high-rank updating capabilities.

# RECOMMENDATIONS:
- Employ a square matrix instead of low-rank matrices for high-rank updating efficiency.
- Use non-parameter operators to reduce input dimensions and increase output dimensions seamlessly.
- Utilize compression and decompression functions to efficiently increase the rank of Delta W.
- Consider rotation as the most efficient method for distinguishing input information.
- Increase the rank from 8 to 256 to bridge the performance gap with FFT.