# SUMMARY
The authors introduce Fast BT, a variant of the BERT architecture, optimizing feedforward layers with fast feedforward networks for significant speed improvements.

# IDEAS:
- Fast BT replaces feedforward layers in BERT with fast feedforward networks.
- Fast BT performs on par with other BERT models but is exponentially faster.
- Fast feedforward networks use conditional matrix multiplication (CMM) for speed.
- CMM organizes neurons into a balanced binary tree, executing one branch per input.
- Traditional feedforward networks use dense matrix multiplication (DMM).
- Fast BT uses only 0.03% of its neurons for inference.
- Fast BT achieves a 78x speedup over traditional BERT models.
- Dense matrix multiplication is highly optimized, limiting further speedups.
- Fast BT models retain at least 96.0% of BERT's predictive performance.
- Performance decreases with increased depth of fast feedforward networks.
- Fast BT models trained for one day on a single GPU perform well.
- Fast BT's best model uses only 0.3% of its neurons, matching BERT's performance.
- Fast feedforward networks can significantly speed up large language models like GPT-3.
- Efficient CMM implementation is crucial for maximizing speedups.
- Single-threaded CPU DMM benefits from replacing DMM with CMM.
- Efficient CMM implementations need optimal caching for tree traversal.
- Fast BT's algorithm is compatible with existing hardware and processes.
- Fast BT uses fewer executions of per-element MAC instructions.
- Efficient CMM implementations manage caching optimally for tree traversal.
- Fast BT's CPU inference uses Intel MKL and custom CUDA kernels for GPU inference.
- Fast BT's GPU inference uses PyTorch kernels and custom CUDA implementations.
- Fast BT's best implementations are significantly faster than traditional feedforward layers.
- Hybrid vector-level sparse tensors could further improve fast feedforward inference.
- Native CMM implementation in Intel MKL and NVIDIA cuBLAS could deliver a 304x speed improvement.

# INSIGHTS:
- Conditional matrix multiplication (CMM) optimizes neuron usage in fast feedforward networks.
- Fast BT achieves significant speedups while maintaining high predictive performance.
- Efficient CMM implementation is key to maximizing speed improvements in neural networks.
- Fast BT demonstrates the potential of conditional neural execution in language modeling.
- Replacing dense matrix multiplication with CMM can benefit single-threaded CPU inference.
- Optimal caching strategies are crucial for efficient CMM implementations.
- Fast BT's design leverages balanced binary trees for faster inference.
- Simplifying activation functions and removing output biases improves fast feedforward networks.
- Training fast BT models on a single GPU retains high predictive performance.
- Future efforts should focus on efficient CMM implementation for further speedups.

# QUOTES:
- "Fast BT replaces the feedforward layers with fast feedforward networks."
- "Fast Bert performs just as well as other BERT-like models."
- "The intermediate layers of Fast BT are designed to be exponentially faster."
- "Inference in an FFF is like performing a conditional matrix multiplication (CMM)."
- "All neurons are used only by some inputs."
- "Dense matrix multiplication is the most optimized mathematical operation in computing history."
- "Fast Bert uses only 0.03% of its neurons for inference."
- "We achieve a 78x speedup and not a 341x speedup."
- "Fast Bert models trained for one day on a single GPU retain at least 96.0% of the predictive performance."
- "Fast feedforward networks have the potential to greatly speed up large language models."
- "The key to this speedup is the operation of conditional matrix multiplication."
- "Efficient implementations of CMM need to manage caching optimally for tree traversal."
- "Single-threaded CPU DMM benefits from replacing DMM with CMM."
- "Efficient CMM implementations distribute the matrix multiplication workload in a way that maximizes the use of distributed cache."
- "Fast feedforward layers perform inference 48 times and 78 times faster than the fastest feedforward layer implementation respectively."
- "Hybrid vector-level sparse tensors could further improve fast feedforward inference."

# HABITS:
- Simplifying activation functions and removing output biases improves network efficiency.
- Training models on a single GPU for one day retains high predictive performance.
- Extending training epochs for specific tasks can significantly improve performance.

# FACTS:
- Fast BT replaces traditional feedforward layers with fast feedforward networks.
- Conditional matrix multiplication (CMM) organizes neurons into a balanced binary tree.
- Dense matrix multiplication (DMM) computes interactions of all rows with all columns.
- Fast BT uses only 0.03% of its neurons for inference.
- Dense matrix multiplication is highly optimized in computing history.
- Fast BT achieves a 78x speedup over traditional BERT models.
- Fast BT models retain at least 96.0% of BERT's predictive performance.
- Performance decreases with increased depth of fast feedforward networks.
- Efficient CMM implementation is crucial for maximizing speedups.
- Single-threaded CPU DMM benefits from replacing DMM with CMM.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
Fast BT optimizes BERT's feedforward layers with fast feedforward networks, achieving significant speedups while maintaining high predictive performance.

# RECOMMENDATIONS:
- Replace traditional feedforward layers with fast feedforward networks for speed improvements.
- Use conditional matrix multiplication (CMM) to optimize neuron usage in neural networks.
- Focus on efficient CMM implementation to maximize speed improvements in neural networks.
- Simplify activation functions and remove output biases to improve network efficiency.
- Train models on a single GPU for one day to retain high predictive performance.