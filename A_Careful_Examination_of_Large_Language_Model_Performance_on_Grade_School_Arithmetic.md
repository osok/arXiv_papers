# SUMMARY
Researchers introduce GSM 1K, a new benchmark of 1250 grade school math problems, to assess overfitting in large language models (LLMs) and ensure accurate evaluation.

# IDEAS:
- GSM 1K was created to address concerns of data contamination in existing benchmarks.
- GSM 1K contains 1250 grade school math problems similar to GSM 8K.
- Human annotators solely created GSM 1K without LLM or synthetic data input.
- GSM 1K ensures a fair comparison by matching the difficulty range of GSM 8K.
- Some models showed a 133% performance drop on GSM 1K compared to GSM 8K.
- Overfitting was observed in certain model families like Mistol and Fi.
- Spearman's correlation (r = 0.32) suggests models may memorize GSM 8K examples.
- Cutting-edge models and Llama 2 family showed minimal overfitting signs.
- All models demonstrated the ability to generalize to new math problems.
- GSM 1K will not be released publicly to prevent future data contamination.
- Evaluation code will be open-sourced for reproducibility.
- GSM 1K will be released when top open-source models achieve over 95% accuracy or by end of 2025.
- GSM 1K problems were created using basic arithmetic operations.
- Quality checks included multiple review layers and human differentiation tests.
- Human crowd workers struggled to differentiate between GSM 8K and GSM 1K problems.
- Pre-existing models like GPT Neo 20b and GPT-2 showed minimal performance differences between datasets.
- Overfit models can still reason effectively despite memorizing training data answers.
- Data contamination alone may not fully explain overfitting.
- Advanced models show minimal overfitting despite known training data containing test instances.
- Overfitting may involve factors beyond data leakage, such as training data collection methods.

# INSIGHTS:
- Overfitting does not necessarily hinder reasoning abilities in LLMs.
- Data contamination alone may not fully explain overfitting in LLMs.
- Advanced models show minimal overfitting despite known training data containing test instances.
- Overfit models can still solve novel problems effectively, indicating reasoning capabilities.
- GSM 1K ensures a fair comparison by matching the difficulty range of GSM 8K.

# QUOTES:
- "GSM 1K was created solely by human annotators without any input from LLMs or synthetic data sources."
- "Our analysis revealed that many models show signs of being influenced by Benchmark data."
- "The worst performing model scored 133% lower on GSM 1K compared to GSM 8K."
- "Cutting Edge models and all sizes of the Llama 2 family showed minimal signs of overfitting."
- "We have decided not to release GSM 1K publicly at this time to prevent future data contamination issues."
- "We will make our evaluation code open source for reproducibility."
- "Overfit models can still reason effectively contrary to the concern that they only memorize training data answers."
- "Data contamination alone may not fully explain overfitting."
- "Advanced models show minimal overfitting despite known training data containing some test instances."
- "Overfitting isn't solely caused by data contamination but may involve other factors."

# HABITS:
- Regularly evaluate major open-source and closed-source releases to update results continuously.
- Conduct rigorous quality checks, including multiple review layers and human differentiation tests.
- Use human annotators to create benchmark problems without LLM or synthetic data input.

# FACTS:
- GSM 1K contains 1250 grade school math problems similar to GSM 8K.
- Some models showed a 133% performance drop on GSM 1K compared to GSM 8K.
- Spearman's correlation (r = 0.32) suggests models may memorize GSM 8K examples.
- Cutting-edge models and Llama 2 family showed minimal overfitting signs.
- All models demonstrated the ability to generalize to new math problems.

# REFERENCES:
- GSM 8K
- GPT Neo 20b
- GPT-2
- Llama 2
- Mistol
- Fi

# ONE-SENTENCE TAKEAWAY
Overfitting in LLMs does not necessarily hinder reasoning abilities, highlighting the need for continuous evaluation and proper benchmarking.

# RECOMMENDATIONS:
- Regularly evaluate major open-source and closed-source releases to update results continuously.
- Conduct rigorous quality checks, including multiple review layers and human differentiation tests.
- Use human annotators to create benchmark problems without LLM or synthetic data input.