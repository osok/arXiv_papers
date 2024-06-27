# SUMMARY
The authors discuss the evolution of Transformers in NLP, redefining decoder-only Transformers as multi-state RNNs (MS RNNs). They introduce Tova, a compression policy that improves performance and reduces memory consumption.

# IDEAS:
- Transformers replaced RNNs in NLP due to their ability to access each token directly.
- Decoder-only Transformers generate output auto-regressively, similar to RNNs maintaining state.
- Redefining decoder-only Transformers as multi-state RNNs (MS RNNs) generalizes traditional RNNs.
- Transformers can be seen as MS RNNs with an infinite number of states.
- Compressing Transformers into finite MS RNNs limits the number of tokens processed at each step.
- Tova, a new compression policy, selects tokens based on attention scores.
- Tova outperforms existing policies with minimal performance degradation.
- Not all recent tokens are important to keep in memory; some can be safely dropped.
- Keeping the first token and important tokens like possessive nouns is crucial.
- Transformer decoders predict the next token using masking and auto-regressive decoding.
- Multi-state RNNs use a matrix of states instead of a single vector.
- Transformers trained up to a specific length struggle to extrapolate beyond that.
- Compression policies convert infinite MS RNNs into finite ones.
- FIFO strategy discards the oldest state when multi-state reaches capacity.
- Tova retains top states based on attention weights of the last token only.
- Tova performs better layer-wise rather than headwise.
- Tova achieves results similar to infinite MS RNN models in various tasks.
- Pre-trained Transformers behave like finite MS RNNs in practice.
- Limiting multi-state size results in shorter generated text.
- Recent tokens are often preserved, but many older tokens are also kept.
- Increasing batch size using Tova improves hardware utilization.
- Simplifying Transformers bridges the gap between them and RNNs.

# INSIGHTS:
- Transformers' direct token access revolutionized NLP, surpassing RNNs' sequential processing.
- Auto-regressive decoding in Transformers aligns with RNNs' state maintenance principle.
- Multi-state RNNs generalize traditional RNNs by using a matrix of states.
- Compressing Transformers into finite MS RNNs optimizes memory usage without significant performance loss.
- Tova's attention-based token selection enhances efficiency and reduces memory consumption.
- Not all recent tokens are crucial; strategic token retention improves model performance.
- Initial tokens and specific important tokens play a vital role in successful decoding.
- Transformer decoders' masking technique enables effective next-token prediction.
- Multi-state RNNs' matrix of states offers a more flexible approach than single-vector RNNs.
- Pre-trained Transformers often function as finite MS RNNs despite their theoretical infinite capacity.

# QUOTES:
- "Transformers replaced RNNs in NLP due to their ability to access each token directly."
- "Decoder-only Transformers generate output auto-regressively, similar to RNNs maintaining state."
- "Redefining decoder-only Transformers as multi-state RNNs (MS RNNs) generalizes traditional RNNs."
- "Transformers can be seen as MS RNNs with an infinite number of states."
- "Compressing Transformers into finite MS RNNs limits the number of tokens processed at each step."
- "Tova, a new compression policy, selects tokens based on attention scores."
- "Tova outperforms existing policies with minimal performance degradation."
- "Not all recent tokens are important to keep in memory; some can be safely dropped."
- "Keeping the first token and important tokens like possessive nouns is crucial."
- "Transformer decoders predict the next token using masking and auto-regressive decoding."
- "Multi-state RNNs use a matrix of states instead of a single vector."
- "Transformers trained up to a specific length struggle to extrapolate beyond that."
- "Compression policies convert infinite MS RNNs into finite ones."
- "FIFO strategy discards the oldest state when multi-state reaches capacity."
- "Tova retains top states based on attention weights of the last token only."
- "Tova performs better layer-wise rather than headwise."
- "Tova achieves results similar to infinite MS RNN models in various tasks."
- "Pre-trained Transformers behave like finite MS RNNs in practice."
- "Limiting multi-state size results in shorter generated text."
- "Recent tokens are often preserved, but many older tokens are also kept."

# HABITS:
- Regularly evaluate models using various benchmarks and Transformer LLM families.
- Use attention scores to dynamically select important tokens during decoding.
- Test different compression policies to optimize model performance and memory usage.
- Analyze token retention processes to understand model behavior better.
- Focus on long-range evaluations for comprehensive model assessment.

# FACTS:
- Transformers replaced RNNs in NLP due to their direct token access capability.
- Decoder-only Transformers generate output auto-regressively, maintaining state like RNNs.
- Multi-state RNNs use a matrix of states instead of a single vector for flexibility.
- Compressing Transformers into finite MS RNNs optimizes memory usage without significant performance loss.
- Tova's attention-based token selection enhances efficiency and reduces memory consumption.

# REFERENCES:
- PG19 test set for evaluating long-range language models
- Zero Scrolls Benchmark for long-range summarization and question answering
- Transformer LLM families: Llama 2, Mistol, and Y
- Mythologic, a Llama 2 13B version fine-tuned for story generation

# ONE-SENTENCE TAKEAWAY
Tova's attention-based token selection optimizes Transformer performance and memory usage, redefining them as efficient multi-state RNNs.

# RECOMMENDATIONS:
- Use Tova for efficient token selection based on attention scores during decoding.
- Compress Transformer models into finite MS RNNs to optimize memory usage.
- Retain initial tokens and important tokens like possessive nouns for successful decoding.
- Evaluate models using various benchmarks and Transformer LLM families for comprehensive assessment.
- Analyze token retention processes to understand model behavior better.