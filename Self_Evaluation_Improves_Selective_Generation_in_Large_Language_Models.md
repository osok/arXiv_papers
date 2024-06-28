# SUMMARY
The text discusses improving the trustworthiness of large language models (LLMs) by using token-level scoring and self-evaluation tasks to enhance quality calibration.

# IDEAS:
- Large language models (LLMs) are trained on vast text corpora and fine-tuned for specific instructions.
- Trustworthiness of LLM outputs is crucial for safe deployment in real-world applications.
- Distance to training distribution in embedding space can predict output quality for generative models.
- Extracting embeddings from well-integrated LLM systems requires significant engineering effort.
- Sequence probability or length-normalized sequence probabilities don't reliably rank outputs by quality.
- Human feedback can fine-tune LLMs to better align with human-judged quality, improving calibration.
- Self-evaluation ability of LLMs can be leveraged to improve quality calibration without expensive human feedback.
- Token-level probability is well-calibrated for multiple-choice and true/false questions.
- Evaluating generation with token-level probabilities might be better than sequence-level likelihood.
- Reducing sequence-level scoring to token-level scoring improves quality calibration for free-form tasks.
- Sample and select method chooses the best answer based on softmax probability score.
- Adding "none of the above" as an option helps mitigate overconfident predictions.
- Calibration AU and selective AU are metrics for evaluating confidence scores in selective generation.
- Sequence-level likelihood is biased towards sequence length, underestimating longer sentences.
- Length normalization improves performance but still has limitations.
- Hybrid strategy combining sample and select with sample and avow performs best overall.
- Self-evaluation complements self-critique and revise techniques to improve answer quality.
- Position bias in answer ordering has minimal impact on performance.
- Previous work focused more on accuracy rather than confidence estimation or calibration.
- Self-evaluation increases inference time but enhances quality calibration.
- Future work aims to improve sequence-level score calibration during training and fine-tuning stages.

# INSIGHTS:
- Trustworthiness of LLM outputs is essential for real-world applications.
- Token-level probabilities are better calibrated than sequence-level likelihoods.
- Human feedback fine-tunes LLMs to align with human judgment, improving calibration.
- Self-evaluation leverages LLMs' abilities to improve quality without costly human feedback.
- Hybrid strategies combining different methods yield better overall performance.

# QUOTES:
- "Trustworthiness of LLM outputs is crucial for safe deployment in real-world applications."
- "Sequence probability or length-normalized sequence probabilities don't reliably rank outputs by quality."
- "Human feedback can fine-tune LLMs to better align with human-judged quality, improving calibration."
- "Token-level probability is well-calibrated for multiple-choice and true/false questions."
- "Evaluating generation with token-level probabilities might be better than sequence-level likelihood."
- "Reducing sequence-level scoring to token-level scoring improves quality calibration for free-form tasks."
- "Sample and select method chooses the best answer based on softmax probability score."
- "Adding 'none of the above' as an option helps mitigate overconfident predictions."
- "Calibration AU and selective AU are metrics for evaluating confidence scores in selective generation."
- "Sequence-level likelihood is biased towards sequence length, underestimating longer sentences."
- "Length normalization improves performance but still has limitations."
- "Hybrid strategy combining sample and select with sample and avow performs best overall."
- "Self-evaluation complements self-critique and revise techniques to improve answer quality."
- "Position bias in answer ordering has minimal impact on performance."
- "Previous work focused more on accuracy rather than confidence estimation or calibration."
- "Self-evaluation increases inference time but enhances quality calibration."
- "Future work aims to improve sequence-level score calibration during training and fine-tuning stages."

# HABITS:
- Using token-level probabilities for better-calibrated evaluations.
- Leveraging self-evaluation to improve model output quality.
- Combining multiple methods for optimal performance in selective generation tasks.
- Adding "none of the above" options to mitigate overconfidence in predictions.
- Focusing on both accuracy and confidence estimation in model evaluations.

# FACTS:
- LLMs are trained on vast text corpora and fine-tuned for specific instructions.
- Distance to training distribution can predict output quality for generative models.
- Sequence probability or length-normalized probabilities don't reliably rank outputs by quality.
- Human feedback fine-tunes LLMs to align with human judgment, improving calibration.
- Token-level probability is well-calibrated for multiple-choice and true/false questions.

# REFERENCES:
None mentioned explicitly.

# ONE-SENTENCE TAKEAWAY
Leveraging token-level scoring and self-evaluation significantly improves the quality calibration of large language models.

# RECOMMENDATIONS:
- Use token-level probabilities for better-calibrated evaluations in LLMs.
- Leverage self-evaluation to improve model output quality without costly human feedback.
- Combine multiple methods for optimal performance in selective generation tasks.
- Add "none of the above" options to mitigate overconfidence in predictions.
- Focus on both accuracy and confidence estimation in model evaluations.