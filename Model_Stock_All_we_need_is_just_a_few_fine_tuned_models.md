# SUMMARY
The section discusses the dynamics of fine-tuned weights, revealing that averaging weights closer together improves model performance. A new method, Model Stock, efficiently merges weights from a few fine-tuned models, achieving high performance with lower computational costs.

# IDEAS:
- Fine-tuned weights with different random seeds form a thin shell layer-wise in weight space.
- Averaging weights closer together leads to better performance on both in-distribution and out-of-distribution tasks.
- Model Stock merges weights from a few fine-tuned models using geometric properties of weight space.
- Model Stock is more computationally efficient than Model Soup while achieving comparable or better results.
- Fine-tuned weights' norms and angles are consistent across various setups and training stages.
- Fine-tuned weights closer to the center exhibit improved performance on both in-distribution and out-of-distribution datasets.
- Fine-tuned weights tend to occupy local minima edges in the test error landscape.
- Randomly perturbed weights near the center also show high performance.
- Fine-tuned weights follow a Gaussian distribution, explaining their geometric patterns.
- Model Stock leverages pre-trained models to approximate the weight center by interpolating between pre-trained and fine-tuned models.
- Bias layers rely more on fine-tuned models, while weight layers depend on pre-trained models.
- Periodic merging during training improves model performance and brings weights closer to the center.
- Model Stock does not require extra training or heuristic hyperparameter settings, simplifying the process.
- Model Stock achieves state-of-the-art performance on ImageNet with various CLIP ViT models.
- Model Stock outperforms Model Soup while using only two models, showcasing its efficiency.
- Model Stock exhibits exceptional performance on ImageNet accuracy and robustness across various distribution shift scenarios.
- Ablation studies show that Model Stock performs well across different merging periods and post-training merging strategies.
- Proximity to the center of the weight distribution is crucial for enhancing performance.
- Wise FT combines weights of pre-trained and fine-tuned models linearly to achieve significant accuracy gains.
- Model Soup merges weights from various fine-tuned models trained with different hyperparameters, improving performance.

# INSIGHTS:
- Fine-tuned weights form a thin shell layer-wise in weight space, improving model performance.
- Averaging weights closer together enhances both in-distribution and out-of-distribution task performance.
- Model Stock merges weights efficiently using geometric properties of weight space and pre-trained model anchoring.
- Consistent norms and angles among fine-tuned weights indicate a general pattern in weight distributions.
- Proximity to the center of the weight distribution is beneficial for model performance.
- Randomly perturbed weights near the center show high performance, emphasizing center proximity's importance.
- Fine-tuned weights follow a Gaussian distribution, explaining their geometric patterns.
- Periodic merging during training improves model performance and brings weights closer to the center.
- Model Stock achieves state-of-the-art performance with lower computational costs compared to existing methods.
- Proximity to the center of the weight distribution is more crucial for enhancing performance than hyperparameter diversity.

# QUOTES:
- "Fine-tuned model weights with different random seeds form a thin shell layer-wise in weight space."
- "Averaging weights that are closer together leads to better performance on both in-distribution and out-of-distribution tasks."
- "Model Stock aims to efficiently merge weights from just a few fine-tuned models by leveraging the geometric properties of the weight space."
- "Model Stock outperforms Model Soup in terms of computational costs while achieving comparable or even better results."
- "The norms and angles of these weights showed almost constant values with minimal errors."
- "Fine-tuned weights closer to the center exhibit improved performance on both in-distribution and out-of-distribution datasets."
- "Fine-tuned weights tended to occupy local minima edges in the test error landscape."
- "Randomly perturbed weights near the center also merit high performance."
- "Fine-tuned weights follow a Gaussian distribution, explaining their geometric patterns."
- "Model Stock leverages pre-trained models to approximate the weight center by interpolating between pre-trained and fine-tuned models."
- "Bias layers rely more on fine-tuned models while weight layers depend on pre-trained models."
- "Periodic merging during training improves model performance and brings weights closer to the center."
- "Model Stock does not require extra training or heuristic hyperparameter settings, simplifying the process."
- "Model Stock achieves state-of-the-art performance on ImageNet with various CLIP ViT models."
- "Model Stock outperforms Model Soup while using only two models, showcasing its efficiency."
- "Model Stock exhibits exceptional performance on ImageNet accuracy and robustness across various distribution shift scenarios."
- "Proximity to the center of the weight distribution might be more crucial for enhancing performance than hyperparameter diversity."

# HABITS:
- Periodically merge weights during training to improve model performance and bring weights closer to the center.
- Leverage pre-trained models to approximate the weight center by interpolating between pre-trained and fine-tuned models.
- Use consistent norms and angles among fine-tuned weights across various setups and training stages.
- Focus on moving fine-tuned weights closer to the center for improved performance on both in-distribution and out-of-distribution datasets.
- Conduct ablation studies to explore different merging periods and post-training merging strategies.

# FACTS:
- Fine-tuned model weights with different random seeds form a thin shell layer-wise in weight space.
- Averaging weights closer together leads to better performance on both in-distribution and out-of-distribution tasks.
- Model Stock merges weights from a few fine-tuned models using geometric properties of weight space.
- Model Stock is more computationally efficient than Model Soup while achieving comparable or better results.
- Fine-tuned weights' norms and angles are consistent across various setups and training stages.
- Fine-tuned weights closer to the center exhibit improved performance on both in-distribution and out-of-distribution datasets.
- Fine-tuned weights tend to occupy local minima edges in the test error landscape.
- Randomly perturbed weights near the center also show high performance.
- Fine-tuned weights follow a Gaussian distribution, explaining their geometric patterns.
- Model Stock leverages pre-trained models to approximate the weight center by interpolating between pre-trained and fine-tuned models.

# REFERENCES:
- CLIP ViT B32
- CLIP ViT B16
- CLIP ViT L14
- ImageNet 1K dataset
- Model Soup
- Wise FT

# ONE-SENTENCE TAKEAWAY
Model Stock efficiently merges fine-tuned model weights using geometric properties, achieving high performance with lower computational costs.

# RECOMMENDATIONS:
- Average weights closer together for better in-distribution and out-of-distribution task performance.
- Merge weights from a few fine-tuned models using geometric properties of weight space.
- Leverage pre-trained models to approximate the weight center by interpolating between pre-trained and fine-tuned models.
- Periodically merge weights during training to improve model performance and bring weights closer to the center.
- Use consistent norms and angles among fine-tuned weights across various setups and training stages.