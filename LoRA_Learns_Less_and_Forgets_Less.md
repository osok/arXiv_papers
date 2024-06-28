# SUMMARY
The text compares LoRA and full fine-tuning for LLaMA models in code and math tasks, analyzing performance, forgetting, and regularization.

# IDEAS:
- LoRA falls short in code tasks compared to full fine-tuning but narrows the gap in math tasks.
- LoRA better preserves source domain performance than full fine-tuning.
- Full fine-tuning induces high-rank perturbations to the base model's weight matrices.
- LoRA offers stronger regularization compared to traditional methods like dropout and weight decay.
- LoRA maintains a diversity of solutions compared to the limited set produced by full fine-tuning.
- LoRA's performance is highly influenced by learning rates and the selection of target modules.
- LoRA can save memory and enable efficient multi-tenant serving by sharing a base model across users.
- Instruction fine-tuning leads to more significant improvements compared to continued pre-training.
- LoRA tends to underperform full fine-tuning, especially in programming tasks.
- LoRA forgets less than full fine-tuning, especially in programming tasks.
- LoRA achieves higher source domain performance for similar target domain performance in some cases.
- LoRA proves to be a more effective regularizer leading to less learning and forgetting.
- Low-rank training can approximate full fine-tuning in coding and math tasks.
- Full fine-tuning does not necessarily learn low-rank perturbations.
- The rank of perturbations increases with more training data and varies across module types and layers.
- The choice of target modules is more crucial than the rank in LoRA.
- Targeting all modules yielded better results compared to MLP and attention modules.
- Selecting a relatively low rank such as r=16 while targeting all modules strikes a good balance.
- Continual learning on a new domain may lead to a trade-off in performance on the original domain.
- Strategies like replaying source domain data during continual learning can help mitigate forgetting.

# INSIGHTS:
- LoRA narrows the performance gap in math tasks with longer training but falls short in code tasks.
- Full fine-tuning induces high-rank perturbations, while LoRA assumes low-rank perturbations.
- LoRA offers stronger regularization and maintains solution diversity compared to full fine-tuning.
- Learning rates and target module selection significantly impact LoRA's performance.
- Instruction fine-tuning leads to more significant improvements than continued pre-training.
- LoRA forgets less than full fine-tuning, especially in programming tasks.
- Low-rank training can approximate full fine-tuning in coding and math tasks.
- The choice of target modules is more crucial than the rank in LoRA.
- Continual learning on a new domain may lead to a trade-off in original domain performance.
- Replaying source domain data during continual learning can help mitigate forgetting.

# QUOTES:
- "LoRA falls short in code tasks compared to full fine-tuning but narrows the gap in math tasks."
- "LoRA better preserves source domain performance than full fine-tuning."
- "Full fine-tuning induces high-rank perturbations to the base model's weight matrices."
- "LoRA offers stronger regularization compared to traditional methods like dropout and weight decay."
- "LoRA maintains a diversity of solutions compared to the limited set produced by full fine-tuning."
- "LoRA's performance is highly influenced by learning rates and the selection of target modules."
- "LoRA can save memory and enable efficient multi-tenant serving by sharing a base model across users."
- "Instruction fine-tuning leads to more significant improvements compared to continued pre-training."
- "LoRA tends to underperform full fine-tuning, especially in programming tasks."
- "LoRA forgets less than full fine-tuning, especially in programming tasks."
- "LoRA achieves higher source domain performance for similar target domain performance in some cases."
- "LoRA proves to be a more effective regularizer leading to less learning and forgetting."
- "Low-rank training can approximate full fine-tuning in coding and math tasks."
- "Full fine-tuning does not necessarily learn low-rank perturbations."
- "The rank of perturbations increases with more training data and varies across module types and layers."
- "The choice of target modules is more crucial than the rank in LoRA."
- "Targeting all modules yielded better results compared to MLP and attention modules."
- "Selecting a relatively low rank such as r=16 while targeting all modules strikes a good balance."
- "Continual learning on a new domain may lead to a trade-off in performance on the original domain."
- "Strategies like replaying source domain data during continual learning can help mitigate forgetting."

# HABITS:
- Conduct thorough learning rate sweeps for each method before training.
- Target all modules rather than just MLP or attention modules for better results.
- Select a relatively low rank such as r=16 while targeting all modules for balance.
- Replay source domain data during continual learning to mitigate forgetting.

# FACTS:
- LoRA falls short in code tasks but narrows the gap in math tasks with longer training.
- Full fine-tuning induces high-rank perturbations, while LoRA assumes low-rank perturbations.
- Instruction fine-tuning leads to more significant improvements than continued pre-training.
- LoRA forgets less than full fine-tuning, especially in programming tasks.
- Low-rank training can approximate full fine-tuning in coding and math tasks.

# REFERENCES:
- LLaMA models
- HumanEval benchmark
- GSM 8K benchmark
- Coding Captain dataset
- StarCoder dataset
- Python Math dataset
- Open Web Math dataset
- If Magicater dataset
- Evel Instruct 110K dataset
- Metamath QA dataset

# ONE-SENTENCE TAKEAWAY
LoRA offers strong regularization and memory efficiency but underperforms full fine-tuning, especially in code tasks.

# RECOMMENDATIONS:
- Use LoRA for improved fine-tuning if instead of Captain for better results.
- Identify the highest stable learning rate for optimal LoRA performance.
- Target all modules rather than just MLP or attention modules for better results.
- Select a relatively low rank such as r=16 while targeting all modules for balance.
- Replay source domain data during continual learning to mitigate forgetting.