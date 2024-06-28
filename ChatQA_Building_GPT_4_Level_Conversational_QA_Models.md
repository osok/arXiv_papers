# SUMMARY
The paper introduces CH AQ q a7b, a conversational QA model matching GP4's accuracy through a two-step instruction tuning process, improved retriever, and meticulous data curation.

# IDEAS:
- Conversational QA models allow users to interact in a conversational manner, making follow-up questions easy.
- These models generate answers without needing specific fine-tuning for each data set.
- They can incorporate retrieved information in both open domain or long document settings.
- Creating a conversational QA model matching top-tier models like GP4 remains challenging.
- CH AQ q a7b achieves GP4-level accuracy through a two-step instruction tuning process.
- An improved retriever for retrieval augmented generation enhances conversational QA.
- Meticulous data curation significantly enhances the language model's ability to integrate context.
- The method outperforms regular instruction tuning or RHF-based methods for retrieval augmented generation.
- Fine-tuning state-of-the-art single-turn query retrievers on multi-turn QA data is effective.
- Chat QA 70b model outperforms GPT 3.5 turbo and GPT 4 in average score without synthetic data.
- Adding unanswerable samples in instruction tuning reduces hallucination in conversational QA.
- Many conversational QA data sets involve answering questions based on provided context or documents.
- Retrieval augmented generation is essential when documents are longer than the context window of the language model.
- Query rewriting methods rewrite the latest turn of question to be standalone for retrieval models.
- Two-stage instruction tuning involves supervised fine-tuning on instruction following and dialogue data sets.
- Context enhanced instruction tuning improves the model's ability to handle context-aware QA.
- Synthetic data generation using GPT 3.5 turbo creates high-quality data sets for fine-tuning language models.
- Fine-tuning a single-turn retriever using conversational query and context pairs enhances performance.
- Human annotated data leads to significant improvements on certain data sets with unanswerable cases.
- Using more context chunks doesn't always lead to better results; top five contexts are optimal.
- Fine-tuned retrievers improve average scores, especially in specific data sets like INSC.

# INSIGHTS:
- Conversational QA models enhance user experience by addressing follow-up questions and asking clarifications.
- Two-stage instruction tuning significantly improves conversational QA capabilities over given contexts.
- Synthetic data from GPT 3.5 turbo can effectively fine-tune language learning models for QA tasks.
- Fine-tuning single-turn retrievers on multi-turn QA data is as effective as top-tier query rewriting models.
- Adding unanswerable samples in instruction tuning guides models to generate "cannot answer" outputs.
- Human annotated data improves performance on unanswerable cases, enhancing overall model accuracy.
- Optimal context chunk retrieval balances finding correct answers without causing confusion.
- Fine-tuned retrievers significantly enhance question answering performance compared to non-fine-tuned versions.
- Human evaluations confirm strong performance of CH AQ q a7b, comparable to GPT 4 in many tasks.
- Incorporating single-turn QA data sets in training blends enhances multi-turn QA capabilities.

# QUOTES:
- "Conversational QA models allow users to interact in a conversational manner, making it easy to ask follow-up questions."
- "Creating a conversational QA model that can match the accuracy of top-tier models like GP4 remains a significant challenge."
- "We achieve this through a two-step instruction tuning process, an improved retriever, and meticulous data curation."
- "Our method outperforms regular instruction tuning or RHF-based methods for retrieval augmented generation in conversational QA."
- "Adding a small number of unanswerable samples in instruction tuning can guide the model to generate a 'cannot answer' output."
- "Many conversational QA data sets have been introduced where the models are asked to answer questions based on provided context or documents."
- "Instruction tuning has become a key component in building state-of-the-art dialogue agents which can handle a wide range of tasks without any prior training."
- "We found that simply adding the top K retrieved chunks for language model fine-tuning doesn't help much for a wide range of conversation QA tasks."
- "Synthetic data generation using GPT 3.5 turbo creates high-quality data sets for fine-tuning language learning models."
- "Fine-tuning state-of-the-art single-turn query retrievers on human annotated multi-turn QA data set is as effective as using the top-tier language model based query rewriting model GPT 3.5 turbo."
- "Our chat QA 70b model outperforms GPT 3.5 turbo and GPT 4 in terms of average score without using any synthetic data from chat GPT models."
- "We also explore the unanswerable scenario where the desired answer is not included in the provided or retrieved context."
- "We show that adding a small number of unanswerable samples in instruction tuning can guide the model to generate a 'cannot answer' output when necessary, significantly reducing hallucination."
- "Conversational QA improves user experiences by addressing follow-up questions and can also ask clarification questions from users if necessary, reducing hallucination."
- "Many conversational QA data sets have been introduced where the models are asked to answer questions based on provided context or documents."
- "The provided context or documents can be text only from various domains or plain text along with tables."
- "Conversational QA involves retrieval augmented generation in open domain setting or when the provided documents are longer than the context window of the language model."
- "The DSE retrievers are usually trained to retrieve the top K relevant chunks given a single question."
- "In conversational QA, follow-up questions may have insufficient information for retrieval while feeding them along with the dialogue history can be redundant and lead to suboptimal results."
- "Most previous solutions are query rewriting methods; the latest turn of question is rewritten to be a standalone query without additional information from previous dialogue history."

# HABITS:
- Regularly fine-tune language models on diverse instruction following and dialogue data sets.
- Integrate contextualized QA data sets into instruction tuning blends for enhanced performance.
- Use synthetic data generation tools like GPT 3.5 turbo for creating high-quality training data sets.
- Fine-tune single-turn retrievers using conversational query and context pairs for better retrieval performance.
- Include unanswerable samples in instruction tuning to guide models towards accurate responses.
- Conduct human evaluations to assess and compare model performance against benchmarks like GPT 4.
- Optimize context chunk retrieval by balancing between too few and too many chunks for best results.
- Continuously improve retriever quality through fine-tuning to enhance question answering accuracy.
- Incorporate single-turn QA data sets in training blends to improve multi-turn QA capabilities.

# FACTS:
- Conversational QA models allow users to interact in a conversational manner, making follow-up questions easy.
- These models generate answers without needing specific fine-tuning for each data set.
- They can incorporate retrieved information in both open domain or long document settings.
- Creating a conversational QA model matching top-tier models like GP4 remains challenging.
- CH AQ q a7b achieves GP4-level accuracy through a two-step instruction tuning process.
- An improved retriever for retrieval augmented generation enhances conversational QA.
- Meticulous data curation significantly enhances the language model's ability to integrate context.
- The method outperforms regular instruction tuning or RHF-based methods for retrieval augmented generation.
- Fine-tuning state-of-the-art single-turn query retrievers on multi-turn QA data is effective.
- Chat QA 70b model outperforms GPT 3.5 turbo and GPT 4 in average score without synthetic data.
- Adding unanswerable samples in instruction tuning reduces hallucination in conversational QA.
- Many conversational QA data sets involve answering questions based on provided context or documents.
- Retrieval augmented generation is essential when documents are longer than the context window of the language model.
- Query rewriting methods rewrite the latest turn of question to be standalone for retrieval models.

# REFERENCES:
None mentioned explicitly.

# ONE-SENTENCE TAKEAWAY
CH AQ q a7b achieves GP4-level accuracy through two-step instruction tuning, improved retriever, and meticulous data curation.

# RECOMMENDATIONS:
- Use conversational QA models for interactive user experiences with follow-up question capabilities.
- Generate answers without specific fine-tuning for each data set using advanced models like CH AQ q a7b.
- Incorporate retrieved information in both open domain or long document settings for better accuracy.
- Apply two-step instruction tuning processes to achieve top-tier model accuracy in conversational QA tasks.
- Enhance retriever quality through fine-tuning for improved retrieval augmented generation performance.
- Curate high-quality data meticulously to enhance language model's ability to integrate context effectively.
- Use synthetic data generation tools like GPT 3.5 turbo for creating high-quality training data sets.
- Fine-tune single-turn retrievers using conversational query and context pairs for better retrieval performance.
- Include unanswerable samples in instruction tuning to guide models towards accurate responses.
- Conduct human evaluations to assess and compare model performance against benchmarks like GPT 4.