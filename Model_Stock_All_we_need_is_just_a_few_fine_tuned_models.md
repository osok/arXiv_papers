# SUMMARY
The section discusses the dynamics of fine-tuned weights, revealing that averaging weights closer together improves model performance. A new method, Model Stock, efficiently merges weights from a few fine-tuned models, achieving high performance with lower computational costs.

# IDEAS:
- Fine-tuned weights with different random seeds cluster closely in weight space.
- Averaging weights improves model performance on both ImageNet and distribution shift benchmarks.
- Model Stock efficiently merges weights from a few fine-tuned models.
- Leveraging geometric properties of weight space and pre-trained model anchoring enhances performance.
- Model Stock outperforms Model Soup in computational costs while achieving comparable or better results.
- Fine-tuned model weights form a thin shell layer-wise in weight space.
- Being closer to the center of this shell benefits model performance.
- Consistent angle and norm values among fine-tuned weights across various setups.
- Fine-tuned weights closer to the center exhibit improved performance.
- Randomly perturbed weights near the center also merit high performance.
- Fine-tuned weights follow a Gaussian distribution.
- Model Stock leverages pre-trained models to approximate the weight center.
- Bias layers rely more on fine-tuned models, while weight layers depend on pre-trained models.
- Periodic merging during training improves model performance.
- Model Stock achieves state-of-the-art performance on ImageNet with various CLIP models.
- Model Stock shows competitive performance with Model Soup using fewer models.
- Model Stock exhibits exceptional performance on ImageNet accuracy and robustness across distribution shifts.
- Ablation studies confirm Model Stock's efficiency and effectiveness.
- Increasing the number of merging models improves performance and moves weights closer to the center.
- Post-training merging strategy for Model Stock achieves improved distribution shift scores.
- Proximity to the center of the weight distribution is crucial for enhancing performance.
- Wise FT combines weights of pre-trained and fine-tuned models linearly for significant accuracy gains.
- Model Soup merges weights from various fine-tuned models trained with different hyperparameters.
- Weight vectors' interpolation reduces variance, contributing to performance gains.

# INSIGHTS:
- Fine-tuned weights cluster closely in weight space, forming a thin shell layer-wise.
- Averaging weights closer together improves model performance on various benchmarks.
- Model Stock efficiently merges weights, leveraging geometric properties and pre-trained model anchoring.
- Proximity to the center of the weight distribution is crucial for model performance.
- Consistent angle and norm values among fine-tuned weights indicate a general pattern in weight distributions.
- Randomly perturbed weights near the center exhibit high performance, emphasizing center proximity's importance.
- Fine-tuned weights follow a Gaussian distribution, explaining their geometric patterns.
- Periodic merging during training continuously approximates the weight center, improving performance.
- Model Stock achieves state-of-the-art performance with fewer models compared to Model Soup.
- Weight vectors' interpolation reduces variance, enhancing performance in weight ensemble methods.

# QUOTES:
- "Fine-tuned weights with different random seeds cluster closely in weight space."
- "Averaging these weights improves model performance on both ImageNet and distribution shift benchmarks."
- "Model Stock efficiently merges weights from a few fine-tuned models."
- "Leveraging geometric properties of weight space and pre-trained model anchoring enhances performance."
- "Model Stock outperforms Model Soup in computational costs while achieving comparable or better results."
- "Fine-tuned model weights form a thin shell layer-wise in weight space."
- "Being closer to the center of this shell benefits model performance."
- "Consistent angle and norm values among fine-tuned weights across various setups."
- "Fine-tuned weights closer to the center exhibit improved performance."
- "Randomly perturbed weights near the center also merit high performance."
- "Fine-tuned weights follow a Gaussian distribution."
- "Model Stock leverages pre-trained models to approximate the weight center."
- "Bias layers rely more on fine-tuned models, while weight layers depend on pre-trained models."
- "Periodic merging during training improves model performance."
- "Model Stock achieves state-of-the-art performance on ImageNet with various CLIP models."
- "Model Stock shows competitive performance with Model Soup using fewer models."
- "Model Stock exhibits exceptional performance on ImageNet accuracy and robustness across distribution shifts."
- "Ablation studies confirm Model Stock's efficiency and effectiveness."
- "Increasing the number of merging models improves performance and moves weights closer to the center."
- "Post-training merging strategy for Model Stock achieves improved distribution shift scores."

# HABITS:
- Periodically merge weights during training to continuously approximate the weight center.
- Leverage pre-trained models to approximate the weight center more accurately.
- Use fewer fine-tuned models for efficient weight merging without extra training or heuristic settings.

# FACTS:
- Fine-tuned weights with different random seeds cluster closely in weight space.
- Averaging these weights improves model performance on both ImageNet and distribution shift benchmarks.
- Model Stock efficiently merges weights from a few fine-tuned models.
- Leveraging geometric properties of weight space and pre-trained model anchoring enhances performance.
- Fine-tuned model weights form a thin shell layer-wise in weight space.
- Consistent angle and norm values among fine-tuned weights across various setups indicate a general pattern in weight distributions.
- Randomly perturbed weights near the center exhibit high performance, emphasizing center proximity's importance.
- Fine-tuned weights follow a Gaussian distribution, explaining their geometric patterns.

# REFERENCES:
- CLIP ViT B32
- CLIP ViT B16
- CLIP ViT L14
- ImageNet 1K dataset
- Model Soup
- Wise FT

# ONE-SENTENCE TAKEAWAY
Proximity to the center of weight distribution is crucial for enhancing model performance efficiently.

# RECOMMENDATIONS:
- Periodically merge weights during training to continuously approximate the weight center.
- Leverage pre-trained models to approximate the weight center more accurately.
- Use fewer fine-tuned models for efficient weight merging without extra training or heuristic settings.