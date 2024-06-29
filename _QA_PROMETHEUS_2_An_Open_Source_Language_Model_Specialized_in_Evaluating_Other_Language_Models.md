# SUMMARY
The new method addresses the limited flexibility and weak evaluation performances of open evaluator language models (LMs) in diverse real-life scenarios by unifying direct assessment and pairwise ranking paradigms to create a robust unified evaluator LM.

# IDEAS:
- The new method addresses limited flexibility and weak evaluation performances of open evaluator language models.
- It aims to bridge the gap by unifying direct assessment and pairwise ranking paradigms.
- The method merges weights of evaluator LMs trained on direct assessment and pairwise ranking formats.
- This creates a unified evaluator LM that excels in both schemes and outperforms existing open evaluator LMs.
- Enhances evaluation capabilities of open evaluator LMs, making them versatile and effective.
- Two base models, mistol 7B and mixol 8x 7B, are trained on feedback and preference data sets.
- Weights are merged using a linear merging technique with a coefficient Alpha set to 0.5.
- The unified evaluator LM is named Prometheus 2 7B and 8x 7B.
- Weight merging combines strengths of both models, outperforming joint training methods.
- Techniques like task arithmetic merging, ties merging, and D merging resolve disagreements and remove redundant weights.
- Unifying direct assessment and pairwise ranking handles diverse real-life scenarios effectively.
- The unified LM works in both formats and outperforms single-format trained evaluator LMs.
- Prometheus 2 models show high correlations with human evaluators and proprietary LM-based judges.
- The unification allows for a comprehensive evaluation process excelling in both assessment schemes.
- The unified evaluator LM can handle a wider range of evaluation criteria beyond generic qualities.
- Prometheus 2 models were validated by comparing performance with human evaluators and proprietary LM-based judges.
- Validation involved assessing correlation with human evaluators and proprietary LMs like GPT-4 and Claude 3 Opus.
- Prometheus 2 models consistently outperformed existing open evaluator LMs in all data sets.
- Evaluated on direct assessment benchmarks like vacuna bench, mount bench, flask, feedback bench.
- Evaluated on pairwise ranking benchmarks like HHH alignment, mount bench, human judgment, Auto jval, preference bench.
- Prometheus 2 models exhibited highest agreement with human evaluators among all open evaluator LMs tested.
- Reduced performance gap with GPT-4 by half on pairwise ranking benchmarks.
- Achieved highest correlation with human evaluators and proprietary LM-based judges on direct assessment benchmarks.
- Surpassed other baselines by 0.2 units across all data sets.
- Showed highest agreement with human evaluators among all open evaluator LMs tested.
- Limitations include merging LMs trained on the same format not necessarily improving performance.
- Optimal Alpha value may vary depending on specific benchmarks and metrics used.
- Weight merging approach may not fully address challenges related to robustness across diverse scenarios.

# INSIGHTS:
- Unifying direct assessment and pairwise ranking enhances evaluation capabilities of open evaluator LMs significantly.
- Weight merging combines strengths of models, outperforming joint training methods in evaluation tasks.
- Prometheus 2 models show high correlations with human evaluators and proprietary LM-based judges.
- Unified evaluator LMs handle diverse real-life scenarios effectively, excelling in both assessment schemes.
- Techniques like task arithmetic merging resolve disagreements and remove redundant weights in task vectors.
- Prometheus 2 models reduce performance gap with GPT-4 by half on pairwise ranking benchmarks.
- Unified evaluator LMs can handle a wider range of evaluation criteria beyond generic qualities.
- Merging LMs trained on the same format may not improve performance and could harm it on average.
- Optimal Alpha value in weight merging requires fine-tuning for different scenarios and benchmarks.
- Weight merging approach may not fully address robustness across diverse real-life scenarios.

# QUOTES:
- "The new method addresses limited flexibility and weak evaluation performances of open evaluator language models."
- "It aims to bridge the gap by unifying direct assessment and pairwise ranking paradigms."
- "This creates a unified evaluator LM that excels in both schemes and outperforms existing open evaluator LMs."
- "Enhances evaluation capabilities of open evaluator LMs, making them versatile and effective."
- "Weights are merged using a linear merging technique with a coefficient Alpha set to 0.5."
- "Weight merging combines strengths of both models, outperforming joint training methods."
- "Techniques like task arithmetic merging, ties merging, and D merging resolve disagreements."
- "Unifying direct assessment and pairwise ranking handles diverse real-life scenarios effectively."
- "Prometheus 2 models show high correlations with human evaluators and proprietary LM-based judges."
- "The unification allows for a comprehensive evaluation process excelling in both assessment schemes."
- "Prometheus 2 models were validated by comparing performance with human evaluators and proprietary LM-based judges."
- "Prometheus 2 models consistently outperformed existing open evaluator LMs in all data sets."
- "Prometheus 2 models exhibited highest agreement with human evaluators among all open evaluator LMs tested."
- "Reduced performance gap with GPT-4 by half on pairwise ranking benchmarks."
- "Achieved highest correlation with human evaluators and proprietary LM-based judges on direct assessment benchmarks."
- "Surpassed other baselines by 0.2 units across all data sets."
- "Showed highest agreement with human evaluators among all open evaluator LMs tested."
- "Limitations include merging LMs trained on the same format not necessarily improving performance."
- "Optimal Alpha value may vary depending on specific benchmarks and metrics used."
- "Weight merging approach may not fully address challenges related to robustness across diverse scenarios."

# HABITS:
- Regularly validate models by comparing performance with human evaluators and proprietary LM-based judges.
- Use techniques like task arithmetic merging to resolve disagreements in task vectors.

# FACTS:
- Prometheus 2 models reduce performance gap with GPT-4 by half on pairwise ranking benchmarks.
- Achieved highest correlation with human evaluators on direct assessment benchmarks, surpassing other baselines by 0.2 units.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
Unifying direct assessment and pairwise ranking paradigms significantly enhances the evaluation capabilities of open evaluator language models.

# RECOMMENDATIONS:
- Unify direct assessment and pairwise ranking paradigms to enhance evaluation capabilities of language models.
- Merge weights of separately trained evaluator LMs using a linear merging technique for better performance.
- Use techniques like task arithmetic merging to resolve disagreements in task vectors effectively.
