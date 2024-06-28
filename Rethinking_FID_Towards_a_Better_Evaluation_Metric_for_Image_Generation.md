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
- CMMD provides consistent estimates even with small image sets, unlike FID.
- CMMD is faster and more practical for evaluating image generation models.
- Calculating FID involves demanding matrix operations not suited for parallel processing.
- MMD involves matrix multiplications, easily parallelized and optimized in deep learning libraries.
- Researchers should reconsider using FID as the primary evaluation metric for image quality.
- Relying on FID could result in dismissing potentially good ideas too early.

# INSIGHTS:
- Human evaluation is costly and doesn't scale well, making automated metrics essential.
- CLIP embeddings are better suited for diverse and complex content in generated images.
- MMD is unbiased and doesn't depend on sample size, unlike FID.
- CMMD aligns better with human perception of image quality than FID.
- High-dimensional covariance matrices from small samples can cause significant errors in FID.
- CMMD uses Gaussian RBF kernel for calculating MMD distance between CLIP embeddings.
- Human evaluation showed CMMD aligns with human preference, unlike FID.
- CMMD correctly identifies quality improvements during iterative image generation.
- FID fails to reflect image quality degradation under complex distortions.
- CMMD provides consistent estimates even with small image sets, unlike FID.

# QUOTES:
- "Human evaluation remains the gold standard for text-to-image research."
- "FID can contradict human raters and fail to capture complex image distortions."
- "CLIP is trained on 400 million images with corresponding text descriptions."
- "MMD doesn't make any assumptions about the distributions."
- "MMD is an unbiased estimator and doesn't exhibit a strong dependency on sample size."
- "CMMD avoids the drawbacks of FID."
- "FID's assumption of normality can lead to errors in high-dimensional feature spaces."
- "High-dimensional covariance matrices from small samples can cause significant errors."
- "CMMD uses Gaussian RBF kernel for calculating MMD distance between CLIP embeddings."
- "Human evaluation showed CMMD aligns with human preference, unlike FID."
- "CMMD correctly identifies quality improvements during iterative image generation."
- "FID fails to reflect image quality degradation under complex distortions."
- "CMMD provides consistent estimates even with small image sets, unlike FID."
- "CMMD is faster and more practical for evaluating image generation models."
- "Calculating FID involves demanding matrix operations not suited for parallel processing."
- "MMD involves matrix multiplications, easily parallelized and optimized in deep learning libraries."
- "Researchers should reconsider using FID as the primary evaluation metric for image quality."
- "Relying on FID could result in dismissing potentially good ideas too early."

# HABITS:
- Conducting human evaluations to align automated metrics with human perception.
- Using large datasets like CLIP's 400 million images for training models.
- Employing Gaussian RBF kernel for calculating MMD distance in evaluations.
- Performing side-by-side evaluations with independent raters for unbiased results.
- Utilizing high-quality crowd computing platforms for human evaluations.

# FACTS:
- Text-to-image models need reliable evaluation metrics for continued progress.
- Human evaluation remains the gold standard but is costly and doesn't scale well.
- CLIP is trained on 400 million images with text descriptions, making it more suitable.
- MMD doesn't assume distributions, unlike FID, which assumes normality.
- MMD is an unbiased estimator and doesn't depend on sample size like FID.

# REFERENCES:
- CLIP embeddings
- Maximum Mean Discrepancy (MMD) distance
- Gaussian RBF kernel
- Inception V3 model
- COCO 30k dataset
- Stable Diffusion 1.4 model
- Muse model
- Party prompts collection

# ONE-SENTENCE TAKEAWAY
CMMD offers a more reliable and robust alternative to FID for evaluating text-to-image models.

# RECOMMENDATIONS:
- Use CMMD instead of FID for evaluating text-to-image models' quality and fidelity.
- Employ large datasets like CLIP's 400 million images for training models.
- Conduct human evaluations to align automated metrics with human perception.
- Utilize Gaussian RBF kernel for calculating MMD distance in evaluations.
- Perform side-by-side evaluations with independent raters for unbiased results.