# SUMMARY
The paper addresses hallucination in using large language models (LLMs) for workflow generation, proposing Retrieval Augmented Generation (RAG) to improve accuracy and trustworthiness.

# IDEAS:
- Hallucination refers to generating non-existent steps or tables in workflows.
- Using LLMs naively can result in hallucinations, especially with out-of-distribution inputs.
- RAG incorporates a retriever to provide relevant information before generating text.
- The retriever is trained to align natural language with JSON objects.
- The retriever uses contrastive loss to minimize distance between positive and negative pairs.
- An index of steps and tables is built using FAISS during initialization.
- The retriever suggests steps and tables based on the natural language query.
- The LLM generates the workflow in JSON format via greedy decoding.
- RAG helps reduce hallucination and improve trustworthiness of generated workflows.
- RAG enhances output quality by retrieving relevant information before generating text.
- RAG enables customization of workflows by allowing users to specify requirements in natural language.
- RAG optimizes model deployment by enabling smaller LLMs while maintaining performance quality.
- RAG increases system accessibility by generating valid structured outputs from natural language inputs.
- RAG involves training a retriever model to align natural language with JSON objects.
- RAG supports in-context learning by providing relevant JSON objects to the LLM before generation.
- RAG aids in generating valid structured outputs from natural language queries.
- RAG fine-tuning improves overall system performance by reducing hallucination and increasing output quality.
- The retriever is trained using pairs of user queries and corresponding steps or tables.
- The retriever encoder uses a Siamese Transformer encoder with mean pooling.
- The LLM is trained separately from the retriever in a RAG fashion.
- The LLM is trained using standard supervised fine-tuning with the retriever's output aiding generation.
- Key metrics include Trigger Exact Match, Bag of Steps, Hallucinated Tables, and Hallucinated Steps.
- Recall@5 and Recall@10 are used to evaluate the retriever for steps and tables respectively.
- Scaling the size of off-the-shelf encoders did not yield significant improvements on retrieval metrics.
- Fine-tuning the encoder significantly improved performance, especially for smaller encoders.
- Larger LLMs can better copy and paste retrieved steps and tables during generation.
- Fine-tuning RAG models significantly reduced hallucination in generated workflows.
- The 7B version of the RAG fine-tuned model provided the best trade-off between performance and model size.
- Pre-training on large amounts of natural language data may be detrimental to specific tasks.

# INSIGHTS:
- Hallucination in LLMs can lead to unreliable and untrustworthy workflow outputs.
- RAG reduces hallucination by incorporating relevant information before text generation.
- Fine-tuning smaller LLMs with retriever output improves performance over larger off-the-shelf models.
- Customization of workflows is enhanced by allowing natural language specifications.
- Smaller LLMs can maintain high performance with RAG, optimizing infrastructure costs.

# QUOTES:
- "Hallucination refers to the generation of properties such as steps or tables that do not actually exist."
- "Using LLMs naively can result in hallucinations, especially when the natural language input is out of distribution."
- "RAG incorporates a retriever to provide relevant information before generating text."
- "The retriever is trained to align natural language with JSON objects."
- "The retriever uses contrastive loss to minimize distance between positive and negative pairs."
- "An index of steps and tables is built using FAISS during initialization."
- "The retriever suggests steps and tables based on the natural language query."
- "The LLM generates the workflow in JSON format via greedy decoding."
- "RAG helps reduce hallucination and improve trustworthiness of generated workflows."
- "RAG enhances output quality by retrieving relevant information before generating text."
- "RAG enables customization of workflows by allowing users to specify requirements in natural language."
- "RAG optimizes model deployment by enabling smaller LLMs while maintaining performance quality."
- "RAG increases system accessibility by generating valid structured outputs from natural language inputs."
- "RAG involves training a retriever model to align natural language with JSON objects."
- "RAG supports in-context learning by providing relevant JSON objects to the LLM before generation."
- "RAG aids in generating valid structured outputs from natural language queries."
- "RAG fine-tuning improves overall system performance by reducing hallucination and increasing output quality."
- "The retriever is trained using pairs of user queries and corresponding steps or tables."
- "The retriever encoder uses a Siamese Transformer encoder with mean pooling."
- "The LLM is trained separately from the retriever in a RAG fashion."

# HABITS:
- Training a retriever model using pairs of user queries and corresponding steps or tables.
- Using contrastive loss to minimize distance between positive and negative pairs during training.
- Building an index of steps and tables using FAISS during initialization.
- Suggesting steps and tables based on natural language queries for workflow generation.
- Generating workflows in JSON format via greedy decoding to ensure valid outputs.

# FACTS:
- Hallucination can lead to unreliable workflow outputs when using LLMs for structured tasks.
- RAG reduces hallucination by incorporating relevant information before text generation.
- Fine-tuning smaller LLMs with retriever output improves performance over larger off-the-shelf models.
- Customization of workflows is enhanced by allowing users to specify requirements in natural language.
- Smaller LLMs can maintain high performance with RAG, optimizing infrastructure costs.

# REFERENCES:
None mentioned explicitly.

# ONE-SENTENCE TAKEAWAY
Retrieval Augmented Generation (RAG) reduces hallucination in workflow generation, enhancing accuracy, trustworthiness, and customization capabilities.

# RECOMMENDATIONS:
- Use RAG to reduce hallucination in structured output tasks like workflow generation.
- Train a retriever model using pairs of user queries and corresponding steps or tables.
- Incorporate relevant information before generating text to improve output quality.
- Fine-tune smaller LLMs with retriever output for optimal performance and cost-efficiency.
- Allow users to specify workflow requirements in natural language for better customization.