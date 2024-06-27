# SUMMARY
Researchers propose a new metric, CMMD, using CLIP embeddings and MMD distance to evaluate text-to-image models, addressing FID's limitations.

# IDEAS:
- Text-to-image models need reliable evaluation metrics for continued progress.
- FID often doesn't align with human evaluations, suggesting it's not the best choice.
- CMMD uses CLIP embeddings and MMD distance to overcome FID's limitations.
- Evaluating image generation models is complex, requiring multiple performance aspects.
- Human evaluation remains the gold standard but is costly and doesn't scale well.
- FID assumes Inception embeddings come from a multivariant normal distribution.
- FID's results can be inconsistent when sample sizes vary.
- FID can contradict human raters and fail to capture complex image distortions.
- CLIP is trained on 400 million images with text descriptions, making it more suitable.
- MMD doesn't assume distributions, unlike FID, which assumes normality.
- MMD is an unbiased estimator and doesn't depend on sample size like FID.
- MMD allows for simple parallel implementation and fast computation.
- CMMD avoids FID's drawbacks and aligns better with human perception.
- FID's assumption of normality can lead to errors in high-dimensional feature spaces.
- High-dimensional covariance matrices from small samples can cause significant errors.
- CMMD uses Gaussian RBF kernel for calculating MMD distance between CLIP embeddings.
- Human evaluation showed CMMD aligns with human preference, unlike FID.
- CMMD correctly identifies quality improvements during iterative image generation.
- FID fails to reflect image quality degradation under complex distortions.
- CMMD provides consistent estimates even with small image sets.
- CMMD is faster and more practical for evaluating image generation models.
- Calculating FID involves demanding matrix operations not suited for parallel processing.
- MMD involves matrix multiplications, easily parallelized in deep learning libraries.
- Researchers should reconsider using FID as the primary evaluation metric.
- Relying on FID could result in dismissing potentially good ideas too early.

# INSIGHTS:
- Reliable evaluation metrics are crucial for the progress of text-to-image models.
- Human evaluation is the gold standard but impractical due to cost and scalability issues.
- FID's assumption of normality often leads to errors in high-dimensional spaces.
- CLIP embeddings are more suitable for diverse and complex content in generated images.
- MMD is unbiased and doesn't depend on sample size, unlike FID.
- CMMD aligns better with human perception of image quality than FID.
- CMMD is faster and more practical for evaluating image generation models.
- Relying on FID could lead to dismissing innovative ideas prematurely.
- Evaluating image generation models requires assessing multiple performance aspects.
- Human raters overwhelmingly preferred images evaluated by CMMD over FID.

# QUOTES:
- "Human evaluation remains the gold standard for text-to-image research."
- "FID may not be the best choice for evaluating text-to-image models."
- "CLIP is trained on 400 million images with corresponding text descriptions."
- "MMD doesn't make any assumptions about the distributions."
- "FID can contradict human raters and fail to capture complex image distortions."
- "CMMD uses CLIP embeddings and the MMD distance."
- "Evaluating image generation models is a complex task."
- "Human evaluation is costly and doesn't scale well."
- "FID's assumption of normality can lead to errors."
- "CMMD correctly identifies quality improvements during iterative image generation."
- "FID fails to reflect image quality degradation under complex distortions."
- "CMMD provides consistent estimates even with small image sets."
- "CMMD is faster and more practical for evaluating image generation models."
- "Calculating FID involves demanding matrix operations not suited for parallel processing."
- "MMD involves matrix multiplications, easily parallelized in deep learning libraries."
- "Researchers should reconsider using FID as the primary evaluation metric."
- "Relying on FID could result in dismissing potentially good ideas too early."

# HABITS:
- Conducting human evaluations to align metrics with human perception of quality.
- Using high-quality crowd computing platforms for independent evaluations.
- Visualizing features of datasets to test assumptions about distributions.
- Applying statistical tests to validate assumptions about data distributions.
- Using anti-alias resizing operations to avoid negative effects on metrics.

# FACTS:
- CLIP is trained on 400 million images with corresponding text descriptions.
- Inception V3 is trained on around 1 million images limited to 1,000 classes.
- MMD doesn't assume distributions, unlike FID, which assumes normality.
- MMD is an unbiased estimator and doesn't depend on sample size like FID.
- Calculating FID involves demanding matrix operations not suited for parallel processing.

# REFERENCES:
- Inception V3 model
- CLIP embeddings
- Maximum Mean Discrepancy (MMD)
- Gaussian RBF kernel
- COCO 30k dataset
- Stable Diffusion 1.4 model
- Muse model
- Party model

# ONE-SENTENCE TAKEAWAY
CMMD offers a more reliable, robust, and practical alternative to FID for evaluating text-to-image models.

# RECOMMENDATIONS:
- Use CMMD instead of FID for evaluating text-to-image models' quality and fidelity.
- Conduct human evaluations to ensure metrics align with human perception of quality.
- Apply anti-alias resizing operations to avoid negative effects on metrics.
- Visualize dataset features to test assumptions about data distributions.
- Use statistical tests to validate assumptions about data distributions.