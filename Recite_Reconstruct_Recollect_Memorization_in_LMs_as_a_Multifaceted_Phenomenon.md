# SUMMARY
The text introduces a taxonomy to categorize language model (LM) memorization behaviors into recitation, reconstruction, and recollection, inspired by human memorization. Experiments show factors like low perplexity and model size influence memorization, with larger models memorizing more data. The taxonomy-based predictive model outperforms generic approaches.

# IDEAS:
- Taxonomy categorizes LM memorization into recitation, reconstruction, and recollection based on human memorization behaviors.
- Recitation involves duplicating sequences from training data verbatim.
- Reconstruction reconstructs passages based on learned patterns or templates.
- Recollection sporadically remembers fragments that do not fit other categories.
- Low perplexity is strongly linked to memorization but varies for different examples.
- Number of memorized sequences increases with training time and model size.
- Recollection experiences the fastest growth among memorization types.
- Logistic regression models predict memorization for each category, outperforming baseline models.
- Low perplexity prompts facilitate recitation, while rare tokens constrain recollection.
- Memorization defined as generating next tokens verbatim when given the first K tokens.
- Analysis based on Pythia models trained on the Pile dataset.
- Key factors influencing memorization: duplicates in training corpus, semantic similarity, textual variations, token frequency.
- Larger models tend to memorize more data due to more parameters capturing sequences accurately.
- Smaller models excel at extrapolating repeating patterns.
- Memorization does not increase uniformly throughout training.
- Repeated exposure to duplicated data is not the sole reason for increased memorization.
- Notable increase in recollection category suggests focus on rarer sequences towards end of training.
- Sudden increase in reconstruction indicates breakthrough in generalizing complex patterns.
- Taxonomy captures meaningful distinctions in dependencies, supporting its role in predicting memorization outcomes.
- Predictive model based on taxonomy outperforms generic baseline models.
- Optimal partition model categorized samples based on Huffman coding length and sequence duplicate count.
- Intuitive taxonomy outperforms optimal partition in categorizing samples based on specific features.
- Rare sequences in recollection category more likely memorized if they do not contain rare tokens.
- Number of duplicates in recollection candidate influences its memorization.
- Beyond a certain threshold of duplicates, increased exposure does not lead to better memorization.
- Predictable continuations strongly associated with memorization across all categories except reconstruction.
- Future work could enhance understanding of memorization by considering more general dependencies.

# INSIGHTS:
- Taxonomy differentiates LM memorization into recitation, reconstruction, and recollection based on human behaviors.
- Low perplexity and model size significantly influence the likelihood of sequence memorization.
- Larger models memorize more data due to their capacity to capture sequences accurately.
- Recollection grows fastest among memorization types, indicating factors beyond repeated exposure.
- Predictive models based on taxonomy outperform generic approaches in predicting memorization outcomes.
- Rare tokens constrain recollection, while low perplexity prompts facilitate recitation.
- Memorization does not increase uniformly; repeated exposure to duplicates is not the sole driver.
- Intuitive taxonomy outperforms optimal partition models in categorizing samples effectively.
- Rare sequences are more likely to be memorized if they lack rare tokens.

# QUOTES:
- "We identify three types of LM memorization: recitation, reconstruction, and recollection."
- "Low perplexity is strongly linked to memorization but this association varies for different examples."
- "The number of memorized sequences increases with training time and model size across all categories."
- "Recollection experiences the fastest growth indicating factors beyond repeated exposure or random memorization."
- "Our taxonomy helps differentiate between recitation and recollection by examining statistical dependencies."
- "Low perplexity prompts facilitate recitation while rare tokens constrain recollection."
- "Larger models tend to memorize more data likely because they have more parameters to capture sequences accurately."
- "Memorization does not increase uniformly throughout training."
- "Repeated exposure to heavily duplicated data is not the sole reason for increased memorization."
- "There is a notable increase in the recollection category suggesting a focus on memorizing rarer sequences."
- "Our predictive model based on this taxonomy outperforms generic baseline models."
- "Rare sequences in the recollection category were more likely to be memorized if they did not contain rare tokens."
- "Beyond a certain threshold of duplicates, increased exposure did not lead to better memorization."
- "Predictable continuations being strongly associated with memorization across all categories except for cases of reconstruction."
- "Our intuitive taxonomy might perform better than the optimal partition because the search for thresholds was limited."

# HABITS:
- Conduct experiments comparing memorized and unmoral factors influencing memorization likelihood.
- Analyze memorization across different model scales and training timings using public datasets.
- Develop logistic regression models to predict memorization for each category.
- Examine statistical dependencies to differentiate between recitation and recollection.
- Use Huffman coding length and sequence duplicate count for optimal partitioning strategies.

# FACTS:
- Low perplexity is strongly linked to language model (LM) memorization likelihood.
- Number of memorized sequences increases with training time and model size across all categories.
- Recollection experiences the fastest growth among LM memorization types.
- Larger models tend to memorize more data due to more parameters capturing sequences accurately.
- Smaller models excel at extrapolating repeating patterns compared to larger models.
- Memorization does not increase uniformly throughout training time.
- Repeated exposure to heavily duplicated data is not the sole reason for increased LM memorization.
- Notable increase in recollection category suggests focus on rarer sequences towards end of training.
- Sudden increase in reconstruction indicates breakthrough in generalizing complex patterns late in training.

# REFERENCES:
- Pythia models trained on the Pile dataset
- Huffman coding length
- Logistic regression models

# ONE-SENTENCE TAKEAWAY
Understanding dependencies between features enhances predictive accuracy of language model (LM) memorization behaviors.

# RECOMMENDATIONS:
- Categorize LM memorization into recitation, reconstruction, and recollection based on human behaviors.
- Use low perplexity prompts to facilitate recitation in language models (LMs).
- Consider rare tokens as constraints for recollection in LMs.
- Develop logistic regression models to predict LM memorization for each category effectively.
- Analyze sequence properties like templating, compressibility, and perplexity for better understanding.