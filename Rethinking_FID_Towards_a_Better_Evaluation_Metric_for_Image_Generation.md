# SUMMARY
Researchers propose a new metric, CMMD, to evaluate text-to-image models, addressing limitations of the current FID metric.

# IDEAS:
- Text-to-image models need reliable evaluation metrics for continued progress.
- FID doesn't always align with human evaluations, suggesting it may not be the best choice.
- CMMD uses CLIP embeddings and Maximum Mean Discrepancy (MMD) distance.
- FID fails to reflect progressive distortion applied to images.
- Evaluating image generation models is complex, requiring multiple performance aspects.
- Human evaluation remains the gold standard but is costly and doesn't scale well.
- FID assumes Inception embeddings come from a multivariate normal distribution.
- FID can contradict human raters and doesn't reflect gradual improvement.
- CLIP is trained on 400 million images with corresponding text descriptions.
- MMD doesn't make assumptions about distributions, unlike FID.
- MMD is an unbiased estimator and doesn't exhibit strong dependency on sample size.
- CMMD avoids the drawbacks of FID and aligns with human perception of image quality.
- FID's assumption of normality can lead to errors and misleading results.
- High-dimensional covariance matrices from small samples can lead to large errors.
- CLIP embeddings are better at representing diverse and complex content.
- MMD was developed as part of a two-sample statistical test.
- MMD is sample efficient and allows for simple parallel implementation.
- CMMD uses the Gaussian RBF kernel with a fixed bandwidth parameter.
- Human evaluation showed that CMMD aligns with human preference better than FID.
- FID requires a large number of images for reliable estimation.
- CMMD provides consistent estimates even with small image sets.
- CMMD evaluation is faster and more practical than FID evaluation.

# INSIGHTS:
- Reliable evaluation metrics are crucial for the progress of text-to-image models.
- Human evaluation is the gold standard but impractical for large-scale use.
- FID's assumption of normality often leads to errors in high-dimensional spaces.
- CLIP embeddings offer a richer representation due to extensive training data.
- MMD's unbiased nature makes it more reliable for evaluating image quality.
- CMMD aligns better with human perception, making it a superior metric.
- FID's poor sample efficiency limits its practical application in model development.
- CMMD's fast computation and sample efficiency make it ideal for real-world use.
- Evaluating image generation models requires considering multiple performance aspects.
- Relying on FID could result in dismissing potentially good ideas too early.

# QUOTES:
- "Human evaluation remains the gold standard for text-to-image research."
- "FID doesn't always align with human evaluations, suggesting it may not be the best choice."
- "Evaluating image generation models is a complex task."
- "CLIP is trained on 400 million images with corresponding text descriptions."
- "MMD doesn't make any assumptions about the distributions."
- "CMMD avoids the drawbacks of FID and aligns with human perception of image quality."
- "FID can contradict human raters and doesn't reflect gradual improvement."
- "High-dimensional covariance matrices from small samples can lead to large errors."
- "CLIP embeddings are better at representing diverse and complex content."
- "MMD was developed as part of a two-sample statistical test."
- "CMMD uses the Gaussian RBF kernel with a fixed bandwidth parameter."
- "Human evaluation showed that CMMD aligns with human preference better than FID."
- "FID requires a large number of images for reliable estimation."
- "CMMD provides consistent estimates even with small image sets."
- "CMMD evaluation is faster and more practical than FID evaluation."
- "Reliable evaluation metrics are crucial for the progress of text-to-image models."
- "Human evaluation is the gold standard but impractical for large-scale use."
- "FID's assumption of normality often leads to errors in high-dimensional spaces."
- "CLIP embeddings offer a richer representation due to extensive training data."
- "MMD's unbiased nature makes it more reliable for evaluating image quality."

# HABITS:
- Conducting human evaluations to align metrics with human perception.
- Using CLIP embeddings for richer representation in text-to-image models.
- Applying statistical tests to validate assumptions in evaluation metrics.
- Visualizing features to understand their distribution and characteristics.
- Fixing parameters in metrics to obtain consistent values.

# FACTS:
- FID assumes Inception embeddings come from a multivariate normal distribution.
- CLIP is trained on 400 million images with corresponding text descriptions.
- MMD doesn't make assumptions about distributions, unlike FID.
- MMD is an unbiased estimator and doesn't exhibit strong dependency on sample size.
- High-dimensional covariance matrices from small samples can lead to large errors.
- CMMD uses the Gaussian RBF kernel with a fixed bandwidth parameter.
- Human evaluation showed that CMMD aligns with human preference better than FID.
- FID requires a large number of images for reliable estimation.
- CMMD provides consistent estimates even with small image sets.

# REFERENCES:
- CLIP embeddings
- Maximum Mean Discrepancy (MMD)
- Gaussian RBF kernel
- Inception V3 model
- COCO 30k dataset
- Stable Diffusion 1.4 model
- Muse model
- Party prompts collection

# ONE-SENTENCE TAKEAWAY
CMMD offers a more reliable and robust alternative to FID for evaluating text-to-image models, aligning better with human perception.

# RECOMMENDATIONS:
- Use CMMD instead of FID for evaluating text-to-image models' quality and fidelity.
- Conduct human evaluations to ensure metrics align with human perception.
- Apply statistical tests to validate assumptions in evaluation metrics.
- Use CLIP embeddings for richer representation in text-to-image models.
- Fix parameters in metrics to obtain consistent values across evaluations.