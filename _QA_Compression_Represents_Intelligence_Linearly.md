# SUMMARY
The paper presents a method to evaluate the intelligence of large language models (LLMs) by correlating compression efficiency with intelligence, addressing issues like overfitting and subjective judgment.

# IDEAS:
- The new method aims to solve evaluating LLMs' intelligence reliably by correlating compression efficiency with intelligence.
- It addresses limited empirical evidence on the relationship between compression and intelligence in LLMs.
- The method provides a stable, flexible, and unsupervised way to evaluate LLMs' performance across various tasks.
- It mitigates issues like overfitting, data contamination, and subjective judgment in evaluating LLMs' intelligence.
- The process involves evaluating pre-trained LLMs for their compression efficiency and intelligence across three key abilities.
- The three key abilities are knowledge and common sense, coding, and mathematical reasoning.
- Compression efficiency is measured using the average bits per character (BPC) metric.
- The correlation between compression efficiency and intelligence is evaluated using Pearson correlation coefficient and RMSE.
- The study focuses on well-trained base models to ensure evaluated intelligence is already manifest.
- A linear correlation between compression efficiency and intelligence is established as a universal principle.
- Superior compression indicates greater intelligence in LLMs, supported by empirical evidence.
- The method addresses potential issues like overfitting benchmarks and selecting appropriate compression corpora.
- The study explores the impact of the size of the compression corpus on the reliability of the BPC metric.
- The analysis extends to cross-ability tasks, demonstrating the effectiveness of using compression efficiency as a reliable evaluation metric.
- The theoretical benefit is establishing a strong empirical correlation between compression efficiency and intelligence in LLMs.
- Superior compression as measured by BPC indicates greater intelligence across various domains.
- The practical benefit is offering a reliable and unsupervised metric for evaluating LLMs' abilities.
- Researchers can update and customize compression corpora to avoid overfitting or test contamination issues.
- The method allows for flexible and stable evaluation of LLMs, demonstrated by linear correlation between compression efficiency and task performance.
- It can be extended to assess LLMs across different model sizes, tokenizers, context window lengths, and pre-training data distributions.
- The method was validated through empirical study by examining the relationship between compression and intelligence in LLMs.
- Experiments were conducted across 30 public LLMs and 12 diverse benchmarks.
- A Pearson correlation coefficient of around -0.95 was found for each evaluated domain of intelligence.
- The linear relationship was observed across different model sizes, tokenizers, and pre-training data distributions.
- The study compared compression efficiency on different corpora to study effects on results.
- The size of the compression corpus was varied to analyze its impact on correlation strength.
- Results showed that compression efficiency serves as a stable, flexible, and reliable metric to evaluate LLMs.
- Limitations include focusing solely on base models, excluding fine-tuned models not considered general-purpose compressors.
- The study concentrates on short to medium context regimes, deferring long context scenarios investigation.

# INSIGHTS:
- Correlating compression efficiency with intelligence offers a reliable metric for evaluating LLMs' abilities.
- Superior compression indicates greater intelligence in LLMs across various domains like knowledge and coding.
- Empirical evidence supports the belief that compression is closely connected to intelligence in AI contexts.
- Using average bits per character (BPC) as a metric provides a stable evaluation method for LLMs.
- Linear correlation between compression efficiency and intelligence is a universal principle for LLM evaluation.
- Customizing compression corpora helps avoid overfitting or test contamination in benchmark evaluations.
- Evaluating well-trained base models ensures that the assessed intelligence is already manifest.
- Compression efficiency can be used to assess LLMs across different model sizes and pre-training data distributions.
- The method's flexibility allows for stable evaluation across various downstream tasks and domains.
- Empirical validation through diverse benchmarks strengthens the method's reliability.

# QUOTES:
- "The new method aims to solve the problem of evaluating the intelligence of large language models."
- "This method addresses the challenge of limited empirical evidence on the relationship between compression and intelligence."
- "Compression efficiency is measured using the average bits per character (BPC) metric."
- "The correlation between compression efficiency and intelligence is evaluated using Pearson correlation coefficient."
- "Superior compression indicates greater intelligence in LLMs."
- "The method provides a stable, flexible, and unsupervised way to evaluate the model's performance."
- "It mitigates issues such as overfitting, data contamination, and subjective judgment."
- "The study focuses on well-trained base models to ensure that the evaluated intelligence is already manifest."
- "A linear correlation between compression efficiency and intelligence is established as a universal principle."
- "The theoretical benefit is establishing a strong empirical correlation between compression efficiency and intelligence."
- "Superior compression as measured by BPC indicates greater intelligence across various domains."
- "The practical benefit is offering a reliable and unsupervised metric for evaluating LLMs' abilities."
- "Researchers can update and customize the compression corpora to avoid overfitting or test contamination issues."
- "The method allows for flexible and stable evaluation of LLMs."
- "It can be extended to assess LLMs across different model sizes, tokenizers, context window lengths, and pre-training data distributions."
- "The method was validated through empirical study by examining the relationship between compression and intelligence in LLMs."
- "Experiments were conducted across 30 public LLMs and 12 diverse benchmarks."
- "A Pearson correlation coefficient of around -0.95 was found for each evaluated domain of intelligence."
- "The linear relationship was observed across different model sizes, tokenizers, and pre-training data distributions."
- "Results showed that compression efficiency serves as a stable, flexible, and reliable metric to evaluate LLMs."

# HABITS:
- Evaluating pre-trained LLMs for their compression efficiency across key abilities like knowledge and coding.
- Using average bits per character (BPC) as a metric to measure compression efficiency.
- Focusing on well-trained base models to ensure evaluated intelligence is already manifest.
- Customizing compression corpora to avoid overfitting or test contamination in benchmark evaluations.
- Conducting experiments across diverse benchmarks to validate methods empirically.

# FACTS:
- The new method correlates compression efficiency with intelligence in large language models (LLMs).
- Compression efficiency is measured using the average bits per character (BPC) metric.
- A Pearson correlation coefficient of around -0.95 was found for each evaluated domain of intelligence.
- Superior compression indicates greater intelligence in LLMs across various domains like knowledge and coding.
- The method provides a stable, flexible, and unsupervised way to evaluate LLMs' performance.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
Correlating compression efficiency with intelligence offers a reliable, flexible metric for evaluating large language models' abilities.

# RECOMMENDATIONS:
- Use average bits per character (BPC) as a metric to measure compression efficiency in LLMs.
- Focus on well-trained base models to ensure evaluated intelligence is already manifest in assessments.
- Customize compression corpora to avoid overfitting or test contamination in benchmark evaluations.
- Conduct experiments across diverse benchmarks to validate methods empirically for robust results.
- Extend evaluations to assess LLMs across different model sizes, tokenizers, context window lengths.