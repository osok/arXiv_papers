# SUMMARY
The paper presents the Pit Method, which eliminates the inductive bias of locality in Vision Transformers (ViT) by treating each pixel as a token.

# IDEAS:
- Pit aims to remove inductive biases related to locality in Vision Transformers (ViT) architecture.
- Treating each individual pixel as a token for the Transformer.
- Using position embeddings learned from scratch to eliminate locality bias.
- Challenges the belief that locality is a fundamental inductive bias for vision tasks.
- Viewing images as sets of individual pixels rather than patches.
- Transformer can capture more signals and create versatile systems for vision tasks.
- Pit achieves better results in quality compared to baselines with locality bias.
- Treats individual pixels in an image as tokens, removing locality bias.
- Each pixel in the image is treated as a separate token.
- Linear projection of each pixel token into a d-dimensional vector.
- Projected pixel tokens are arranged into a sequence with a learnable CLS token.
- Learnable position embeddings provide spatial information.
- Sequence of pixel tokens fed into a Transformer architecture.
- Eliminates inductive bias of locality present in traditional architectures like ViT.
- Models arbitrarily sized images and generalizes to irregular regions.
- Reduces vocabulary size significantly compared to patch-based tokenization.
- Computationally expensive for modeling long sequences but feasible with advancements.
- Theoretical benefits include removal of inductive bias and handling irregular regions.
- Practical benefits include effectiveness in supervised learning, self-supervised learning, and image generation.
- Empirical verification shows Pit's potential in various vision tasks.
- Validated through supervised learning, self-supervised learning, and image generation case studies.
- Achieved better quality results than baselines in supervised learning.
- Improved accuracy with self-supervised pre-training using masked autoencoding (MAE).
- Outperformed baselines in image generation tasks with diffusion Transformer (DiT).
- Computational expense associated with modeling long sequences of individual pixels.
- Not as practical as ViT in terms of efficiency due to longer sequences.
- Future advancements may address computational challenges of Pit.

# INSIGHTS:
- Removing locality bias allows Transformers to model images as sets of individual pixels.
- Pit's design enables it to handle arbitrarily sized images and irregular regions effectively.
- Treating pixels as tokens reduces vocabulary size, avoiding out-of-vocabulary issues.
- Pit challenges the belief that locality is essential for vision tasks, showing better results without it.
- Empirical results suggest Pit can scale better than ViT, especially with self-supervised pre-training.

# QUOTES:
- "Pit aims to completely remove the remaining inductive biases related to locality in ViT."
- "By viewing images as sets of individual pixels rather than patches, the Transformer can capture more signals."
- "Pit not only successfully removes the locality bias but also achieves better results in quality."
- "Treating each pixel as a token and using learnable position embeddings eliminates the inductive bias of locality."
- "Pit can model arbitrarily sized images and generalize to irregular regions."
- "Treating pixels as tokens reduces the vocabulary size significantly compared to patch-based tokenization."
- "Pit challenges the conventional belief that locality is a fundamental inductive bias for vision tasks."
- "Pit demonstrates effectiveness in various tasks such as supervised learning, self-supervised learning, and image generation."
- "The computational expense of modeling long sequences may not be a critical bottleneck."
- "Pit could be a valuable addition to the toolkit for processing images."

# HABITS:
- Treating each pixel in an image as a separate token for processing.
- Using learnable position embeddings to provide spatial information in sequences.
- Arranging projected pixel tokens into sequences with a learnable CLS token.
- Feeding sequences of pixel tokens into a Transformer architecture for processing.

# FACTS:
- Pit eliminates the inductive bias of locality in Vision Transformers (ViT).
- Each pixel in an image is treated as a separate token in Pit.
- Learnable position embeddings are used to provide spatial information in Pit.
- Pit achieves better quality results compared to baselines with locality bias.
- Pit can model arbitrarily sized images and generalize to irregular regions.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
Pit removes locality bias in Vision Transformers by treating pixels as tokens, achieving superior results.

# RECOMMENDATIONS:
- Remove inductive biases related to locality in Vision Transformers for better performance.
- Treat each individual pixel as a token for more versatile vision systems.
- Use position embeddings learned from scratch to eliminate locality bias.
- View images as sets of individual pixels rather than patches for better signal capture.
- Consider Pit's design for modeling arbitrarily sized images and irregular regions.