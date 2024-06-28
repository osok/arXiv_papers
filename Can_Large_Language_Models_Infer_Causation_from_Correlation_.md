# SUMMARY
The section introduces causal inference and its importance in reasoning. The authors propose a new task for NLP called Core 2 cause, which tests the ability of large language models to infer causation from correlation. They generate a data set of over 400k samples and evaluate the performance of 17 existing LLMs on this task, finding that none of them perform well. They also explore whether LLMs can learn the skill through fine-tuning but find that their causal inference skills are not robust.

# IDEAS:
- Causal inference is our capacity to deduce what causes what.
- Two methods to identify causality: experiential knowledge and formal causal reasoning.
- Large language models (LLMs) should develop the capability to infer causation from correlation.
- Core 2 cause is a new task designed to test LLMs' causal reasoning skills.
- The Core 2 cause data set contains over 400,000 samples.
- None of the 17 LLMs tested excelled in the causal inference task.
- Fine-tuned LLMs showed better performance but lacked robust causal inference skills.
- Directed graphical causal models (DGCMs) visualize relationships between variables.
- DGCMs assume graphs are directed acyclic to avoid complexity.
- D-separation helps establish conditional independence between nodes in a DAG.
- The Markov property states each node is conditionally independent of its non-descendants given its parents.
- Markov equivalence class (MEC) groups DAGs that induce the same joint distribution.
- The Peter-Clark (PC) algorithm identifies causal relationships using conditional independence and the causal Markov assumption.
- The Core 2 cause task involves learning a function to determine the validity of correlation statements and causal hypotheses.
- Graph isomorphism checks ensure uniqueness in generated DAGs.
- D-separation sets are used to form statistical correlations and cluster causal graphs into MECs.
- Six common types of causal relationships are considered in hypotheses generation.
- Ground truth validity labels are assigned based on the necessity of hypothesized causal relations.
- Correlations and hypotheses are verbalized into natural language statements.
- The Core 2 cause data set includes 415,944 samples with 18.57% valid samples.
- A diverse list of LLMs, including BERT-based and GPT-based models, were tested on the Core 2 cause data set.
- Fine-tuned models showed significant performance improvement, with Roberta large MNLI achieving a 94.74 F1 score.
- Robustness tests include paraphrasing hypotheses and reversing variable names.
- Performance drops significantly under robustness tests, indicating sensitivity to language changes and variable refactorization.
- Existing research on causal reasoning in NLP focuses on empirical knowledge, while Core 2 cause emphasizes pure causal inference skills.
- Future research should explore larger graphs and hidden confounders in causal inference tasks.

# INSIGHTS:
- Causal inference is crucial for establishing accurate cause-effect relationships between variables or events.
- Large language models need to develop robust causal reasoning skills beyond capturing statistical correlations.
- Directed graphical causal models (DGCMs) help visualize and understand complex variable interactions.
- D-separation is essential for determining conditional independence in directed acyclic graphs (DAGs).
- Markov equivalence class (MEC) groups DAGs with identical statistical properties, highlighting the complexity of inferring causation from correlation.
- The Peter-Clark (PC) algorithm efficiently identifies causal relationships using conditional independence principles.
- Fine-tuning LLMs can improve performance in causal inference tasks but may not ensure robustness in unfamiliar scenarios.
- Robustness tests reveal that LLMs may overfit training data rather than genuinely acquiring reasoning skills.
- Future research should address hidden confounders and larger graphs to enhance causal inference capabilities in LLMs.

# QUOTES:
- "Causal inference is our capacity to deduce what causes what."
- "Large language models should develop the capability to infer causation from correlation."
- "Core 2 cause is a new task designed to test LLMs' causal reasoning skills."
- "None of the 17 LLMs tested excelled in the causal inference task."
- "Fine-tuned LLMs showed better performance but lacked robust causal inference skills."
- "Directed graphical causal models visualize relationships between variables."
- "D-separation helps establish conditional independence between nodes in a DAG."
- "The Markov property states each node is conditionally independent of its non-descendants given its parents."
- "Markov equivalence class groups DAGs that induce the same joint distribution."
- "The Peter-Clark algorithm identifies causal relationships using conditional independence and the causal Markov assumption."
- "Graph isomorphism checks ensure uniqueness in generated DAGs."
- "D-separation sets are used to form statistical correlations and cluster causal graphs into MECs."
- "Six common types of causal relationships are considered in hypotheses generation."
- "Ground truth validity labels are assigned based on the necessity of hypothesized causal relations."
- "Correlations and hypotheses are verbalized into natural language statements."
- "The Core 2 cause data set includes 415,944 samples with 18.57% valid samples."
- "A diverse list of LLMs, including BERT-based and GPT-based models, were tested on the Core 2 cause data set."
- "Fine-tuned models showed significant performance improvement, with Roberta large MNLI achieving a 94.74 F1 score."
- "Robustness tests include paraphrasing hypotheses and reversing variable names."
- "Performance drops significantly under robustness tests, indicating sensitivity to language changes and variable refactorization."

# HABITS:
- Regularly test models on new tasks to assess their capabilities beyond standard benchmarks.
- Fine-tune models with specific data sets to improve their performance on targeted tasks.
- Conduct robustness tests to ensure models' skills are not limited to training data overfitting.
- Use directed graphical causal models (DGCMs) to visualize complex relationships between variables.
- Apply D-separation principles to determine conditional independence in directed acyclic graphs (DAGs).
- Utilize graph isomorphism checks to ensure uniqueness in generated graphs for data sets.
- Generate ground truth validity labels based on the necessity of hypothesized causal relations across all graphs in a MEC.
- Verbalize correlations and hypotheses into natural language statements for easier interpretation.

# FACTS:
- Causal inference allows us to deduce accurate cause-effect relationships between variables or events.
- Large language models (LLMs) currently lack robust causal reasoning skills despite capturing statistical correlations.
- Directed graphical causal models (DGCMs) are used to represent relationships among variables in a graph format.
- D-separation is a key concept for establishing conditional independence between nodes in a directed acyclic graph (DAG).
- The Markov property states that each node is conditionally independent of its non-descendants given its parents in a DAG.
- Markov equivalence class (MEC) groups DAGs that induce the same joint distribution, highlighting the complexity of inferring causation from correlation.
- The Peter-Clark (PC) algorithm identifies causal relationships using principles of conditional independence and the causal Markov assumption.
- The Core 2 cause data set contains over 400,000 samples designed to test LLMs' ability to infer causation from correlation.
- Fine-tuned LLMs showed improved performance but lacked robustness when exposed to unfamiliar scenarios or adversarial attacks.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
Large language models need robust causal reasoning skills beyond statistical correlations for accurate cause-effect relationship inference.

# RECOMMENDATIONS:
- Develop large language models' capability to infer causation from correlation for better reasoning skills.
- Use directed graphical causal models (DGCMs) to visualize complex relationships between variables effectively.
- Apply D-separation principles to determine conditional independence in directed acyclic graphs (DAGs).
- Utilize graph isomorphism checks to ensure uniqueness in generated graphs for data sets.
- Generate ground truth validity labels based on hypothesized causal relations across all graphs in a MEC.
- Verbalize correlations and hypotheses into natural language statements for easier interpretation.
- Conduct robustness tests like paraphrasing hypotheses and reversing variable names to ensure model reliability.
- Explore larger graphs and hidden confounders in future research for enhanced causal inference capabilities.