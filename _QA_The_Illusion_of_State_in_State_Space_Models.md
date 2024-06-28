# SUMMARY
Recent theoretical work reveals that Transformers and state space models (SSMs) cannot handle inherently sequential computations, unlike simple recurrent neural networks (RNNs).

# IDEAS:
- Transformers cannot express inherently sequential computation, limiting their ability to handle state tracking problems.
- Simple RNNs can naturally express state tracking problems like composing sequences of permutations.
- Transformers and SSMs cannot learn to compose permutations with a fixed number of layers.
- RNNs can solve permutation composition with just one layer, unlike Transformers and SSMs.
- Theoretical analysis shows that SSMs are not more recurrent or capable of tracking state than Transformers.
- Linear and Mamba-style SSMs struggle to learn to compose permutations with a fixed number of layers.
- Arguments suggesting SSMs have an advantage over Transformers in state tracking are misguided.
- Linear SSMs and their generalizations are in the complexity class 5-uniform 2, similar to Transformers.
- SSMs cannot solve inherently sequential problems, including state tracking problems like permutation composition.
- SSMs, despite their stateful design, are constrained to solutions within the class 2-complexity.
- Linear SSMs consist of state space layers using learned parameter matrices and projections.
- S6 models generalize linear SSMs by adding a selection mechanism inspired by dynamic gating in LSTMs.
- S6 models involve iterated scalar multiplication due to diagonal matrix parameterization.
- Both linear SSMs and S6 models cannot solve 6-hard problems like evaluating Boolean formulas or graph connectivity.
- SSMs cannot simulate true recurrent models in a realistic setting with a bounded number of layers.
- Adding non-linearity to the SSM architecture can make it more like an RNN.
- Input-dependent transition matrices can transform an SSM into a weighted finite automaton (WFA) SSM layer.
- These extensions aim to bridge the gap in expressive power between SSMs and true recurrent models like RNNs.
- The paper highlights that SSMs cannot solve the 3-word problem, unlike RNNs.
- The addition of non-linearity allows the SSM to have a recurrent form effectively like an RNN.

# INSIGHTS:
- Transformers and SSMs share limitations in handling inherently sequential computations.
- Simple RNNs outperform Transformers and SSMs in state tracking tasks like permutation composition.
- Theoretical analysis disproves the belief that SSMs are more recurrent than Transformers.
- Linear and Mamba-style SSMs are limited to the complexity class 5-uniform 2, similar to Transformers.
- Adding non-linearity and input-dependent transition matrices can enhance SSM's expressive power.
- Both linear SSMs and S6 models cannot solve complex state tracking problems beyond class 2-complexity.
- Extensions like non-linearity and input-dependent matrices aim to make SSMs more like RNNs.
- Despite their design, SSMs cannot handle complex state tracking tasks such as evaluating Boolean formulas.
- The paper establishes that RNNs can solve permutation composition with fewer layers than SSMs or Transformers.
- The proposed extensions aim to bridge the gap between SSMs and true recurrent models.

# QUOTES:
- "Transformers cannot express inherently sequential computation, limiting their ability to handle state tracking problems."
- "Simple RNNs can naturally express state tracking problems like composing sequences of permutations."
- "Transformers and SSMs cannot learn to compose permutations with a fixed number of layers."
- "RNNs can solve permutation composition with just one layer, unlike Transformers and SSMs."
- "Theoretical analysis shows that SSMs are not more recurrent or capable of tracking state than Transformers."
- "Linear and Mamba-style SSMs struggle to learn to compose permutations with a fixed number of layers."
- "Arguments suggesting SSMs have an advantage over Transformers in state tracking are misguided."
- "Linear SSMs and their generalizations are in the complexity class 5-uniform 2, similar to Transformers."
- "SSMs cannot solve inherently sequential problems, including state tracking problems like permutation composition."
- "SSMs, despite their stateful design, are constrained to solutions within the class 2-complexity."
- "Linear SSMs consist of state space layers using learned parameter matrices and projections."
- "S6 models generalize linear SSMs by adding a selection mechanism inspired by dynamic gating in LSTMs."
- "S6 models involve iterated scalar multiplication due to diagonal matrix parameterization."
- "Both linear SSMs and S6 models cannot solve 6-hard problems like evaluating Boolean formulas or graph connectivity."
- "SSMs cannot simulate true recurrent models in a realistic setting with a bounded number of layers."
- "Adding non-linearity to the SSM architecture can make it more like an RNN."
- "Input-dependent transition matrices can transform an SSM into a weighted finite automaton (WFA) SSM layer."
- "These extensions aim to bridge the gap in expressive power between SSMs and true recurrent models like RNNs."
- "The paper highlights that SSMs cannot solve the 3-word problem, unlike RNNs."
- "The addition of non-linearity allows the SSM to have a recurrent form effectively like an RNN."

# HABITS:
N/A

# FACTS:
N/A

# REFERENCES:
N/A

# ONE-SENTENCE TAKEAWAY
Transformers and state space models (SSMs) are limited in handling inherently sequential computations, unlike simple recurrent neural networks (RNNs).

# RECOMMENDATIONS:
- Consider using simple RNNs for tasks involving inherently sequential computations and state tracking problems.
- Be cautious of claims suggesting that SSMs have an advantage over Transformers in terms of recurrence.
- Explore adding non-linearity to the SSM architecture to enhance its expressive power for state tracking tasks.
- Investigate input-dependent transition matrices as a way to transform an SSM into a weighted finite automaton layer.
- Recognize that both linear and Mamba-style SSMs share limitations with Transformers in solving sequential problems.