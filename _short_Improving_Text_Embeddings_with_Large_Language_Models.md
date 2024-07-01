# SUMMARY
The paper presents a comprehensive approach to embedding tasks, categorizing them into asymmetric and symmetric groups, and evaluates their performance.

# IDEAS:
- Embedding tasks are categorized into asymmetric and symmetric groups based on a simple taxonomy.
- Asymmetric tasks are divided into short-long match, long-short match, short-short match, and long-long match.
- Symmetric tasks are divided into monolingual semantic textual similarity (STS) and bitext retrieval.
- A two-step prompt template is designed for asymmetric tasks to generate task-specific examples.
- Symmetric task prompts are tailored to specific objectives like monolingual STS and bitext retrieval.
- Placeholders in prompt templates are filled with values randomly sampled at runtime.
- The embedding model is trained using generated synthetic data with info NCE loss over in-batch negatives.
- A temperature-scaled cosine similarity function computes the matching score between query and document.
- The pre-trained mistl 7B checkpoint is fine-tuned using gradient checkpointing, mixed precision training, and DeepSpeed 03.
- The model is evaluated on the MTE Benchmark, outperforming previous state-of-the-art models by 2.4 points.
- The model significantly surpasses current commercial models in retrieval performance on the BEIR Benchmark.
- Generated synthetic data includes 500k examples with 150k unique instructions covering 93 languages.
- The model's multilingual retrieval capabilities are discussed, focusing on high-resource and low-resource languages.
- The impact of contrastive pre-training on model quality for mistl 7B based models is evaluated.
- Performance on personalized PASY retrieval tasks is analyzed.
- Training hyperparameters are analyzed, noting mistl 7B initialization outperforms llama 27B.
- Natural language instructions have a considerable impact on performance.

# INSIGHTS
- Embedding tasks can be effectively categorized into asymmetric and symmetric groups for better model training.
- Asymmetric tasks benefit from a two-step prompt template to generate task-specific examples.
- Symmetric task prompts need to be tailored to specific objectives like monolingual STS and bitext retrieval.
- Randomly sampled placeholders in prompt templates enhance the diversity of training data.
- Info NCE loss over in-batch negatives improves the training of embedding models.
- Temperature-scaled cosine similarity functions are effective for computing matching scores between queries and documents.
- Fine-tuning with gradient checkpointing, mixed precision training, and DeepSpeed 03 reduces GPU memory requirements.
- The mistl 7B model achieves superior performance on the MTE Benchmark compared to previous state-of-the-art models.
- Synthetic data generation covering multiple languages enhances the model's multilingual retrieval capabilities.
- Contrastive pre-training significantly impacts the quality of mistl 7B based models.
- Personalized PASY retrieval tasks benefit from the model's fine-tuning and training techniques.
- Mistl 7B initialization outperforms llama 27B in embedding tasks.
- Natural language instructions play a crucial role in improving model performance.

# QUOTES:
- "We categorize embedding tasks into asymmetric and symmetric groups based on a simple taxonomy."
- "Asymmetric tasks are divided into short-long match, long-short match, short-short match, and long-long match."
- "Symmetric tasks are divided into monolingual semantic textual similarity (STS) and bitext retrieval."
- "We designed a two-step prompt template for asymmetric tasks."
- "Symmetric task prompts are tailored to specific objectives like monolingual STS and bitext retrieval."
- "Placeholders in each prompt template are filled with values randomly sampled at runtime."
- "We train the embedding model using generated synthetic data with info NCE loss over in-batch negatives."
- "A temperature-scaled cosine similarity function computes the matching score between query and document."
- "We fine-tune the pre-trained mistl 7B checkpoint using gradient checkpointing, mixed precision training, and DeepSpeed 03."
- "Our model achieves the highest average score on the MTE Benchmark, outperforming previous state-of-the-art models by 2.4 points."
- "The model significantly surpasses current commercial models in retrieval performance on the BEIR Benchmark."
- "Generated synthetic data includes 500k examples with 150k unique instructions covering 93 languages."
- "We discuss the multilingual retrieval capabilities of our model."
- "Contrastive pre-training impacts the quality of mistl 7B based models."
- "We analyze the performance of our model on personalized PASY retrieval tasks."
- "Mistl 7B initialization performs better than llama 27B."
- "Natural language instructions have a considerable impact on performance."

# HABITS
- Designing two-step prompt templates for generating task-specific examples in asymmetric tasks.
- Tailoring symmetric task prompts to specific objectives like monolingual STS and bitext retrieval.
- Using randomly sampled placeholders in prompt templates to enhance training data diversity.
- Applying gradient checkpointing, mixed precision training, and DeepSpeed 03 for fine-tuning models.
- Evaluating models on benchmarks like MTE and BEIR to measure performance improvements.

# FACTS:
- Embedding tasks can be categorized into asymmetric and symmetric groups based on a simple taxonomy.
- Asymmetric tasks include short-long match, long-short match, short-short match, and long-long match.
- Symmetric tasks include monolingual semantic textual similarity (STS) and bitext retrieval.
- Generated synthetic data includes 500k examples with 150k unique instructions covering 93 languages.
- The mistl 7B model outperforms previous state-of-the-art models by 2.4 points on the MTE Benchmark.
- The model surpasses current commercial models in retrieval performance on the BEIR Benchmark.

# REFERENCES
None mentioned.

# ONE-SENTENCE TAKEAWAY
Embedding tasks benefit from tailored prompt templates and fine-tuning techniques, achieving superior multilingual retrieval performance.

# RECOMMENDATIONS
- Categorize embedding tasks into asymmetric and symmetric groups for better model training efficiency.
- Use two-step prompt templates for generating task-specific examples in asymmetric tasks.
- Tailor symmetric task prompts to specific objectives like monolingual STS and bitext retrieval.
- Incorporate randomly sampled placeholders in prompt templates to enhance training data diversity.
- Apply info NCE loss over in-batch negatives to improve embedding model training.
- Use temperature-scaled cosine similarity functions for computing matching scores between queries and documents.
- Fine-tune models with gradient checkpointing, mixed precision training, and DeepSpeed 03 to reduce GPU memory requirements.
- Evaluate models on benchmarks like MTE and BEIR to measure performance improvements.