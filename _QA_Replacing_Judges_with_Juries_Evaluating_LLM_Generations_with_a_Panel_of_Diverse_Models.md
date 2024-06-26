# SUMMARY
The paper discusses challenges in evaluating generative language models, proposing a panel of LLM evaluators (Poll) to address biases and improve cost-effectiveness.

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
- Reference-based scoring involves comparing the output to a gold reference.
- Pairwise scoring compares two outputs from different models, assigning a preference score.
- Poll helps reduce in-model bias present in single judge models like GPT-4.
- Poll provides a more cost-effective solution for evaluation tasks.
- Poll offers better generalization across different tasks than a single judge model.
- Poll enhances accuracy and consistency in evaluations compared to individual judges.
- Running Poll is 7 to 8 times less expensive than running a single GPT-4 judge.
- Parallel processing of smaller models in Poll is expected to be faster than using a single large model.
- Evaluator models like GPT-4 tend to have biases, favoring their own outputs.
- GPT-4 shows high variance with minor prompt changes, indicating inconsistency.
- GPT-4 may over-reason and inject too much background knowledge into evaluations.
- Intra-model bias in GPT-4 leads to skewed evaluations favoring its own outputs.

# INSIGHTS:
- Evaluating generative language models requires meaningful data and accurate response assessment methods.
- Multiple-choice datasets probe different properties than free-form generative tasks.
- Automatic metrics often fail to capture the intended properties of interest in evaluations.
- Using multiple evaluator models reduces intra-model bias and provides diverse perspectives.
- Aggregating scores from multiple judges mitigates individual model biases effectively.
- Poll is significantly more cost-effective and scalable than using a single large judge model.
- Poll's correlation with human judgments indicates its effectiveness in capturing intended properties.
- Different scoring settings provide varied perspectives on model performance across tasks.
- Reducing in-model bias leads to more objective and reliable evaluations.
- Parallel processing of smaller models enhances evaluation efficiency compared to a single large model.

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
- "Reference-based scoring involves comparing the output to a gold reference."
- "Pairwise scoring compares two outputs from different models, assigning a preference score."
- "Poll helps reduce in-model bias present in single judge models like GPT-4."
- "Poll provides a more cost-effective solution for evaluation tasks."
- "Poll offers better generalization across different tasks than a single judge model."
- "Poll enhances accuracy and consistency in evaluations compared to individual judges."
- "Running Poll is 7 to 8 times less expensive than running a single GPT-4 judge."
- "Parallel processing of smaller models in Poll is expected to be faster than using a single large model."
- "Evaluator models like GPT-4 tend to have biases, favoring their own outputs."
- "GPT-4 shows high variance with minor prompt changes, indicating inconsistency."
- "GPT-4 may over-reason and inject too much background knowledge into evaluations."

# HABITS:
- Using multiple evaluator models from different families reduces intra-model bias effectively.
- Aggregating scores from multiple judges mitigates individual model biases efficiently.
- Employing cost-effective solutions for scalable evaluation tasks enhances accessibility.
- Correlating model evaluations with human judgments ensures capturing intended properties accurately.
- Implementing varied scoring settings provides comprehensive perspectives on model performance.

# FACTS:
- Evaluating generative language models requires meaningful data and accurate response assessment methods.
- Multiple-choice datasets probe different properties than free-form generative tasks.
- Automatic metrics often fail to capture the intended properties of interest in evaluations.
- Using multiple evaluator models reduces intra-model bias and provides diverse perspectives.
- Aggregating scores from multiple judges mitigates individual model biases effectively.
- Poll is significantly more cost-effective and scalable than using a single large judge model.
- Poll's correlation with human judgments indicates its effectiveness in capturing intended properties.
- Different scoring settings provide varied perspectives on model performance across tasks.
- Reducing in-model bias leads to more objective and reliable evaluations.
- Parallel processing of smaller models enhances evaluation efficiency compared to a single large model.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
Using a panel of LLM evaluators (Poll) reduces bias, improves cost-effectiveness, and enhances evaluation accuracy.

# RECOMMENDATIONS:
- Use multiple evaluator models from different families to reduce intra-model bias effectively.
- Aggregate scores from multiple judges to mitigate individual model biases efficiently.
- Employ cost-effective solutions for scalable evaluation tasks to enhance accessibility.
- Correlate model evaluations with human judgments to ensure capturing intended properties accurately.
- Implement varied scoring settings to provide comprehensive perspectives on model performance.