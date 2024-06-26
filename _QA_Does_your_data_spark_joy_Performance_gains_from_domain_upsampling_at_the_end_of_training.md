# SUMMARY
The paper addresses optimizing pre-training data mixes for large language models (LLMs) using a novel domain upsampling strategy to balance common crawl and domain-specific data.

# IDEAS:
- The main problem is determining the optimal strategy for mixing common crawl and domain-specific data.
- Previous works struggled with balancing heavily processed common crawl data and domain-specific datasets.
- Limited disclosure of pre-training data contents in modern language models.
- Difficulty and cost of validating data mixing strategies at a large scale.
- Lack of open research on pre-training data for LLMs.
- Domain upsampling modifies the data mixture at the end of training to improve LLM pre-training.
- Initial baseline mix includes large-scale common crawl, small-scale common crawl, domain-specific data, and code.
- Domain upsampling increases representation of domain-specific and code datasets while removing large-scale common crawl.
- Biasing the model towards high information density domains improves performance on challenging benchmarks.
- Domain upsampling boosts model performance on GSM 8K and human avow by approximately 10 percentage points.
- High-quality domain-specific data and code enhance mathematical and programming abilities.
- Performance enhancement does not compromise general language modeling capabilities.
- Overall improvement in model performance as measured by Gauntlet v0.3 core average.
- Domain upsampling improves world knowledge as indicated by MMLU and Gauntlet v0.3 subset scores.
- Adjusting the duration of domain upsampling navigates the tradeoff between specific domains and general capabilities.
- Increasing domain upsampling beyond 20% improves math and coding benchmarks but affects general language modeling.
- Strategic timing and balancing of domain upsampling achieve optimal performance across benchmarks.
- Domain upsampling led to improvements of up to 6.90 percentage points on MMLU.
- Improvements of 8.26 percentage points on GSM 8K due to domain upsampling.
- HumanEval saw improvements of 6.17 percentage points with domain upsampling.
- Experiments with varying durations of domain upsampling demonstrate tradeoffs between specific domains and general models.
- Data mix proportions for domain upsampling were not definitively better than initial mix for overall performance.
- Domain upsampling provides a flop-efficient tool to balance specific domain capabilities and general proficiency.
- Experimental design involved starting with a checkpoint and changing mixing proportions for remaining tokens.
- Emphasizing high information density domains at the end of training benefits the model.
- Removing math-heavy pre-training data during domain upsampling quantifies impact on benchmarks.
- Cost-effective way to measure impact of pre-training datasets on model capabilities.
- Domain upsampling enhances model performance on specific tasks with targeted changes to data mix.
- Study's findings suggest domain upsampling is effective and cost-efficient for improving pre-training data mix.
- Significant performance boosts achieved on challenging benchmarks without compromising general capabilities.
- Performance levels comparable to models trained for twice the number of tokens but at half the training flops.
- Domain upsampling is a flop-efficient tool to analyze individual dataset impacts on model capabilities.

# INSIGHTS:
- Balancing common crawl and domain-specific data is crucial for optimal LLM pre-training strategies.
- Domain upsampling modifies data mix proportions at training's end, enhancing model performance cost-effectively.
- High-quality domain-specific data significantly boosts mathematical and programming abilities in LLMs.
- Strategic timing of domain upsampling balances specific domain enhancements with general language modeling.
- Domain upsampling achieves significant performance boosts without compromising general language capabilities.
- Flop-efficient tools like domain upsampling make pre-training data experiments more accessible and cost-effective.
- Emphasizing high information density domains at training's end benefits model performance on specific tasks.
- Simple heuristics for selecting new data mix proportions can have strong positive effects on LLMs.
- Domain upsampling provides insights into the importance of specific subsets of pre-training data.
- Adjusting domain upsampling duration navigates tradeoffs between specific domains and general capabilities.

# QUOTES:
- "The main problem is determining the optimal strategy for mixing common crawl and domain-specific data."
- "Previous works struggled with balancing heavily processed common crawl data and domain-specific datasets."
- "Limited disclosure of pre-training data contents in modern language models."
- "Difficulty and cost of validating data mixing strategies at a large scale."
- "Lack of open research on pre-training data for LLMs."
- "Domain upsampling modifies the data mixture at the end of training to improve LLM pre-training."
- "Initial baseline mix includes large-scale common crawl, small-scale common crawl, domain-specific data, and code."
- "Domain upsampling increases representation of domain-specific and code datasets while removing large-scale common crawl."
- "Biasing the model towards high information density domains improves performance on challenging benchmarks."
- "Domain upsampling boosts model performance on GSM 8K and human avow by approximately 10 percentage points."
- "High-quality domain-specific data and code enhance mathematical and programming abilities."
- "Performance enhancement does not compromise general language modeling capabilities."
- "Overall improvement in model performance as measured by Gauntlet v0.3 core average."
- "Domain upsampling improves world knowledge as indicated by MMLU and Gauntlet v0.3 subset scores."
- "Adjusting the duration of domain upsampling navigates the tradeoff between specific domains and general capabilities."
- "Increasing domain upsampling beyond 20% improves math and coding benchmarks but affects general language modeling."
- "Strategic timing and balancing of domain upsampling achieve optimal performance across benchmarks."
- "Domain upsampling led to improvements of up to 6.90 percentage points on MMLU."
- "Improvements of 8.26 percentage points on GSM 8K due to domain upsampling."
- "HumanEval saw improvements of 6.17 percentage points with domain upsampling."

# HABITS:
- Adjusting data mix proportions strategically towards the end of training sessions.
- Emphasizing high information density domains during critical training phases.
- Conducting experiments with varying durations of specific interventions like domain upsampling.
- Using simple heuristics for selecting new data mix proportions during training adjustments.
- Removing subsets of less relevant pre-training data during targeted interventions.

# FACTS:
- Balancing common crawl and domain-specific data is crucial for optimal LLM pre-training strategies.
- Domain upsampling modifies data mix proportions at training's end, enhancing model performance cost-effectively.
- High-quality domain-specific data significantly boosts mathematical and programming abilities in LLMs.
- Strategic timing of domain upsampling balances specific domain enhancements with general language modeling.
- Domain upsampling achieves significant performance boosts without compromising general language capabilities.

# REFERENCES:
None mentioned explicitly in the input.

# ONE-SENTENCE TAKEAWAY
Domain upsampling effectively balances specific domain enhancements with general language modeling, boosting LLM performance cost-efficiently.

# RECOMMENDATIONS:
- Balance common crawl and domain-specific data for optimal LLM pre-training strategies.
- Modify data mix proportions at training's end to enhance model performance cost-effectively.
- Emphasize high-quality domain-specific data to boost mathematical and programming abilities in LLMs.
- Strategically time domain upsampling to balance specific enhancements with general language modeling capabilities.
- Use simple heuristics for selecting new data mix proportions during training adjustments.