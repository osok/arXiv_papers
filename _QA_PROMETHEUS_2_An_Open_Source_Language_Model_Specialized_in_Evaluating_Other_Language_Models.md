# SUMMARY
The new method addresses the limited flexibility and weak performance of open evaluator language models (LMs) by unifying direct assessment and pairwise ranking paradigms.

# IDEAS:
- The new method addresses limited flexibility and weak evaluation performances of open evaluator language models.
- It aims to bridge the gap by unifying direct assessment and pairwise ranking paradigms.
- The method creates a unified evaluator LM by merging weights of separately trained evaluator LMs.
- This approach enhances evaluation capabilities, making them more versatile and effective.
- Two base models, mistol 7B and mixol 8x 7B, are trained on different feedback data sets.
- Weights are merged using a linear technique with a coefficient Alpha set to 0.5.
- The unified evaluator LM, Prometheus 2, excels in both direct assessment and pairwise ranking.
- Weight merging outperforms joint training by showing positive task transfer and improved performance.
- Techniques like task arithmetic merging and D merging resolve disagreements and remove redundant weights.
- Unifying direct assessment and pairwise ranking handles diverse real-life scenarios effectively.
- The unified LM works in both formats and outperforms single-format trained evaluator LMs.
- Prometheus 2 models show high correlations with human evaluators and proprietary LM-based judges.
- This unification allows for a more comprehensive evaluation process.
- The unified evaluator LM can handle a wider range of evaluation criteria beyond generic qualities.
- Prometheus 2 models were validated by comparing performance with human evaluators and proprietary LMs.
- Correlation coefficients measured agreement between Prometheus 2 models and human evaluators or proprietary LMs.
- Prometheus 2 consistently outperformed existing open evaluator LMs in all data sets.
- They excelled in both direct assessment and pairwise ranking benchmarks.
- Prometheus 2 reduced the performance gap with GPT-4 by half on pairwise ranking benchmarks.
- Specific results showed highest correlation with human evaluators and proprietary LM-based judges.
- Prometheus 2 surpassed other baselines by 0.2 units across all data sets.
- Limitations include that merging LMs trained on the same format may not improve performance.
- Optimal Alpha value may vary, introducing complexity and requiring fine-tuning.
- Weight merging may not fully address robustness across diverse real-life scenarios.

# INSIGHTS:
- Unifying direct assessment and pairwise ranking enhances evaluator LMs' versatility and effectiveness.
- Weight merging combines strengths of different models, outperforming joint training methods.
- Prometheus 2 models show high agreement with human evaluators, reducing gaps with proprietary LMs.
- Comprehensive evaluation processes benefit from handling diverse real-life scenarios effectively.
- Techniques like task arithmetic merging resolve disagreements, enhancing overall performance.

# QUOTES:
- "The new method addresses limited flexibility and weak evaluation performances of open evaluator language models."
- "It aims to bridge the gap by unifying direct assessment and pairwise ranking paradigms."
- "This approach enhances evaluation capabilities, making them more versatile and effective."
- "Weights are merged using a linear technique with a coefficient Alpha set to 0.5."
- "The unified evaluator LM, Prometheus 2, excels in both direct assessment and pairwise ranking."
- "Weight merging outperforms joint training by showing positive task transfer and improved performance."
- "Unifying direct assessment and pairwise ranking handles diverse real-life scenarios effectively."
- "Prometheus 2 models show high correlations with human evaluators and proprietary LM-based judges."
- "This unification allows for a more comprehensive evaluation process."
- "Prometheus 2 consistently outperformed existing open evaluator LMs in all data sets."
- "They excelled in both direct assessment and pairwise ranking benchmarks."
- "Prometheus 2 reduced the performance gap with GPT-4 by half on pairwise ranking benchmarks."
- "Specific results showed highest correlation with human evaluators and proprietary LM-based judges."
- "Prometheus 2 surpassed other baselines by 0.2 units across all data sets."
- "Limitations include that merging LMs trained on the same format may not improve performance."

# HABITS:
- Regularly validate models by comparing performance with human evaluators and proprietary LMs.
- Use correlation coefficients to measure agreement between models and human evaluators or proprietary LMs.
- Fine-tune the coefficient Alpha in the linear merging process for optimal results.

# FACTS:
- The new method addresses limited flexibility and weak evaluation performances of open evaluator language models.
- Two base models, mistol 7B and mixol 8x 7B, are trained on different feedback data sets.
- Weights are merged using a linear technique with a coefficient Alpha set to 0.5.
- Prometheus 2 models show high correlations with human evaluators and proprietary LM-based judges.

# REFERENCES:
- Mistol 7B
- Mixol 8x 7B
- Prometheus 2
- GPT 41106
- Claude 3 Opus

# ONE-SENTENCE TAKEAWAY
Unifying direct assessment and pairwise ranking paradigms significantly enhances the versatility and effectiveness of evaluator language models.

# RECOMMENDATIONS:
- Unify direct assessment and pairwise ranking paradigms for versatile evaluator language models.
- Merge weights of separately trained evaluator LMs using a linear technique with coefficient Alpha set to 0.5.
- Validate models by comparing performance with human evaluators and proprietary LMs.
