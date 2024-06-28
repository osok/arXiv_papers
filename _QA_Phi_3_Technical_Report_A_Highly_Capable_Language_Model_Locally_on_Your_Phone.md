# SUMMARY
The F3 Mini model, a small yet highly capable language model, aims to match larger models' performance while being efficient for local inference on modern phones.

# IDEAS:
- The F3 Mini model aims to match larger models' performance while being small and efficient.
- It was trained on larger, more advanced datasets compared to its predecessor, Phi2.
- The model combines LLM-based filtering of web data and LLM-created synthetic data.
- Focus on data quality allows smaller models to reach larger models' performance levels.
- Quantized to 4 bits, it runs efficiently on devices like the iPhone 14.
- The model is a Transformer decoder architecture with a default context length of 4K.
- It can extend to a long context version with a context length of 128K.
- Built upon a similar block structure as Llama 2, using the same tokenizer.
- The model has 372 hidden dimensions, 32 heads, and 32 layers.
- Trained using B float 16 for a total of 3.3T tokens.
- Chat fine-tuned and can be quantized to four bits, occupying approximately 1.8 GB of memory.
- Achieves more than 12 tokens per second when running natively on-device and fully offline.
- Training data includes heavily filtered web data and synthetic LLM-generated data.
- Phase one involves web sources for general knowledge and language understanding.
- Phase two merges filtered web data with synthetic data for logical reasoning and niche skills.
- Calibrated to be in the data optimal regime for small models.
- Post-training includes supervised instruction fine-tuning and preference tuning with DPO.
- Evaluated across dozens of RY harm categories to ensure alignment with responsible AI principles.
- Undergoes red teaming and automated testing to identify areas of improvement.
- Evaluated on standard open-source benchmarks measuring reasoning ability.
- Safety benchmarks evaluate responses in terms of groundedness and harmfulness.
- Despite capabilities, limitations include limited factual knowledge storage and English language restrictions.
- Offers theoretical and practical benefits compared to larger models like Mixol 8X 7B and GPT-3.5.
- Innovative training methodology focuses on data quality rather than sheer scale.
- Can be easily inferenced locally on a modern phone, providing efficiency and accessibility.
- Undergoes rigorous post-training processes aligned with responsible AI principles.

# INSIGHTS:
- Smaller models can achieve large models' performance by focusing on training data quality.
- Quantization to 4 bits significantly reduces memory usage, enabling efficient local inference.
- Combining LLM-based filtering and synthetic data enhances model training effectiveness.
- Data optimal regime calibration is crucial for small model performance enhancement.
- Post-training processes ensure robustness, safety, and alignment with ethical standards.

# QUOTES:
- "The motivation behind developing the F3 Mini model was to push the boundaries of what small language models can achieve."
- "The goal was to demonstrate that by focusing on the quality of training data... smaller models can reach the level of larger models."
- "The F3 Mini model was quantized to 4 bits to reduce memory usage."
- "The model achieves more than 12 tokens per second when running natively on-device and fully offline."
- "Training data consists of heavily filtered web data from various open internet sources."
- "Phase one involves web sources to teach the model general knowledge and language understanding."
- "Phase two merges filtered web data with synthetic data to teach the model logical reasoning and niche skills."
- "The model is calibrated to be in the data optimal regime for small models."
- "Post-training includes supervised instruction fine-tuning and preference tuning with DPO."
- "Evaluations across dozens of RY harm categories ensure alignment with responsible AI principles."
- "Red teaming and automated testing identify areas of improvement."
- "Evaluated on standard open-source benchmarks measuring reasoning ability."
- "Safety benchmarks evaluate responses in terms of groundedness and harmfulness."
- "Despite its capabilities, the F3 Mini model has limitations related to its size."
- "The F3 Mini model offers theoretical and practical benefits compared to larger models."

# HABITS:
- Focus on high-quality training data rather than sheer scale for model development.
- Combine LLM-based filtering of web data with synthetic LLM-generated data for training.
- Calibrate models to be in the data optimal regime for enhanced performance.
- Conduct rigorous post-training processes including supervised instruction fine-tuning.
- Perform red teaming and automated testing to identify areas of improvement.

# FACTS:
- The F3 Mini model has 372 hidden dimensions, 32 heads, and 32 layers.
- Trained using B float 16 for a total of 3.3T tokens.
- Quantized to four bits, occupying approximately 1.8 GB of memory.
- Achieves more than 12 tokens per second when running natively on-device.
- Evaluated across dozens of RY harm categories for responsible AI alignment.

# REFERENCES:
- Llama 2
- Mixol 8X 7B
- GPT-3.5
- Phi2
- iPhone 14 with A16 Bionic chip

# ONE-SENTENCE TAKEAWAY
Focusing on high-quality training data enables small language models like F3 Mini to match larger models' performance.

# RECOMMENDATIONS:
- Focus on high-quality training data rather than sheer scale for better model performance.
- Combine LLM-based filtering of web data with synthetic LLM-generated data for training effectiveness.
- Calibrate models to be in the data optimal regime for enhanced performance.
- Conduct rigorous post-training processes including supervised instruction fine-tuning.
- Perform red teaming and automated testing to identify areas of improvement.