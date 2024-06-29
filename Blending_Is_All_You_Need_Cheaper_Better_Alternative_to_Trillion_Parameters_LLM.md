# SUMMARY
The authors discuss the limitations of large language models (LLMs) in chat AI applications and propose an innovative approach called Blended, where a group of moderately sized LLMs collaborate to form a chat AI that outperforms systems with significantly more parameters.

# IDEAS:
- Large language models (LLMs) require significant computational resources and are often only accessible through public APIs.
- Blended combines responses from multiple smaller LLMs to create a highly capable and engaging chat AI.
- Blended outperformed OpenAI's ChatGPT, a model with over 175 billion parameters, on the Chai platform.
- Users found Blended more engaging, entertaining, and useful than ChatGPT-based chat AIs.
- Early chat AIs were rule-based but evolved into generative retrieval-based models with pre-trained Transformer language models.
- Human feedback is crucial in training chat AIs to align with human expectations of engaging conversations.
- Blended uses existing small conversational LLMs to create a single chat AI with diverse and engaging responses.
- Combining systems has been explored in deep learning using methods like stacking, negative correlation learning, and probability averaging.
- Sequence-level ensembling approaches average conditional token-level probabilities of multiple systems.
- Minimum Bayes Risk (MBR) decoding selects the predicted best system output using system outputs.
- LLM Blender blends outputs from different language models by ranking and fusing top outputs using a deep sequence-to-sequence system.
- Blended stochastically selects the system that generates the next response, allowing for model blending in multi-turn conversations.
- Evaluating chat AI quality involves measuring user retention and engagement as meaningful performance indicators.
- User retention measures the fraction of users returning to the platform after joining.
- User engagement is measured by the average time a user spends on the platform per visit.
- Blended outperformed OpenAI GPT-3.5 in user engagement and retention despite having fewer parameters.
- Blending multiple smaller systems can improve user experience without increasing inference costs.
- The Blended system had the highest initial engagement and best decay rate for engagement ratio.
- Future research will explore expanding the selection set of component chat AIs to increase conversation diversity and richness.
- Optimal selection distribution involves using a deep learning classifier to predict the probability distribution over the chat AI selection set.
- The classifier identifies the chat AI most likely to provide the next engaging response based on human feedback signals.
- Introducing new chat AIs to the selection set can be done without risking a drop in Blended performance.

# INSIGHTS:
- Combining smaller LLMs can outperform larger models in user engagement and retention.
- Human feedback is essential for training chat AIs to meet user expectations.
- Blending multiple systems can create more diverse and engaging conversations.
- Evaluating chat AI quality through user retention and engagement provides meaningful performance metrics.
- Expanding the selection set of component chat AIs can enhance conversation diversity without increasing computational costs.

# QUOTES:
- "Blended combines responses from multiple smaller LLMs to create a highly capable and engaging chat AI."
- "Users found Blended more engaging, entertaining, and useful than ChatGPT-based chat AIs."
- "Early chat AIs were rule-based but evolved into generative retrieval-based models with pre-trained Transformer language models."
- "Human feedback is crucial in training chat AIs to align with human expectations of engaging conversations."
- "Blended uses existing small conversational LLMs to create a single chat AI with diverse and engaging responses."
- "Combining systems has been explored in deep learning using methods like stacking, negative correlation learning, and probability averaging."
- "Sequence-level ensembling approaches average conditional token-level probabilities of multiple systems."
- "Minimum Bayes Risk (MBR) decoding selects the predicted best system output using system outputs."
- "LLM Blender blends outputs from different language models by ranking and fusing top outputs using a deep sequence-to-sequence system."
- "Blended stochastically selects the system that generates the next response, allowing for model blending in multi-turn conversations."
- "Evaluating chat AI quality involves measuring user retention and engagement as meaningful performance indicators."
- "User retention measures the fraction of users returning to the platform after joining."
- "User engagement is measured by the average time a user spends on the platform per visit."
- "Blended outperformed OpenAI GPT-3.5 in user engagement and retention despite having fewer parameters."
- "Blending multiple smaller systems can improve user experience without increasing inference costs."
- "The Blended system had the highest initial engagement and best decay rate for engagement ratio."
- "Future research will explore expanding the selection set of component chat AIs to increase conversation diversity and richness."
- "Optimal selection distribution involves using a deep learning classifier to predict the probability distribution over the chat AI selection set."
- "The classifier identifies the chat AI most likely to provide the next engaging response based on human feedback signals."
- "Introducing new chat AIs to the selection set can be done without risking a drop in Blended performance."

# HABITS:
- Regularly measure user retention and engagement to evaluate chat AI performance.
- Use human feedback to train chat AIs for better alignment with user expectations.
- Experiment with combining multiple smaller LLMs for improved conversational quality.
- Continuously expand the selection set of component chat AIs for richer conversations.
- Train deep learning classifiers to optimize model selection distribution.

# FACTS:
- Large language models (LLMs) require significant computational resources and are often only accessible through public APIs.
- Blended outperformed OpenAI's ChatGPT, a model with over 175 billion parameters, on the Chai platform.
- Early chat AIs were rule-based but evolved into generative retrieval-based models with pre-trained Transformer language models.
- Human feedback is crucial in training chat AIs to align with human expectations of engaging conversations.
- Combining systems has been explored in deep learning using methods like stacking, negative correlation learning, and probability averaging.

# REFERENCES:
- OpenAI's ChatGPT
- Chai platform
- Pigmillion 6B
- Chai model 6B
- Vonia 13B
- OpenAI Da Vinci GPT 3.5

# ONE-SENTENCE TAKEAWAY
Combining multiple smaller LLMs can create more engaging and efficient chat AIs than single large models.

# RECOMMENDATIONS:
- Combine responses from multiple smaller LLMs for highly capable and engaging chat AI.
- Use human feedback to train chat AIs for better alignment with user expectations.
- Measure user retention and engagement as meaningful performance indicators for chat AIs.
- Expand the selection set of component chat AIs for richer conversation diversity.
- Train deep learning classifiers to optimize model selection distribution for better responses.