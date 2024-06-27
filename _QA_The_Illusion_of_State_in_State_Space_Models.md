# SUMMARY
Recent theoretical work reveals that Transformers and SSMs cannot handle inherently sequential problems like state tracking, unlike RNNs.

# IDEAS:
- Transformers are incapable of expressing inherently sequential computation.
- Transformers cannot handle simple state tracking problems such as composing sequences of permutations.
- Simple recurrent neural networks (RNNs) can naturally express state tracking problems.
- Transformers and SSMs cannot learn to compose permutations with a fixed number of layers.
- RNNs can compose permutations with just one layer.
- Transformers and SSMs are not equipped for state tracking and recurrent computation.
- Linear and Mamba-style SSMs struggle to learn to compose permutations.
- Arguments suggesting SSMs have an advantage over Transformers in state tracking are misguided.
- Linear and Mamba-style SSMs share the same limitations as Transformers in solving sequential problems.
- SSMs cannot express solutions to problems outside the complexity class 2^2.
- SSMs are constrained to solutions within the class 2^2, limiting their ability to handle complex state tracking tasks.
- Linear SSMs consist of state space layers using learned parameter matrices and projections.
- S6 models generalize linear SSMs by adding a selection mechanism inspired by dynamic gating in LSTMs.
- Linear SSMs use matrix powering to compute the convolutional form.
- S6 models involve iterated scalar multiplication due to diagonal matrix parameterization.
- Both linear SSMs and S6 models cannot solve inherently sequential problems beyond the complexity class 2^2.
- SSMs cannot solve 6^6 hard problems such as evaluating Boolean formulas or graph connectivity.
- SSMs are unable to compose permutations, unlike RNNs.
- SSMs cannot simulate true recurrent models in a realistic setting with a bounded number of layers.
- Adding non-linearity to the SSM architecture can increase its expressive power for state tracking.
- Introducing input-dependent transition matrices can transform SSMs into weighted finite automata (WFA) SSM layers.

# INSIGHTS:
- Transformers and SSMs cannot handle inherently sequential problems like state tracking, unlike RNNs.
- Linear and Mamba-style SSMs share the same limitations as Transformers in solving sequential problems.
- Adding non-linearity to the SSM architecture can increase its expressive power for state tracking.
- Introducing input-dependent transition matrices can transform SSMs into weighted finite automata (WFA) SSM layers.
- RNNs can compose permutations with just one layer, unlike Transformers and SSMs.
- Arguments suggesting SSMs have an advantage over Transformers in state tracking are misguided.
- Both linear SSMs and S6 models cannot solve inherently sequential problems beyond the complexity class 2^2.
- Linear SSMs use matrix powering to compute the convolutional form, while S6 models involve iterated scalar multiplication.
- SSMs cannot express solutions to problems outside the complexity class 2^2, limiting their ability to handle complex state tracking tasks.
- Theoretical analysis shows that Transformers and SSMs are limited in their ability to solve inherently sequential problems.

# QUOTES:
- "Transformers are incapable of expressing inherently sequential computation."
- "Transformers cannot handle simple state tracking problems such as composing sequences of permutations."
- "Simple recurrent neural networks (RNNs) can naturally express state tracking problems."
- "Transformers and SSMs cannot learn to compose permutations with a fixed number of layers."
- "RNNs can compose permutations with just one layer."
- "Transformers and SSMs are not equipped for state tracking and recurrent computation."
- "Linear and Mamba-style SSMs struggle to learn to compose permutations."
- "Arguments suggesting SSMs have an advantage over Transformers in state tracking are misguided."
- "Linear and Mamba-style SSMs share the same limitations as Transformers in solving sequential problems."
- "SSMs cannot express solutions to problems outside the complexity class 2^2."
- "SSMs are constrained to solutions within the class 2^2, limiting their ability to handle complex state tracking tasks."
- "Linear SSMs consist of state space layers using learned parameter matrices and projections."
- "S6 models generalize linear SSMs by adding a selection mechanism inspired by dynamic gating in LSTMs."
- "Linear SSMs use matrix powering to compute the convolutional form."
- "S6 models involve iterated scalar multiplication due to diagonal matrix parameterization."
- "Both linear SSMs and S6 models cannot solve inherently sequential problems beyond the complexity class 2^2."
- "SSMs cannot solve 6^6 hard problems such as evaluating Boolean formulas or graph connectivity."
- "SSMs are unable to compose permutations, unlike RNNs."
- "SSMs cannot simulate true recurrent models in a realistic setting with a bounded number of layers."
- "Adding non-linearity to the SSM architecture can increase its expressive power for state tracking."

# HABITS:
N/A

# FACTS:
N/A

# REFERENCES:
N/A

# ONE-SENTENCE TAKEAWAY
Transformers and SSMs are limited in handling inherently sequential problems like state tracking, unlike RNNs.

# RECOMMENDATIONS:
- Add non-linearity to the SSM architecture to increase its expressive power for state tracking.
- Introduce input-dependent transition matrices to transform SSMs into weighted finite automata (WFA) layers.