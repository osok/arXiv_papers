# SUMMARY
The Raika models, including Core, Flash, and Edge, aim to advance language and vision tasks by outperforming larger models in efficiency and performance.

# IDEAS:
- Raika models excel in both automated base model evaluations and blind third-party human evaluations.
- Designed to outperform larger models like GPT-4V and Gemini Ultra in language and vision tasks.
- Focus on improving multimodal capabilities, excelling in multimodal chat evaluations.
- Developed to be powerful and competitive on a compute class basis.
- Training involves ingesting diverse datasets, including text, images, videos, and audio clips.
- Training data includes 25% code-related, 30% STEM-related, 25% web crawl data, and 10% math-related content.
- About 15% of pre-training data is multilingual with 32 diverse languages.
- Models use a modular encoder-decoder architecture supporting text, image, video, and audio inputs.
- Backbone Transformer model utilizes Su glue grouped query attention, rotary positional embeddings, and RMS Norm.
- Regular models have a context length of 8K; long context models have 128K.
- Synthetic creation of supervised fine-tuning data using reverse instruction tuning from long documents.
- Trained predominantly on Nvidia H100s using PyTorch with clusters from various vendors.
- Peak compute involves approximately 2.5K H100s and 2.5K A100s.
- Optimized for quality, diversity, and scale with a focus on improving IO performance using SEF file system.
- Superior performance across a range of language and vision tasks within their compute class.
- More computationally efficient and cost-effective compared to other models in the same compute class.
- Advanced architecture features enhance modeling capabilities and overall performance.
- Validated through comprehensive evaluations on language and vision tasks.
- Compared against proprietary large language models (LLM) APIs using metrics like MML score.
- Evaluations included automated base model evaluations and blind third-party human evaluations.
- Tested on benchmarks such as GSM 8K, HumanEval, GPQA, VQA V2, and MMU.
- Evaluated on text-only chat, multimodal chat, video question answering, and long context question answering tasks.
- Cross-lingual evaluations and medical reasoning tasks were also part of the testing process.
- Raika Core approached GPT-4V performance levels on MMLU, VQA2, and multimodal chat evaluations.
- Outperformed models like Claude 3, Opus, Sonet, and Haiku on multimodal chat human evaluation.
- Raika Core ranked third on the internal leaderboard for text-on-chat tasks.
- Limitations include significant computational resources needed for deployment and inference.
- Training data knowledge cutoff of November 2023 may limit adaptation to newer data trends.
- Performance may vary depending on the specific task or domain.

# INSIGHTS:
- Raika models achieve high performance with fewer parameters than larger models like GPT-4V.
- Multimodal capabilities are a key strength of Raika models, excelling in chat evaluations.
- Modular encoder-decoder architecture supports diverse input types: text, image, video, audio.
- Training involves diverse datasets with a significant portion being multilingual content.
- Advanced architecture features like Su glue grouped query attention enhance model performance.
- Comprehensive validation includes automated and blind human evaluations across various benchmarks.
- Raika Core ranks highly in text-on-chat tasks, showcasing its language processing capabilities.
- Significant computational resources are required for deploying Raika Edge and Flash models.
- Training data cutoff may limit the model's ability to adapt to new data trends post-November 2023.
- Continuous improvements are ongoing to address existing limitations in performance.

# QUOTES:
- "Raika models excel in both automated base model evaluations and blind third-party human evaluations."
- "Designed to outperform larger models like GPT-4V and Gemini Ultra in language and vision tasks."
- "Focus on improving multimodal capabilities, excelling in multimodal chat evaluations."
- "Developed to be powerful and competitive on a compute class basis."
- "Training involves ingesting diverse datasets, including text, images, videos, and audio clips."
- "Training data includes 25% code-related, 30% STEM-related, 25% web crawl data, and 10% math-related content."
- "About 15% of pre-training data is multilingual with 32 diverse languages."
- "Models use a modular encoder-decoder architecture supporting text, image, video, and audio inputs."
- "Backbone Transformer model utilizes Su glue grouped query attention, rotary positional embeddings, and RMS Norm."
- "Regular models have a context length of 8K; long context models have 128K."
- "Synthetic creation of supervised fine-tuning data using reverse instruction tuning from long documents."
- "Trained predominantly on Nvidia H100s using PyTorch with clusters from various vendors."
- "Peak compute involves approximately 2.5K H100s and 2.5K A100s."
- "Optimized for quality, diversity, and scale with a focus on improving IO performance using SEF file system."
- "Superior performance across a range of language and vision tasks within their compute class."
- "More computationally efficient and cost-effective compared to other models in the same compute class."
- "Advanced architecture features enhance modeling capabilities and overall performance."
- "Validated through comprehensive evaluations on language and vision tasks."
- "Compared against proprietary large language models (LLM) APIs using metrics like MML score."
- "Evaluations included automated base model evaluations and blind third-party human evaluations."

# HABITS:
- Ingesting diverse datasets including text, images, videos, and audio clips for training models.
- Utilizing a modular encoder-decoder architecture for supporting multiple input types efficiently.
- Employing advanced architecture features like Su glue grouped query attention for better performance.
- Optimizing training processes for quality, diversity, and scale with a focus on IO performance.
- Conducting comprehensive evaluations including automated base model evaluations and blind human assessments.

# FACTS:
- Raika models are designed to outperform larger models like GPT-4V in language and vision tasks.
- Training data includes approximately 25% code-related content and 30% STEM-related content.
- About 15% of pre-training data is multilingual with 32 diverse languages weighted by frequency.
- Regular Raika models have a context length of 8K; long context models have 128K.
- Peak compute for training involves approximately 2.5K H100s and 2.5K A100s.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
Raika models offer state-of-the-art performance in language and vision tasks with fewer parameters than larger models.

# RECOMMENDATIONS:
- Utilize Raika models for efficient language and vision task performance with fewer computational resources required.
- Leverage the modular encoder-decoder architecture for supporting diverse input types effectively.
- Optimize training processes focusing on quality, diversity, scale, and IO performance improvements.
- Conduct comprehensive evaluations including automated base model assessments and blind human evaluations.