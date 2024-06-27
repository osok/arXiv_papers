# SUMMARY
The study investigates task contamination in few-shot learning with large language models, revealing significant contamination and its impact on model performance.

# IDEAS:
- Few-shot methods like In-Context Learning (ICL) show impressive results with minimal data.
- Task contamination occurs when models have prior knowledge of unseen data or tasks.
- Closed models don't disclose pre-training data, making contamination assessment challenging.
- Open models' data may change, complicating contamination detection.
- The study evaluates 12 models on 16 classification tasks and one semantic parsing task.
- Data sets created before training data collection perform better than majority baselines.
- Classification tasks without contamination rarely show significant improvements over baselines.
- Membership inference attacks reveal strong correlation between extracted examples and model accuracy.
- GPT-3 series models show increased extractable training examples and zero-shot performance over time.
- Four methods used to measure task contamination: training data inspection, task example extraction, membership inference, and chronological analysis.
- Chronological analysis has high recall but low precision for detecting contamination.
- Training data inspection and task example extraction have low recall but high precision.
- Strong evidence of task contamination found in some model-data set combinations.
- Pre-2021 data sets show higher performance than post-2021 data sets in zero and few-shot settings.
- GPT-3 series models show dramatic performance increase on pre-2021 data sets over time.
- Instruction tuning is not the main reason for GPT-3 series performance increase.
- Open LLMs show slight performance increase over time on pre-2021 data sets.
- Training data inspection reveals task contamination in some instruction fine-tuned open LLMs.
- Task example extraction shows evidence of contamination in GPT-3 series models.
- Membership inference attack shows increasing task contamination in semantic parsing tasks.
- Closed-source models may show inflated performance due to task contamination.
- Publicly releasing training data sets can help diagnose contamination issues.
- Research community is increasingly aware of potential data contamination in LLMs.

# INSIGHTS:
- Task contamination significantly impacts few-shot learning model performance.
- Closed-source models' undisclosed pre-training data complicates contamination detection.
- Chronological analysis effectively identifies potential task contamination patterns.
- GPT-3 series models' performance increase suggests task contamination from user inputs.
- Instruction fine-tuning alone doesn't explain GPT-3 series' performance gains.
- Membership inference attacks reveal increasing task contamination over time.
- Publicly releasing training data sets aids in diagnosing contamination issues.
- Task contamination detection methods vary in precision and recall effectiveness.
- Open LLMs show less significant performance improvements compared to GPT-3 series.
- Task contamination challenges the reliability of zero-shot and few-shot evaluations.

# QUOTES:
- "Few-shot methods like In-Context Learning (ICL) show impressive results with minimal data."
- "Task contamination occurs when models have prior knowledge of unseen data or tasks."
- "Closed models don't disclose pre-training data, making contamination assessment challenging."
- "Open models' data may change, complicating contamination detection."
- "Data sets created before training data collection perform better than majority baselines."
- "Classification tasks without contamination rarely show significant improvements over baselines."
- "Membership inference attacks reveal strong correlation between extracted examples and model accuracy."
- "GPT-3 series models show increased extractable training examples and zero-shot performance over time."
- "Chronological analysis has high recall but low precision for detecting contamination."
- "Training data inspection and task example extraction have low recall but high precision."
- "Strong evidence of task contamination found in some model-data set combinations."
- "Pre-2021 data sets show higher performance than post-2021 data sets in zero and few-shot settings."
- "GPT-3 series models show dramatic performance increase on pre-2021 data sets over time."
- "Instruction tuning is not the main reason for GPT-3 series performance increase."
- "Open LLMs show slight performance increase over time on pre-2021 data sets."
- "Training data inspection reveals task contamination in some instruction fine-tuned open LLMs."
- "Task example extraction shows evidence of contamination in GPT-3 series models."
- "Membership inference attack shows increasing task contamination in semantic parsing tasks."
- "Closed-source models may show inflated performance due to task contamination."
- "Publicly releasing training data sets can help diagnose contamination issues."

# HABITS:
- Conducting membership inference attacks to detect task contamination in models.
- Using chronological analysis to identify potential task contamination patterns.
- Inspecting training data for signs of task-specific examples.
- Extracting task examples from existing models to check for contamination.
- Dividing data sets into pre and post-training collection categories for analysis.
- Comparing proprietary and open models to understand performance differences.
- Reviewing tasks to remove those known to be difficult for LLMs.
- Testing for task data contamination by generating training examples from LLMs.

# FACTS:
- Few-shot methods like ICL deliver impressive results with minimal data.
- Task contamination can occur through inclusion of test or training examples in pre-training data.
- Closed models don't disclose their pre-training data, complicating contamination assessment.
- Open models' data may change, making it hard to detect contamination reliably.
- Data sets created before training data collection perform better than majority baselines.
- Classification tasks without contamination rarely show significant improvements over baselines.
- Membership inference attacks reveal strong correlation between extracted examples and model accuracy.
- GPT-3 series models show increased extractable training examples and zero-shot performance over time.
- Chronological analysis has high recall but low precision for detecting contamination.

# REFERENCES:
None provided.

# ONE-SENTENCE TAKEAWAY
Task contamination significantly impacts few-shot learning model performance, necessitating careful evaluation and public release of training data.

# RECOMMENDATIONS:
- Use chronological analysis to identify potential task contamination patterns effectively.
- Conduct membership inference attacks to detect task contamination in models.
- Inspect training data for signs of task-specific examples to detect contamination.
- Extract task examples from existing models to check for possible contamination.
- Divide data sets into pre and post-training collection categories for analysis clarity.
- Compare proprietary and open models to understand performance differences better.
- Review tasks to remove those known to be difficult for large language models (LLMs).
