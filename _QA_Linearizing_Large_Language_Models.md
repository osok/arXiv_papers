# SUMMARY
Supra aims to efficiently convert large Transformers into performant RNNs for sequence modeling tasks, addressing instability and performance issues in linear Transformers.

# IDEAS:
- Supra leverages high-quality pre-trained Transformers linearized using a fraction of pre-training data.
- It addresses normalization instability by replacing it with a group norm operation.
- Supra incorporates modern relative positional encoding schemes like RoPE.
- Shared weights between keys and queries are introduced in Supra.
- Supra uses trainable layers with a similarity function defined as FX = ReLU(WX + b).
- New parameters in Supra are trained jointly with the rest of the network.
- A fixed decay vector gamma is employed for stable attention computations.
- Recurrent formulation is utilized for inference at test time in Supra.
- Supra demonstrates competitive results with the strongest pre-trained recurrent models.
- Linear attention reduces inference cost for language and multimodal models.
- Linear attention allows for constant inference cost regardless of the number of generated tokens.
- Linearization technique connects Transformers and RNNs, providing duality in training and inference.
- Linear attention offers computational benefits and stability advantages for long sequences.
- Supra outperforms RW kv5 with minimal up-training and is competitive with a 7B Mamba model.
- Supra preserves performance on most benchmarks compared to Transformers and linear models at 7B scale.
- Performance drop in Supra models compared to softmax Transformers is noted.
- Data quality influences the performance of Supra models.
- Normalization is key for stable up-training in Supra.
- T2R up-training method was unstable compared to Supra.
- Supra relies on initializing with strong pre-trained Transformers.
- Supra models suffer from poor performance on tasks requiring in-context learning.

# INSIGHTS:
- Supra bridges the gap between softmax Transformers' performance and linear Transformers' efficiency.
- Modern relative positional encoding schemes enhance performance in Supra.
- Joint training of new parameters ensures cohesive learning in Supra.
- Fixed decay vector ensures stable attention computations during training and inference.
- Linear attention's constant inference cost benefits long sequence processing.
- Supra's competitive performance showcases its effectiveness in converting Transformers into RNNs.
- Data quality significantly impacts the performance of linearized models like Supra.
- Normalization stability is crucial for effective up-training in large-scale models.
- Strong pre-trained Transformers are essential for initializing effective Supra models.
- In-context learning remains a challenge for linear models like Supra.

# QUOTES:
- "Supra leverages high-quality pre-trained Transformers linearized using a fraction of pre-training data."
- "It addresses normalization instability by replacing it with a group norm operation."
- "Supra incorporates modern relative positional encoding schemes like RoPE."
- "Shared weights between keys and queries are introduced in Supra."
- "Supra uses trainable layers with a similarity function defined as FX = ReLU(WX + b)."
- "New parameters in Supra are trained jointly with the rest of the network."
- "A fixed decay vector gamma is employed for stable attention computations."
- "Recurrent formulation is utilized for inference at test time in Supra."
- "Supra demonstrates competitive results with the strongest pre-trained recurrent models."
- "Linear attention reduces inference cost for language and multimodal models."
- "Linear attention allows for constant inference cost regardless of the number of generated tokens."
- "Linearization technique connects Transformers and RNNs, providing duality in training and inference."
- "Linear attention offers computational benefits and stability advantages for long sequences."
- "Supra outperforms RW kv5 with minimal up-training and is competitive with a 7B Mamba model."
- "Supra preserves performance on most benchmarks compared to Transformers and linear models at 7B scale."
- "Performance drop in Supra models compared to softmax Transformers is noted."
- "Data quality influences the performance of Supra models."
- "Normalization is key for stable up-training in Supra."
- "T2R up-training method was unstable compared to Supra."
- "Supra relies on initializing with strong pre-trained Transformers."
- "Supra models suffer from poor performance on tasks requiring in-context learning."

# HABITS:
- Leveraging high-quality pre-trained Transformers for efficient model conversion.
- Addressing normalization instability through group norm operations.
- Incorporating modern relative positional encoding schemes like RoPE.
- Introducing shared weights between keys and queries for better performance.
- Using trainable layers with a similarity function defined as FX = ReLU(WX + b).
- Training new parameters jointly with the rest of the network for cohesive learning.
- Employing a fixed decay vector gamma for stable attention computations.
- Utilizing recurrent formulation for efficient inference at test time.

# FACTS:
- Supra leverages high-quality pre-trained Transformers linearized using a fraction of pre-training data.
- It addresses normalization instability by replacing it with a group norm operation.
- Modern relative positional encoding schemes like RoPE are incorporated in Supra.
- Shared weights between keys and queries are introduced in Supra.
- Trainable layers with a similarity function defined as FX = ReLU(WX + b) are used in Supra.
- New parameters in Supra are trained jointly with the rest of the network.
- A fixed decay vector gamma is employed for stable attention computations.
- Recurrent formulation is utilized for inference at test time in Supra.
- Linear attention reduces inference cost for language and multimodal models.
- Linear attention allows for constant inference cost regardless of the number of generated tokens.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
Supra efficiently converts large Transformers into performant RNNs, addressing instability and performance issues in linear Transformers.

# RECOMMENDATIONS:
- Leverage high-quality pre-trained Transformers for efficient model conversion using a fraction of pre-training data.
- Address normalization instability by replacing it with a group norm operation for better stability.
- Incorporate modern relative positional encoding schemes like RoPE to enhance model performance.
- Introduce shared weights between keys and queries to improve model efficiency and effectiveness.
- Use trainable layers with a similarity function defined as FX = ReLU(WX + b) for better learning outcomes.