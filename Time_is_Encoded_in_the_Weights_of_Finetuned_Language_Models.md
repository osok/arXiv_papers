# SUMMARY
The authors discuss temporal misalignment in language models and propose using time vectors to adapt models to specific time periods, improving performance.

# IDEAS:
- Temporal misalignment occurs when training and testing data are from different time periods.
- Performance of language models can degrade significantly due to temporal misalignment.
- Adapting models to specific time periods is challenging due to varying time scales.
- Interpolating between parameters of fine-tuned models can modify neural network behavior.
- Time vectors represent directions in weight space that improve performance on specific time periods.
- Time vectors are organized on a manifold, with close time periods yielding close time vectors.
- Temporal degradation correlates with angles between time vectors.
- Interpolating between time vectors can improve performance on intervening months or years.
- Time vectors can generalize task-specific models across similar time periods.
- Temporal variation is encoded in the weight space of fine-tuned models.
- Weight interpolation customizes language models to new time periods.
- The authors provide code, data, and over 500 fine-tuned models publicly.
- Yearly degradation shows a linear pattern in model performance decline.
- Monthly degradation exhibits seasonal trends in temporal misalignment.
- Models trained on a particular month perform better on the same month in other years.
- Time vectors' similarity correlates with performance decay over time.
- Interpolating between time vectors improves performance on unseen times.
- Task vectors are differences between pre-trained and fine-tuned model weights.
- Time vectors extend task vectors to the time domain.
- Interpolating between oldest and newest time vectors improves performance on intervening years.
- Larger models show greater improvements with interpolation methods.
- Model soup technique combines time-specific models for multiple time periods.
- Uniform soup applies equal weight among all models; greedy soup includes only performance-improving models.
- Time soups generally perform worse than models fine-tuned on all available data.
- Future research could explore sophisticated ways of combining data from different years.

# INSIGHTS:
- Temporal misalignment causes significant performance drops in language models over time.
- Time vectors represent weight space directions that enhance model performance for specific periods.
- Interpolating between time vectors can adapt models to new, unseen time periods effectively.
- Yearly degradation in model performance follows a linear pattern, while monthly shows seasonal trends.
- Time vectors' organization on a manifold allows for intuitive interpolation and adaptation.
- Larger language models benefit more from interpolation techniques for temporal adaptation.
- Combining time-specific models (model soup) does not outperform fine-tuning on all available data.
- Temporal variation is inherently encoded in the weight space of fine-tuned language models.

# QUOTES:
- "Temporal misalignment occurs when the training and testing data don't match up in terms of time periods."
- "We need to adapt our models to work well with data from specific time periods."
- "Time vectors represent a direction in weight space that improves performance on text from the target time period."
- "Temporal degradation in yearly and monthly settings is strongly correlated with the angles between time vectors."
- "Interpolating between two time vectors can find vectors that improve performance on intervening months or years."
- "Time vectors are intuitively organized on a manifold."
- "Performance decays linearly on a yearly scale, but there are seasonal trends in month-to-month misalignment."
- "Time vectors closer together in weight space are also closer together in time."
- "The similarity of time vectors correlates with temporal degradation."
- "Interpolating between models fine-tuned on the oldest and newest times improves performance on intervening years."
- "Creating labeled data sets can be time-consuming and expensive."
- "Larger models show greater improvements with interpolation methods."
- "Model soup technique allows us to train time-specific models independently and combine them at any time."
- "Time soups generally perform worse than models fine-tuned using all available data."
- "Future research could explore more sophisticated ways of combining data from different years."

# HABITS:
- Fine-tuning language models on multiple time-stratified data sets for analysis.
- Using heat maps to visualize yearly temporal misalignment in model performance.
- Calculating percent change in perplexity to account for yearly performance differences.
- Training models on monthly splits to explore unexplored areas of temporal misalignment.
- Measuring cosine similarity between model weights from different time periods.
- Performing arithmetic on task-specific model weights for updating to future times.

# FACTS:
- Temporal misalignment can cause significant drops in language model performance over different periods.
- Yearly degradation in model performance follows a linear pattern across tasks and model sizes.
- Monthly degradation exhibits seasonal trends, with better performance on the same month across years.
- Time vectors' similarity correlates with temporal degradation, indicating their organization on a manifold.
- Interpolating between oldest and newest time vectors improves performance on intervening years and months.

# REFERENCES:
- T5 small, T5 large, and T5 3B pre-trained language models
- WMT language modeling data set
- NewSum and PoAF tasks
- Bloom filter for measuring overlap between yearly train and test splits
- Titan A40 and A100 GPUs for running evaluations

# ONE-SENTENCE TAKEAWAY
Interpolating between time vectors effectively adapts language models to new, unseen time periods, improving their performance.

# RECOMMENDATIONS:
- Adapt language models to specific periods by interpolating between fine-tuned model parameters.
- Use heat maps to visualize temporal misalignment and calculate percent change in perplexity.
- Train models on monthly splits to explore seasonal trends in temporal misalignment.
- Measure cosine similarity between model weights from different periods for better adaptation.
- Perform arithmetic on task-specific model weights for updating to future times.