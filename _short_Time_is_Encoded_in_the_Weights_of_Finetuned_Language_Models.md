# SUMMARY
Researchers create time-specific language modeling datasets from news and Twitter, fine-tune T5 models, and analyze temporal misalignment and interpolation.

# IDEAS:
- Create two new time-specific language modeling datasets from news and Twitter domains.
- Randomly sample articles and tweets from specific time periods for dataset creation.
- Provide a comprehensive overview of language use in news and Twitter over the past decade.
- Fine-tune T5 small, T5 large, and T5 3B models on time-stratified datasets.
- Use the LM adaptation objective to reduce computational burden during fine-tuning.
- Employ low-rank adaptation (LoRA) and merge LoRA weights back into the base model.
- Explore different ways of interpolating between time vectors to generalize to new times.
- Compute interpolation between two time vectors through a weighted sum of the vectors.
- Evaluate performance of interpolated models on intervening times by sweeping over interpolation weights.
- Measure temporal misalignment across various domains, tasks, and time scales.
- Reveal linear patterns of degradation in each task for all model sizes on a yearly scale.
- Find nonlinear patterns corresponding to the cycle of months in each year on a monthly scale.
- Analyze weights of time-specific models and use time vectors to update models to unseen times.
- Weights of time vectors become less similar as the times they were fine-tuned on become more misaligned.
- Use time vector analogies to update models to intervening future and multiple time periods.
- Interpolating between time vectors improves performance on unseen intervening times and future times.
- Building a multi-year model using a soup of time vectors does not perform as well as fine-tuning on all times at once.

# INSIGHTS:
- Time-specific datasets provide a comprehensive overview of language use over the past decade.
- Fine-tuning models on time-stratified datasets reveals temporal misalignment patterns.
- Interpolating between time vectors helps generalize models to unseen times.
- Temporal misalignment shows linear degradation yearly but nonlinear monthly patterns.
- Weights of time vectors diverge as fine-tuning times become more misaligned.

# QUOTES:
- "Create two new time-specific language modeling datasets from news and Twitter domains."
- "Randomly sample articles and tweets from specific time periods for dataset creation."
- "Provide a comprehensive overview of language use in news and Twitter over the past decade."
- "Fine-tune T5 small, T5 large, and T5 3B models on time-stratified datasets."
- "Use the LM adaptation objective to reduce computational burden during fine-tuning."
- "Employ low-rank adaptation (LoRA) and merge LoRA weights back into the base model."
- "Explore different ways of interpolating between time vectors to generalize to new times."
- "Compute interpolation between two time vectors through a weighted sum of the vectors."
- "Evaluate performance of interpolated models on intervening times by sweeping over interpolation weights."
- "Measure temporal misalignment across various domains, tasks, and time scales."
- "Reveal linear patterns of degradation in each task for all model sizes on a yearly scale."
- "Find nonlinear patterns corresponding to the cycle of months in each year on a monthly scale."
- "Analyze weights of time-specific models and use time vectors to update models to unseen times."
- "Weights of time vectors become less similar as the times they were fine-tuned on become more misaligned."
- "Use time vector analogies to update models to intervening future and multiple time periods."
- "Interpolating between time vectors improves performance on unseen intervening times and future times."
- "Building a multi-year model using a soup of time vectors does not perform as well as fine-tuning on all times at once."

# HABITS:
- Regularly sample articles and tweets from specific periods for dataset creation.
- Fine-tune language models on stratified datasets to understand temporal changes.
- Use low-rank adaptation techniques to reduce computational burden during model training.
- Continuously explore new methods for interpolating between data points for better generalization.

# FACTS:
- Time-specific datasets offer insights into language use over the past decade.
- Temporal misalignment can be analyzed across various domains, tasks, and scales.
- Linear degradation patterns are observed yearly, while nonlinear patterns appear monthly.

# REFERENCES:
None mentioned explicitly.

# ONE-SENTENCE TAKEAWAY
Interpolating between time vectors enhances model performance on unseen times, revealing temporal misalignment patterns.