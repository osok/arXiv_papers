# SUMMARY
The text discusses enhancing large language models' (LLMs) mathematical skills using a self-critique pipeline, focusing on rejective fine-tuning (RFT) and direct preference optimization (DPO).

# IDEAS:
- Enhancing LLMs' mathematical skills during feedback learning phase improves practical deployment.
- Math critique model derived from LLM provides feedback on generated solutions.
- Rejective fine-tuning (RFT) involves multiple sampling iterations, rejecting certain responses.
- Direct preference optimization (DPO) updates the model by learning from pairs of correct and incorrect answers.
- MAURV Benchmark evaluates LLMs on complex real-world mathematical problems.
- Self-critique pipeline enhances both mathematical and linguistic abilities simultaneously.
- Math critique model scores responses based on questions, reference answers, and explanatory analysis.
- Math critique categorizes responses into four groups: entirely incorrect, partially correct, mostly correct, and completely correct.
- Average score evaluation calculates mean critique scores for a set of questions.
- Hard split evaluation categorizes answers as passing or failing based on correctness threshold.
- Self-critique pipeline reduces manual annotation efforts and enhances model efficiency.
- DPO method improves model performance by comparing correct and incorrect answers.
- DPO data filtering selects pairs based on significant differences in math critique scoring results.
- Critique RFT data set includes sampled questions and responses meeting a minimum correct score threshold.
- Data collection includes public datasets, middle school, and university exam questions.
- Model outperforms others in various tasks, achieving high scores on different datasets.
- Ablation studies analyze the impact of data composition on model performance.
- Incorporating math-specific data enhances model's mathematical capabilities significantly.
- Model demonstrates competitive or superior performance in mathematical reasoning and cross-linguistic generalization.
- Limitations include difficulty with questions involving drawings and precision calculations.
- Future work includes integrating multimodal input and output components.

# INSIGHTS:
- Self-critique pipeline enhances both mathematical and linguistic abilities simultaneously.
- Math critique model uses language models' contextual abilities for precise judgments.
- Rejective fine-tuning (RFT) refines data set by rejecting certain responses based on criteria.
- Direct preference optimization (DPO) learns from pairs of correct and incorrect answers.
- MAURV Benchmark evaluates LLMs on complex real-world mathematical problems.
- Self-critique pipeline reduces manual annotation efforts and enhances model efficiency.
- DPO method improves model performance by comparing correct and incorrect answers.
- Data collection includes public datasets, middle school, and university exam questions.
- Model outperforms others in various tasks, achieving high scores on different datasets.
- Incorporating math-specific data enhances model's mathematical capabilities significantly.

# QUOTES:
- "We introduce a math critique model derived from the LLM itself to provide feedback on its generated solutions."
- "Our approach consists of two stages: rejective fine-tuning (RFT) and direct preference optimization (DPO)."
- "We use math critique evaluations to refine the data set, focusing on improving the LLM's ability to generate mathematically accurate and logically consistent responses."
- "Math critique classifies responses into four categories: entirely incorrect, partially correct but with errors in the process, mostly correct but with some flaws in the process, and completely correct."
- "The self-critique pipeline involves training a math critique model, a chat model, and iteratively fine-tuning them using rejection sampling."
- "The DPO method is advantageous due to its simplicity in handling data flows, stability, and speed during training."
- "We observed significant improvements in mathematical capabilities across different data sets in comparison to proprietary models like the GPT series by OpenAI."
- "Our results indicated promising performance, especially in Chinese language capabilities."
- "One issue is our model's difficulty with questions involving drawings as it is purely linguistic."
- "We plan to explore integrating multimodal input and output components."

# HABITS:
- Utilizing rejective fine-tuning (RFT) to refine data sets for better accuracy.
- Implementing direct preference optimization (DPO) for learning from answer pairs.
- Regularly evaluating models using benchmarks like MAURV for real-world problems.
- Iteratively fine-tuning models using rejection sampling to enhance efficiency.
- Collecting diverse data sets from public sources and academic exams for training.

# FACTS:
- MAURV Benchmark evaluates LLMs on complex real-world mathematical problems.
- Math critique model scores responses based on questions, reference answers, and explanatory analysis.
- Rejective fine-tuning (RFT) involves multiple sampling iterations, rejecting certain responses.
- Direct preference optimization (DPO) updates the model by learning from pairs of correct and incorrect answers.
- Data collection includes public datasets, middle school, and university exam questions.

# REFERENCES:
- MAURV Benchmark
- GSM 8K
- Math training sets
- APE2 110K
- C-Math
- Hungarian National Exam

# ONE-SENTENCE TAKEAWAY
Enhancing LLMs' mathematical skills through self-critique pipelines significantly improves their practical deployment in real-world scenarios.

# RECOMMENDATIONS:
- Use self-critique pipelines to enhance both mathematical and linguistic abilities simultaneously.
- Implement rejective fine-tuning (RFT) to refine data sets for better accuracy.
- Apply direct preference optimization (DPO) for learning from pairs of correct and incorrect answers.
- Regularly evaluate models using benchmarks like MAURV for real-world problems.
- Collect diverse data sets from public sources and academic exams for training.