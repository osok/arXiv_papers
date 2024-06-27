# SUMMARY
The Raika models, including Core, Flash, and Edge, aim to advance language and vision tasks by providing efficient, powerful models that outperform larger models in various benchmarks.

# IDEAS:
- Raika models aim to advance state-of-the-art in language and vision tasks.
- They excel in both automated base model evaluations and blind third-party human evaluations.
- Designed to outperform larger models like GPT-4V and Gemini Ultra.
- Focused on improving multimodal capabilities, excelling in multimodal chat evaluations.
- Developed to be powerful and competitive on a compute class basis.
- Training involves ingesting a mixture of publicly available and proprietary datasets.
- Training data includes text, images, videos, and audio clips.
- Data set includes 25% code-related, 30% STEM-related, 25% web crawl data, and 10% math-related content.
- About 15% of pre-training data is multilingual with 32 diverse languages.
- Models use a modular encoder-decoder architecture supporting text, image, video, and audio inputs.
- Backbone Transformer model utilizes Su glue grouped query attention, rotary positional embeddings, and RMS Norm.
- Models trained with bf16 and have a context length of 8K for regular models.
- Long context models like Raika Flash and Core have 128K context length for long documents.
- Synthetic creation of supervised fine-tuning data using reverse instruction tuning from long documents.
- Training predominantly on Nvidia H100s using PyTorch with clusters from various vendors.
- Peak compute of approximately 2.5K H100s and 2.5K A100s.
- Training optimized for quality, diversity, and scale with a focus on improving IO performance.
- Raika models offer superior performance across a range of language and vision tasks.
- They are computationally efficient and cost-effective compared to other models in the same compute class.
- Advanced architecture features like s glue grouped query attention and RMS Norm enhance modeling capabilities.
- Validated through comprehensive evaluations on language and vision tasks.
- Evaluations included automated base model evaluations and blind third-party human evaluations.
- Compared against other Frontier models like GPT-4V, Claude 3 models, Gemini Ultra, Gemma 7B, and Mistol 7B.
- Evaluated on benchmarks such as GSM 8K, HumanEval, GPQA, VQA V2, and MMU.
- Tested on text-only chat, multimodal chat, video question answering, and long context question answering tasks.
- Raika Core achieved competitive results in language and vision tasks compared to other Frontier class models.
- Outperformed models like GPT-4V on MMLU, VQA2, and third-party multimodal chat evaluation.
- Limitations include the need for significant computational resources due to their dense nature.
- Training data knowledge cutoff of November 2023 may limit adaptability to newer data trends.

# INSIGHTS:
- Raika models excel in both automated base model evaluations and blind third-party human evaluations.
- Designed to outperform larger models like GPT-4V and Gemini Ultra in various benchmarks.
- Focused on improving multimodal capabilities, excelling in multimodal chat evaluations.
- Training involves ingesting a mixture of publicly available and proprietary datasets.
- Models use a modular encoder-decoder architecture supporting text, image, video, and audio inputs.
- Backbone Transformer model utilizes Su glue grouped query attention and RMS Norm.
- Long context models like Raika Flash and Core have 128K context length for long documents.
- Training predominantly on Nvidia H100s using PyTorch with clusters from various vendors.
- Raika models offer superior performance across a range of language and vision tasks.
- They are computationally efficient and cost-effective compared to other models in the same compute class.

# QUOTES:
- "Raika models aim to advance state-of-the-art in language and vision tasks."
- "They excel in both automated base model evaluations and blind third-party human evaluations."
- "Designed to outperform larger models like GPT-4V and Gemini Ultra."
- "Focused on improving multimodal capabilities, excelling in multimodal chat evaluations."
- "Developed to be powerful and competitive on a compute class basis."
- "Training involves ingesting a mixture of publicly available and proprietary datasets."
- "Training data includes text, images, videos, and audio clips."
- "Data set includes 25% code-related, 30% STEM-related, 25% web crawl data, and 10% math-related content."
- "About 15% of pre-training data is multilingual with 32 diverse languages."
- "Models use a modular encoder-decoder architecture supporting text, image, video, and audio inputs."
- "Backbone Transformer model utilizes Su glue grouped query attention, rotary positional embeddings, and RMS Norm."
- "Models trained with bf16 and have a context length of 8K for regular models."
- "Long context models like Raika Flash and Core have 128K context length for long documents."
- "Synthetic creation of supervised fine-tuning data using reverse instruction tuning from long documents."
- "Training predominantly on Nvidia H100s using PyTorch with clusters from various vendors."
- "Peak compute of approximately 2.5K H100s and 2.5K A100s."
- "Training optimized for quality, diversity, and scale with a focus on improving IO performance."
- "Raika models offer superior performance across a range of language and vision tasks."
- "They are computationally efficient and cost-effective compared to other models in the same compute class."

# HABITS:
- Ingesting a mixture of publicly available and proprietary datasets for training.
- Utilizing advanced architecture features like Su glue grouped query attention and RMS Norm.
- Training predominantly on Nvidia H100s using PyTorch with clusters from various vendors.

# FACTS:
- Raika models aim to advance state-of-the-art in language and vision tasks.
- They excel in both automated base model evaluations and blind third-party human evaluations.
- Designed to outperform larger models like GPT-4V and Gemini Ultra in various benchmarks.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
Raika models provide efficient, powerful solutions for language and vision tasks by outperforming larger models in various benchmarks.

# RECOMMENDATIONS:
- Focus on improving multimodal capabilities for better performance in multimodal chat evaluations.
