# SUMMARY
The paper introduces Super Context, a method enhancing in-context learning in large language models (LLMs), outperforming traditional methods across various natural language understanding tasks.

# IDEAS:
- Super Context enhances in-context learning in large language models (LLMs) by incorporating auxiliary knowledge.
- The method achieves an average performance of 80.5%, compared to 79.86% for LLMs alone.
- Super Context includes a small discriminative model's prediction and confidence in the LLM prompt.
- The unique prompt design inserts a receipt between the question-answer pair.
- The receipt provides the discriminative model's prediction and confidence and explains the prediction.
- Super Context questions LLMs about which in-context example it learned from.
- The method evaluates on various natural language understanding (NLU) tasks.
- Tasks include sentiment analysis, natural language inference, paraphrasing, and question answering.
- Super Context outperforms baseline methods like 16-shot in-context learning and BM25.
- Demonstrations during the inference stage influence performance.
- ChatGPT shows a decreasing attention trend for in-context examples.
- InstructGPT shows a U-shaped occurrence pattern for in-context examples.
- Super Context generates output rationale to explain LLM predictions.
- Higher average rationale overlap with humans is achieved by Super Context.
- Rationale overlap is 0.575 for Super Context compared to 0.45 for 16-shot ChatGPT.
- Positive correlation exists between discriminative model confidence and LLM prediction performance.
- Including discriminative model confidence improves performance of ChatGPT and LLaMA 2 7B Chat.
- Super Context significantly improves exact match and accuracy for open questions in SQuAD 2.0 dataset.
- Accuracy for open questions improved from 32.35% (ChatGPT) to 54.65% (Super Context).
- Findings highlight improvements, modifications, and achievements of Super Context.

# INSIGHTS:
- Super Context enhances LLMs by integrating auxiliary knowledge from a discriminative model.
- Unique prompt design with a receipt improves LLM performance on new tasks.
- Evaluations show Super Context outperforms traditional in-context learning methods.
- Demonstrations during inference stage affect LLM attention patterns differently.
- Super Context's rationale generation aligns more closely with human understanding.
- Discriminative model confidence positively impacts LLM prediction accuracy.
- Significant improvement in open question accuracy with Super Context on SQuAD 2.0 dataset.

# QUOTES:
- "Our method outperforms traditional and context learning methods achieving an average performance of 80.5%."
- "We include the discriminative model's prediction and confidence in the prompt for the LLM."
- "Super Context generates output rationale to explain the LLM predictions."
- "We found that Super Context achieves a higher average rationale overlap of 0.575 with humans."
- "Including the discriminative model's confidence in the prompt design of Super Context improves performance."
- "Accuracy for open questions improved from 32.35% (ChatGPT) to 54.65% (Super Context)."
- "ChatGPT shows a decreasing attention trend for in-context examples."
- "InstructGPT shows a U-shaped occurrence pattern for in-context examples."
- "Super Context outperforms other baseline methods such as 16-shot in-context learning and BM25."
- "Our findings highlight the improvements, modifications, and achievements of Super Context."

# HABITS:
- Incorporate auxiliary knowledge from a small discriminative model into LLM prompts.
- Design unique prompts that include predictions and confidence levels from discriminative models.
- Evaluate methods on a variety of natural language understanding tasks for comprehensive assessment.
- Analyze the influence of demonstrations during the inference stage on model performance.
- Generate output rationales to explain predictions and align them with human understanding.

# FACTS:
- Super Context achieves an average performance of 80.5%, outperforming traditional methods.
- The method includes a small discriminative model's prediction and confidence in the prompt.
- Evaluated on tasks like sentiment analysis, natural language inference, and question answering.
- ChatGPT shows a decreasing attention trend for in-context examples during inference.
- InstructGPT shows a U-shaped occurrence pattern for in-context examples during inference.
- Rationale overlap with humans is 0.575 for Super Context compared to 0.45 for 16-shot ChatGPT.
- Including discriminative model confidence improves performance of ChatGPT and LLaMA 2 7B Chat.

# REFERENCES:
- SQuAD 2.0 dataset
- ChatGPT
- InstructGPT
- LLaMA 2 7B Chat

# ONE-SENTENCE TAKEAWAY
Super Context significantly enhances large language models' performance by integrating auxiliary knowledge and unique prompt designs.

# RECOMMENDATIONS:
- Integrate auxiliary knowledge from discriminative models to enhance LLM performance on new tasks.
- Use unique prompt designs that include predictions and confidence levels from discriminative models.
- Evaluate methods on diverse natural language understanding tasks for comprehensive assessment.
- Analyze the influence of demonstrations during inference to understand attention patterns.
- Generate output rationales to explain predictions and align them with human understanding.