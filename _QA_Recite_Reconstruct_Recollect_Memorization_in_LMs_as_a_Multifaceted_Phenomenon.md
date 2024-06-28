# SUMMARY
The paper discusses a taxonomy for language model (LM) memorization, categorizing it into recitation, reconstruction, and recollection, and explores factors influencing memorization.

# IDEAS:
- Recitation involves generating verbatim copies of common texts like webpage boilerplate or software licenses.
- Reconstruction occurs when the model learns templates and reconstructs samples based on broadly applicable patterns.
- Recollection refers to memorizing rare sequences not highly duplicated or easily reconstructed.
- The taxonomy allows for a nuanced understanding of how LM memorization occurs.
- Factors determining memorization include duplicates, semantic matches, textual matches, token frequency, templating, compressibility, and perplexity.
- Duplicates refer to the number of duplicates in the training data for a given sequence.
- Semantic matches assess the similarity of samples in training using document embeddings.
- Textual matches identify sequences with low Levenshtein edit distance in their prompts.
- Token frequency statistics are computed for individual tokens in the sequence.
- Templating involves identifying predictable patterns like repeating or incrementing sequences.
- Compressibility measures how easily a sequence can be compressed.
- Perplexity is the average perplexity across tokens, with low perplexity sequences being more likely memorized.
- Logistic regressions predict memorization by training separate models for each taxonomic category.
- Larger models tend to memorize more data, with recollection growing the most as model size increases.
- Reconstruction barely increases with model size, indicating smaller models are effective at extrapolating templates.
- The proportion of recitation decreases relative to overall memorization as model size increases.
- The intuitive taxonomic model outperforms both the generic Baseline and optimally partitioned models in predicting memorization.
- The intuitive taxonomic model is better calibrated and more accurate overall except for the recollection set.
- Statistical tests confirm significant differences in dependencies across taxonomic categories.
- The intuitive taxonomy helps predict memorization from dependent factors and expresses some natural kinds.

# INSIGHTS:
- Recitation involves generating verbatim copies of common texts like webpage boilerplate or software licenses.
- Reconstruction occurs when the model learns templates and reconstructs samples based on broadly applicable patterns.
- Recollection refers to memorizing rare sequences not highly duplicated or easily reconstructed.
- Factors determining memorization include duplicates, semantic matches, textual matches, token frequency, templating, compressibility, and perplexity.
- Larger models tend to memorize more data, with recollection growing the most as model size increases.
- Reconstruction barely increases with model size, indicating smaller models are effective at extrapolating templates.
- The proportion of recitation decreases relative to overall memorization as model size increases.
- The intuitive taxonomic model outperforms both the generic Baseline and optimally partitioned models in predicting memorization.
- The intuitive taxonomic model is better calibrated and more accurate overall except for the recollection set.
- Statistical tests confirm significant differences in dependencies across taxonomic categories.

# QUOTES:
- "Recitation involves highly duplicated sequences in the training corpus where the model generates verbatim copies."
- "Reconstruction occurs when the model learns templates and reconstructs samples based on broadly applicable patterns."
- "Recollection refers to cases where the model memorizes rare sequences that are not highly duplicated."
- "The taxonomy allows for a nuanced understanding of how LM memorization occurs."
- "Factors determining memorization include duplicates, semantic matches, textual matches, token frequency, templating, compressibility, and perplexity."
- "Larger models tend to memorize more data, with recollection growing the most as model size increases."
- "Reconstruction barely increases with model size, indicating smaller models are effective at extrapolating templates."
- "The proportion of recitation decreases relative to overall memorization as model size increases."
- "The intuitive taxonomic model outperforms both the generic Baseline and optimally partitioned models in predicting memorization."
- "The intuitive taxonomic model is better calibrated and more accurate overall except for the recollection set."
- "Statistical tests confirm significant differences in dependencies across taxonomic categories."

# HABITS:
N/A

# FACTS:
N/A

# REFERENCES:
N/A

# ONE-SENTENCE TAKEAWAY
The taxonomy categorizes LM memorization into recitation, reconstruction, and recollection, enhancing understanding and prediction accuracy.

# RECOMMENDATIONS:
N/A