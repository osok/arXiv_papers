# SUMMARY
The paper assesses if interpretability tools for Transformers can apply to new RNN models, specifically Mamba and RW KV V5, focusing on steerability and behavior control.

# IDEAS:
- The paper investigates steerability of RNNs using techniques originally developed for Transformers.
- Authors hypothesize steering with CA would work on RNNs without architecture-specific changes.
- Compressed state of RNNs might make them easier to steer compared to Transformers.
- The tuned lens approach helps understand RNN language models' predictions at different layers.
- Fine-tuning RNN models on specific behaviors and using linear probes elicits latent knowledge.
- Mamba and RW KV architectures handle long sequences by parallelized training across the time dimension.
- Mamba uses a selective state space model (SSM) in each layer, enhancing expressivity.
- RW KV employs alternating time mix and channel mix modules in its layers.
- Mamba uses causal convolution blocks to route information between token positions.
- RW KV V4 has a vector-valued state, while V5 has a matrix-valued state.
- Specific behaviors studied include coordination, hallucination, myopic reward, survival instinct, and refusal.
- Steering vectors are computed based on differences in mean activation vectors for specific behaviors.
- Steering vectors are multiplied by a scalar multiplier to determine the sign and strength of intervention.
- Steering effects are most prominent in the middle layers of the models.
- Selective state space model (SSM) in Mamba adapts parameters based on input data.
- SSM enhances Mamba's capacity to capture complex relationships and dependencies within sequences.
- State steering involves manipulating RNNs' internal state to influence responses.
- State steering generates a steering state vector based on the internal state of RNN models.
- Logit lens sets residuals to zero, while tuned lens trains affine transformations for each layer.
- Tuned lens aims for similarity with the final layer's token distribution.
- Probes in the ELK approach are trained using seven different linear probing methods.
- Linear probing methods include LDA, mass mean probing, logistic regression, CCS, CRC, and more.
- Probes are trained on examples containing specific contexts like "Alice."
- Probes' effectiveness is evaluated based on distinguishing between hard examples with different contexts.

# INSIGHTS:
- Steerability techniques for Transformers can potentially apply to RNNs without architecture-specific changes.
- Compressed states in RNNs may facilitate easier steering compared to Transformers.
- Fine-tuning and linear probes can elicit latent knowledge from RNN models.
- Mamba's selective state space model (SSM) enhances expressivity by adapting parameters based on input data.
- State steering manipulates RNNs' internal states to influence their responses effectively.
- Tuned lens provides a more refined approach to decoding intermediate values in Transformer models.
- Linear probing methods can generalize across different contexts and maintain accuracy in predictions.
- Steering effects are most prominent in the middle layers of RNN models.
- Mamba and RW KV architectures offer efficient handling of long sequences through unique mechanisms.
- Probes trained on easy examples with specific contexts can predict correct labels in challenging scenarios.

# QUOTES:
- "The paper investigates the steerability of RNNs using techniques originally developed for Transformers."
- "Compressed state of RNNs might make them easier to steer compared to Transformers."
- "The tuned lens approach helps understand RNN language models' predictions at different layers."
- "Mamba uses a selective state space model (SSM) in each layer, enhancing expressivity."
- "RW KV employs alternating time mix and channel mix modules in its layers."
- "Steering vectors are computed based on differences in mean activation vectors for specific behaviors."
- "Steering effects are most prominent in the middle layers of the models."
- "State steering involves manipulating RNNs' internal state to influence responses."
- "Logit lens sets residuals to zero, while tuned lens trains affine transformations for each layer."
- "Probes in the ELK approach are trained using seven different linear probing methods."

# HABITS:
- Fine-tuning RNN models on specific behaviors to elicit latent knowledge.
- Using linear probes to assess models' ability to generalize to unseen scenarios.
- Employing selective state space models (SSM) to enhance model expressivity.
- Manipulating internal states of RNNs for effective state steering.
- Training probes on examples containing specific contexts like "Alice."

# FACTS:
- Mamba and RW KV architectures handle long sequences by parallelized training across the time dimension.
- Mamba uses a selective state space model (SSM) in each layer, enhancing expressivity.
- RW KV employs alternating time mix and channel mix modules in its layers.
- RW KV V4 has a vector-valued state, while V5 has a matrix-valued state.
- Specific behaviors studied include coordination, hallucination, myopic reward, survival instinct, and refusal.

# REFERENCES:
- Selective State Space Model (SSM)
- Contrastive Activation Edition (CAA)
- State Steering
- Tuned Lens
- Linear Probing Methods: LDA, Mass Mean Probing, Logistic Regression, CCS, CRC

# ONE-SENTENCE TAKEAWAY
Steerability techniques for Transformers can apply to RNNs, enhancing their interpretability and behavior control.

# RECOMMENDATIONS:
- Investigate steerability of RNNs using techniques originally developed for Transformers.
- Hypothesize that steering with CA would work on RNNs without architecture-specific changes.
- Explore the tuned lens approach to understand RNN language models' predictions at different layers.
- Fine-tune RNN models on specific behaviors and use linear probes to elicit latent knowledge.
- Utilize selective state space models (SSM) in each layer to enhance expressivity.