# SUMMARY
The paper discusses the challenges in evaluating generative language models, comparing a panel of LLM evaluators (Poll) to a single large judge like GPT-4.

# IDEAS:
- Evaluating generative language models is challenging due to finding meaningful data and assessing response correctness.
- Multiple-choice datasets like MMLU sidestep generation evaluation but probe different properties.
- Automatic metrics like BLEU and ROUGE often fail to analyze intended properties, causing false positives/negatives.
- Recent methods use trained or prompted models as evaluators to address evaluation issues.
- Poll consists of multiple evaluator models from different families, reducing intra-model bias.
- Poll uses a voting function to aggregate scores, mitigating individual model biases.
- Poll is over seven times cheaper than using a single GPT-4 judge.
- Poll correlates better with human judgments across various tasks compared to a single large judge.
- Single point scoring rates the quality of a single model output independently.
- Reference-based scoring involves scoring based on alignment with a gold reference.
- Pairwise scoring compares two outputs and assigns a preference score.
- Poll helps reduce in-model bias present in single judge models like GPT-4.
- Poll provides a more cost-effective solution for evaluation tasks.
- Poll offers better generalization across different tasks than a single judge model.
- Poll enhances accuracy and consistency of evaluations across various datasets.
- Running Poll is 7 to 8 times less expensive than running a single GPT-4 judge.
- Parallel processing of smaller models in Poll is expected to be faster than using a single large model.
- GPT-4 tends to recognize and prefer its own outputs, indicating self-preference bias.
- GPT-4 shows high variance with minor prompt changes, leading to inconsistent performance.
- GPT-4 may over-reason and inject too much background knowledge into evaluations.
- Intra-model bias in GPT-4 can lead to skewed evaluations not reflecting true response quality.

# INSIGHTS:
- Evaluating generative models is complex due to data and correctness assessment challenges.
- Multiple-choice datasets probe different properties than free-form generative tasks.
- Automatic metrics often fail to capture intended properties, leading to evaluation errors.
- Using multiple evaluator models reduces bias and provides diverse evaluation perspectives.
- Aggregating scores from multiple judges mitigates individual model biases effectively.
- Cost-effectiveness and scalability are significant advantages of using Poll over GPT-4.
- Poll's correlation with human judgments indicates its effectiveness in diverse tasks.
- Different scoring settings provide varied perspectives on model output quality.
- Reducing in-model bias leads to more objective and reliable evaluations.
- Parallel processing in Poll enhances evaluation efficiency compared to single large models.

# QUOTES:
- "Evaluating generative language models is challenging due to finding meaningful data and assessing response correctness."
- "Multiple-choice datasets like MMLU sidestep generation evaluation but probe different properties."
- "Automatic metrics like BLEU and ROUGE often fail to analyze intended properties, causing false positives/negatives."
- "Recent methods use trained or prompted models as evaluators to address evaluation issues."
- "Poll consists of multiple evaluator models from different families, reducing intra-model bias."
- "Poll uses a voting function to aggregate scores, mitigating individual model biases."
- "Poll is over seven times cheaper than using a single GPT-4 judge."
- "Poll correlates better with human judgments across various tasks compared to a single large judge."
- "Single point scoring rates the quality of a single model output independently."
- "Reference-based scoring involves scoring based on alignment with a gold reference."
- "Pairwise scoring compares two outputs and assigns a preference score."
- "Poll helps reduce in-model bias present in single judge models like GPT-4."
- "Poll provides a more cost-effective solution for evaluation tasks."
- "Poll offers better generalization across different tasks than a single judge model."
- "Poll enhances accuracy and consistency of evaluations across various datasets."
- "Running Poll is 7 to 8 times less expensive than running a single GPT-4 judge."
- "Parallel processing of smaller models in Poll is expected to be faster than using a single large model."
- "GPT-4 tends to recognize and prefer its own outputs, indicating self-preference bias."
- "GPT-4 shows high variance with minor prompt changes, leading to inconsistent performance."
- "GPT-4 may over-reason and inject too much background knowledge into evaluations."

# HABITS:
N/A

# FACTS:
N/A

# REFERENCES:
N/A

# ONE-SENTENCE TAKEAWAY
Using a panel of LLM evaluators (Poll) offers cost-effective, unbiased, and accurate evaluations compared to a single large judge like GPT-4.

# RECOMMENDATIONS:
- Use multiple evaluator models from different families to reduce intra-model bias effectively.
- Aggregate scores from multiple judges to mitigate individual model biases efficiently.
- Opt for cost-effective solutions like Poll for scalable evaluation tasks.
- Employ different scoring settings for varied perspectives on model output quality.
- Leverage parallel processing of smaller models for faster evaluation efficiency.