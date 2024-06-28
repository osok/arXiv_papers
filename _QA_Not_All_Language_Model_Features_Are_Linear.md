# SUMMARY
The paper addresses gaps in understanding how language models use multi-dimensional representations, proposing a method using sparse autoencoders to discover and analyze these features.

# IDEAS:
- The proposed method addresses gaps in understanding multi-dimensional representations in language models.
- Existing research primarily focuses on one-dimensional features and linear representations.
- The method uses sparse autoencoders to discover multi-dimensional features in language models.
- Clustering dictionary elements based on cosine or Jaccard similarity is the first step.
- Sparse autoencoders are run on hidden states to focus on specific multi-dimensional features.
- Reconstructed activation vectors are examined to identify irreducible multi-dimensional features.
- Visual inspection or automated testing validates the presence of multi-dimensional features.
- The method has been successful on synthetic data sets with known irreducible features.
- Discovering multi-dimensional features refines understanding of model behavior beyond linear representations.
- Multi-dimensional features provide a more comprehensive view of how models process information.
- Uncovering these features is crucial for advancing interpretability and transparency of models.
- Practical benefits include methodologies like sparse autoencoders for discovering complex representations.
- Circular representations are validated through tasks related to modular arithmetic.
- Intervention experiments show models use circular representations for modular arithmetic tasks.
- Layerwise activation patching and EVR techniques isolate circuits for computing target outputs.
- Sparse autoencoders find interpretable circles in hidden states of GPT-2 and Mistell 7B models.
- Weekdays and months tasks demonstrate usage of circular representations in language models.
- Limitations include uncertainties about the scarcity of interpretable multi-dimensional features.
- Clustering technique effectiveness in identifying multi-dimensional features is uncertain.
- Definition of irreducible features has to be relaxed for practical constraints.
- Study did not uncover a small subset of MLP neurons responsible for clock algorithm.
- Experiments were conducted only on models up to size 8B, larger models may show more universal representations.

# INSIGHTS:
- Multi-dimensional features refine understanding of model behavior beyond linear representations.
- Sparse autoencoders effectively discover and analyze multi-dimensional features in language models.
- Circular representations are fundamental units of computation for certain problems in large language models.
- Practical methodologies like sparse autoencoders advance interpretability and transparency of models.
- Clustering dictionary elements based on similarity helps identify multi-dimensional features.
- Visual inspection or automated testing validates the presence of multi-dimensional features.
- Weekdays and months tasks showcase how models use circular representations for modular arithmetic.
- Uncovering multi-dimensional features is crucial for revealing true variables within language models.
- Larger model sizes may show more universal representations, indicating scalability of findings.
- Identifying irreducible multi-dimensional features provides a comprehensive view of model processing.

# QUOTES:
- "The proposed method addresses the gap in existing research on language models regarding the understanding of how language models utilize multi-dimensional representations."
- "The research in the field has primarily focused on one-dimensional features and linear representations."
- "Sparse autoencoders are run on all hidden states in the layer during this process."
- "The resulting reconstructed activation vectors are then examined to identify reducible multi-dimensional features."
- "The examination of the reconstructed activation vectors can be done manually by visually inspecting PCA projections."
- "The method has been successful on synthetic data sets with known irreducible multi-dimensional features."
- "Discovering multi-dimensional representations refines the understanding of model behavior beyond simple one-dimensional linear representations."
- "Uncovering these multi-dimensional representations is crucial for revealing the true variables within language models."
- "Circular representations are validated through tasks related to modular arithmetic such as modular addition in days of the week."
- "Intervention experiments are then conducted on Mistell 7B and Llama 38B models to show that they indeed use circular representations."
- "Layerwise activation patching and explanation via regression (EVR) techniques isolate the circuit for computing the target output."
- "Sparse autoencoders discover irreducible multi-dimensional features, finding interpretable circles in the hidden states of GPT-2 and Mistell 7B models."
- "The specific tasks proposed to demonstrate the usage of circular representations in language models are the weekdays task and the month's task."
- "The definition of irreducible features has to be relaxed to align with practical constraints."
- "The study did not uncover a small subset of MLP neurons responsible for implementing the clock algorithm."

# HABITS:
- Clustering dictionary elements based on cosine or Jaccard similarity helps identify feature groups.
- Running sparse autoencoders on hidden states focuses reconstruction on specific multi-dimensional features.
- Examining reconstructed activation vectors identifies irreducible multi-dimensional features.
- Visual inspection or automated testing validates presence of multi-dimensional features.
- Conducting intervention experiments shows model usage of circular representations for modular arithmetic tasks.

# FACTS:
- Existing research primarily focuses on one-dimensional features and linear representations in language models.
- Sparse autoencoders can discover and analyze multi-dimensional features in language models.
- Clustering dictionary elements based on similarity helps identify groups corresponding to specific features.
- Visual inspection or automated tests validate presence of multi-dimensional features.
- Circular representations are fundamental units of computation for certain problems in large language models.

# REFERENCES:
- GPT-2
- Mistell 7B
- Llama 38B

# ONE-SENTENCE TAKEAWAY
Discovering multi-dimensional features refines understanding and advances interpretability of language models beyond linear representations.

# RECOMMENDATIONS:
- Use sparse autoencoders to discover and analyze multi-dimensional features in language models.
- Cluster dictionary elements based on cosine or Jaccard similarity to identify feature groups.
- Examine reconstructed activation vectors to identify irreducible multi-dimensional features.
- Validate presence of multi-dimensional features through visual inspection or automated testing.
- Conduct intervention experiments to show model usage of circular representations for modular arithmetic tasks.