# SUMMARY
The section discusses leveraging Retrieval Augmented Generation (RAG) to enhance the trustworthiness of a commercial application that converts natural language into workflows, aiming to reduce hallucination and improve output quality.

# IDEAS:
- RAG aims to reduce hallucination in generating workflows from natural language inputs.
- Workflows are represented as JSON documents with each step as an adjacent object.
- Fine-tuning large language models can lead to hallucination, especially with out-of-distribution inputs.
- RAG retrieves relevant JSON objects to enhance the validity and executability of generated workflows.
- The retriever aligns semantics between natural language queries and structured JSON objects.
- Structured output tasks like text-to-code or text-to-SQL conversion require interpretable and executable output.
- Guided generation using outlines can help generate steps within a given context.
- RAG can maintain performance without sacrificing accuracy by deploying a smaller LLM with a minimal retriever model.
- The retriever suggests steps and tables which are added to the user query to form the LLM prompt.
- The LLM generates the workflow in JSON format through greedy decoding.
- Training the retriever encoder aligns natural language with JSON objects.
- The risk of hallucination arises from step names and database table names.
- Fine-tuning the retriever model enhances alignment between text and JSON objects.
- A Siamese Transformer encoder with mean pooling encodes user queries, steps, and tables into fixed-length vectors.
- The retriever is trained on pairs of user queries and corresponding steps or tables.
- The retriever retrieves the top K steps and tables based on cosine similarity.
- Fine-tuning the LLM involves incorporating the retriever's output in JSON format into the LLM input.
- The approach simplifies the structured output task for the LLM.
- Evaluation metrics include trigger exact match, bag of steps, hallucinated tables, and hallucinated steps.
- Fine-tuning different sizes of LLMs and retriever encoders measures their impact on system performance.
- Scaling up model size helps improve certain metrics, especially with RAG.
- Larger models tend to perform better and hallucinate less compared to smaller models.
- Pre-training on a large amount of natural language data may not be beneficial for this task.
- Removing suggestions during evaluation significantly drops model performance.
- Errors in generated workflows can stem from issues in both the retriever and the language model.
- Breaking down queries into shorter texts can improve retriever performance.
- Synthetic data generation can help address logic-based errors in the language model.
- Using a 7B parameter model allows for larger batch sizes and increased system throughput.
- Decoupling the retriever and language model enables easier reuse and independent optimization.

# INSIGHTS:
- RAG reduces hallucination by retrieving relevant JSON objects for workflow generation.
- Fine-tuning large language models risks hallucination, especially with out-of-distribution inputs.
- Structured output tasks require interpretable and executable outputs, making them challenging.
- Deploying a smaller LLM with a minimal retriever model maintains performance without sacrificing accuracy.
- Training the retriever encoder aligns natural language with JSON objects, reducing hallucination risks.
- Fine-tuning significantly improves retrieval results and domain-specific representation.
- Larger models perform better and hallucinate less compared to smaller models in RAG tasks.
- Pre-training on extensive natural language data may not benefit domain-specific tasks like workflow generation.
- Removing retriever suggestions during evaluation significantly impacts model performance.
- Errors in generated workflows can be mitigated by breaking down queries and using synthetic data.

# QUOTES:
- "RAG aims to reduce hallucination in generating workflows from natural language inputs."
- "Workflows are represented as JSON documents with each step as an adjacent object."
- "Fine-tuning large language models can lead to hallucination, especially with out-of-distribution inputs."
- "RAG retrieves relevant JSON objects to enhance the validity and executability of generated workflows."
- "The retriever aligns semantics between natural language queries and structured JSON objects."
- "Structured output tasks like text-to-code or text-to-SQL conversion require interpretable and executable output."
- "Guided generation using outlines can help generate steps within a given context."
- "RAG can maintain performance without sacrificing accuracy by deploying a smaller LLM with a minimal retriever model."
- "The retriever suggests steps and tables which are added to the user query to form the LLM prompt."
- "The LLM generates the workflow in JSON format through greedy decoding."
- "Training the retriever encoder aligns natural language with JSON objects."
- "The risk of hallucination arises from step names and database table names."
- "Fine-tuning the retriever model enhances alignment between text and JSON objects."
- "A Siamese Transformer encoder with mean pooling encodes user queries, steps, and tables into fixed-length vectors."
- "The retriever is trained on pairs of user queries and corresponding steps or tables."
- "The retriever retrieves the top K steps and tables based on cosine similarity."
- "Fine-tuning the LLM involves incorporating the retriever's output in JSON format into the LLM input."
- "The approach simplifies the structured output task for the LLM."
- "Evaluation metrics include trigger exact match, bag of steps, hallucinated tables, and hallucinated steps."
- "Fine-tuning different sizes of LLMs and retriever encoders measures their impact on system performance."

# HABITS:
- Fine-tuning large language models for domain-specific tasks to ensure accuracy and reduce hallucination.
- Training a retriever encoder to align natural language with structured JSON objects for better workflow generation.
- Using a Siamese Transformer encoder with mean pooling to encode user queries, steps, and tables into vectors.
- Fine-tuning the retriever model to enhance alignment between text and JSON objects for domain representation.
- Breaking down queries into shorter texts for more precise retrieval by the retriever.

# FACTS:
- RAG reduces hallucination by retrieving relevant JSON objects for workflow generation.
- Fine-tuning large language models risks hallucination, especially with out-of-distribution inputs.
- Structured output tasks require interpretable and executable outputs, making them challenging.
- Deploying a smaller LLM with a minimal retriever model maintains performance without sacrificing accuracy.
- Training the retriever encoder aligns natural language with JSON objects, reducing hallucination risks.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
RAG reduces hallucination in workflow generation by retrieving relevant JSON objects, enhancing validity and executability.

# RECOMMENDATIONS:
- Use RAG to reduce hallucination in generating workflows from natural language inputs effectively.
- Represent workflows as JSON documents with each step as an adjacent object for clarity.
- Fine-tune large language models cautiously to avoid hallucination, especially with out-of-distribution inputs.
- Retrieve relevant JSON objects to enhance the validity and executability of generated workflows.
- Align semantics between natural language queries and structured JSON objects using a trained retriever.