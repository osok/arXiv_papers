# SUMMARY
The new method, Joint Example Selection (JEST), aims to solve inefficient and costly manual curation of large-scale datasets for pre-training models by introducing a model-based data curation approach.

# IDEAS:
- JEST accelerates learning in multimodal tasks by selecting highly learnable batches from larger super batches.
- The method addresses slow and power law scaling of large-scale pre-training.
- JEST prioritizes examples that are both unlearned and learnable, improving training efficiency.
- It enables the use of small curated datasets to guide the curation of larger datasets.
- JEST uses model-based scoring functions to score subbatches based on losses from learner models.
- Three scoring heuristics are used: hard learner, easy reference, and learnability.
- Hard learner prioritizes batches with high loss under the learner model.
- Easy reference prioritizes data that is easy for a pre-trained reference model.
- Learnability combines scores to upsample data that is unlearned and learnable.
- JEST samples batches in proportion to their joint learnability.
- Efficient scoring and multi-resolution training are leveraged for gains in efficiency.
- Data quality bootstrapping uses a pre-trained reference model to guide larger dataset curation.
- JEST surpasses the quality of the reference model on downstream tasks.
- The method simplifies data curation by eliminating the need for foundation datasets.
- JEST offers a more effective replacement for generic foundation datasets.
- The method is validated through experiments comparing it to state-of-the-art models.
- Visualizing the learnability matrix helps evaluate the efficacy of JEST.
- JEST significantly accelerates learning, reaching baseline performance with fewer training examples.
- The method achieves state-of-the-art results on ImageNet and COCO datasets.
- JEST+ achieved a new state-of-the-art on ImageNet and COCO with reduced compute resources.
- Flexi+ surpassed previous state-of-the-art using nine times less compute.
- Limitations include reliance on small curated reference datasets and potential computational overhead.
- The method's effectiveness depends on the quality of reference datasets.
- Generalizability to other domains or tasks remains to be fully explored.

# INSIGHTS:
- JEST accelerates multimodal learning by selecting highly learnable data batches efficiently.
- Prioritizing unlearned and learnable examples improves training efficiency and performance.
- Model-based scoring functions and heuristics guide effective data selection.
- Efficient scoring and multi-resolution training enhance training efficiency.
- Data quality bootstrapping leverages small curated datasets for larger dataset curation.
- JEST eliminates the need for foundation datasets, simplifying data curation.
- The method achieves state-of-the-art results with significantly fewer computational resources.
- Reliance on curated reference datasets may limit applicability in some scenarios.
- The method's generalizability to other domains needs further validation.

# QUOTES:
- "JEST aims to solve the problem of inefficient and costly manual curation of large-scale datasets."
- "JEST accelerates learning in multimodal tasks by selecting highly learnable batches from larger super batches."
- "The method addresses the challenge of slow and power law scaling of large-scale pre-training."
- "JEST prioritizes examples that are both unlearned and learnable, thus accelerating learning."
- "JEST uses model-based scoring functions to score entire subbatches of data."
- "Three scoring heuristics are used: hard learner, easy reference, and learnability."
- "Hard learner prioritizes batches with high loss under the learner model."
- "Easy reference prioritizes data that is easy for a pre-trained reference model."
- "Learnability combines these scores to upsample data that is unlearned and learnable."
- "JEST samples batches in proportion to their joint learnability."
- "Efficient scoring and multi-resolution training are leveraged for gains in efficiency."
- "Data quality bootstrapping uses a pre-trained reference model to guide larger dataset curation."
- "JEST surpasses the quality of the reference model on downstream tasks."
- "The method simplifies data curation by eliminating the need for foundation datasets."
- "JEST offers a more effective replacement for generic foundation datasets."
- "The method is validated through experiments comparing it to state-of-the-art models."
- "Visualizing the learnability matrix helps evaluate the efficacy of JEST."
- "JEST significantly accelerates learning, reaching baseline performance with fewer training examples."
- "The method achieves state-of-the-art results on ImageNet and COCO datasets."
- "JEST+ achieved a new state-of-the-art on ImageNet and COCO with reduced compute resources."

# HABITS:
- Prioritize examples that are both unlearned and learnable to improve training efficiency.
- Use model-based scoring functions to score subbatches based on losses from learner models.
- Leverage efficient scoring and multi-resolution training for gains in efficiency.
- Utilize small curated datasets to guide the curation of larger datasets.

# FACTS:
- JEST accelerates learning in multimodal tasks by selecting highly learnable batches from larger super batches.
- The method addresses slow and power law scaling of large-scale pre-training.
- JEST prioritizes examples that are both unlearned and learnable, improving training efficiency.
- It enables the use of small curated datasets to guide the curation of larger datasets.
- JEST uses model-based scoring functions to score subbatches based on losses from learner models.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
JEST accelerates multimodal learning by selecting highly learnable data batches, improving training efficiency and performance.

# RECOMMENDATIONS:
- Prioritize examples that are both unlearned and learnable to improve training efficiency.
- Use model-based scoring functions to score subbatches based on losses from learner models.
- Leverage efficient scoring and multi-resolution training for gains in efficiency.
- Utilize small curated datasets to guide the curation of larger datasets.