# SUMMARY
The paper proposes enhancing conversational QA by addressing follow-up questions and reducing hallucination, using a two-stage instruction tuning method for better retrieval and context-aware generation.

# IDEAS:
- Conversational QA enhances user experiences by addressing follow-up questions and reducing hallucination.
- This approach has become the standard for deploying QA models in production.
- Follow-up questions may lack sufficient information for retrieval in conversational QA.
- Training a dense retriever to retrieve top K relevant chunks given a single question is suggested.
- Previous solutions for conversational QA include query rewriting methods and generative models.
- A two-stage instruction tuning method improves generation with retrieval or provided context.
- Zero-shot evaluation and fine-tuning a single-turn query retriever on multi-turn data sets are focused on.
- This straightforward approach yields comparable zero-shot results to state-of-the-art query rewriting models.
- Instruction tuning equips language models to follow natural language instructions.
- High-quality instruction tuning data sets are crucial for effective model training.
- A two-stage instruction tuning method is proposed for chat QA.
- Supervised fine-tuning is applied on a blend of instruction following and dialogue data sets in the first stage.
- Context-enhanced instruction tuning is introduced in the second stage for context-aware generation.
- A large supervised fine-tuning set is constructed by combining multiple high-quality instruction tuning data sets.
- Contextualized QA data sets are integrated into the instruction tuning blend in the second stage.
- Human-annotated and synthetic conversational QA data sets enhance the model's conversational QA capability.
- Fine-tuning a single-turn retriever using conversational query and context pairs is proposed.
- The effectiveness of fine-tuning is compared to query rewriting methods across five benchmark data sets.
- GPT 3.5 turbo is used as a conversational query rewriting model with task instructions and few-shot examples.
- Fine-tuning performs marginally worse than query rewriting in average top one recall.
- Fine-tuning achieves better results at average top five recall compared to query rewriting methods.
- Fine-tuning on high-quality conversational query context pairs performs on par with query rewriting methods.
- Fine-tuning avoids extra computational time and cost associated with autoregressive generation.

# INSIGHTS:
- Conversational QA reduces hallucination and enhances user experience by addressing follow-up questions effectively.
- Training dense retrievers for top K relevant chunks improves retrieval in conversational QA.
- Two-stage instruction tuning significantly enhances context-aware generation in conversational QA models.
- High-quality instruction tuning data sets are essential for effective language model training.
- Fine-tuning on conversational query context pairs performs comparably to query rewriting methods without extra costs.

# QUOTES:
- "Conversational QA enhances user experiences by addressing follow-up questions and reducing hallucination."
- "This approach has become the standard for deploying QA models in production."
- "Follow-up questions may lack sufficient information for retrieval in conversational QA."
- "Training a dense retriever to retrieve top K relevant chunks given a single question is suggested."
- "Previous solutions for conversational QA include query rewriting methods and generative models."
- "A two-stage instruction tuning method improves generation with retrieval or provided context."
- "Zero-shot evaluation and fine-tuning a single-turn query retriever on multi-turn data sets are focused on."
- "This straightforward approach yields comparable zero-shot results to state-of-the-art query rewriting models."
- "Instruction tuning equips language models to follow natural language instructions."
- "High-quality instruction tuning data sets are crucial for effective model training."
- "A two-stage instruction tuning method is proposed for chat QA."
- "Supervised fine-tuning is applied on a blend of instruction following and dialogue data sets in the first stage."
- "Context-enhanced instruction tuning is introduced in the second stage for context-aware generation."
- "A large supervised fine-tuning set is constructed by combining multiple high-quality instruction tuning data sets."
- "Contextualized QA data sets are integrated into the instruction tuning blend in the second stage."
- "Human-annotated and synthetic conversational QA data sets enhance the model's conversational QA capability."
- "Fine-tuning a single-turn retriever using conversational query and context pairs is proposed."
- "The effectiveness of fine-tuning is compared to query rewriting methods across five benchmark data sets."
- "GPT 3.5 turbo is used as a conversational query rewriting model with task instructions and few-shot examples."
- "Fine-tuning performs marginally worse than query rewriting in average top one recall."

# HABITS:
- Training dense retrievers to improve retrieval in conversational QA.
- Applying supervised fine-tuning on a blend of instruction following and dialogue data sets.
- Integrating contextualized QA data sets into the instruction tuning blend.
- Using human-annotated and synthetic conversational QA data sets for model enhancement.
- Fine-tuning single-turn retrievers using conversational query and context pairs.

# FACTS:
- Conversational QA reduces hallucination and enhances user experience by addressing follow-up questions effectively.
- Training dense retrievers for top K relevant chunks improves retrieval in conversational QA.
- Two-stage instruction tuning significantly enhances context-aware generation in conversational QA models.
- High-quality instruction tuning data sets are essential for effective language model training.
- Fine-tuning on conversational query context pairs performs comparably to query rewriting methods without extra costs.

# REFERENCES:
- GPT 3.5 turbo as a conversational query rewriting model.

# ONE-SENTENCE TAKEAWAY
Two-stage instruction tuning significantly enhances context-aware generation, improving conversational QA by addressing follow-up questions effectively.

# RECOMMENDATIONS:
- Train dense retrievers to improve retrieval in conversational QA systems effectively.
- Apply supervised fine-tuning on a blend of instruction following and dialogue data sets.
- Integrate contextualized QA data sets into the instruction tuning blend for better results.
- Use human-annotated and synthetic conversational QA data sets to enhance model capabilities.
- Fine-tune single-turn retrievers using conversational query and context pairs for better performance.