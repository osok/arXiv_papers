# SUMMARY
The paper discusses methods to build robust AI systems, focusing on defending superhuman Go agents against adversarial attacks using various defense strategies.

# IDEAS:
- The new method aims to build robust AI systems, especially superhuman Go agents resilient to adversarial attacks.
- Defense strategies include adversarial training with hand-constructed positions, iterated adversarial training, and using a Vision Transformer (ViT).
- The goal is to make AI agents minimally exploitable by adversaries, preventing game-losing blunders.
- Iterated adversarial training involves alternately training a victim agent and an adversary agent over multiple rounds.
- The victim is trained to be robust against the latest adversary, and then a new adversary is trained to attack this hardened victim.
- Training continues until the victim's win rate plateaus or a set maximum compute budget is reached.
- Each defender learned effective defenses but did not achieve 100% win rates, indicating partial protection.
- The final victim remains vulnerable even at high visits, showing the challenge of complete robustness.
- The method highlights the difficulty of defending against all possible attacks in Go.
- Theoretical benefits include insights into achieving robustness in AI systems against adversarial attacks.
- Practical benefits include evaluating defenses like adversarial training and using ViT instead of CNN.
- None of the defenses make attacks impossible but increase the compute needed for successful attacks.
- The method suggests future research avenues like developing new attack algorithms and improving sample efficiency.
- Validation involved testing three defenses: positional adversarial training, iterated adversarial training, and ViT backbone.
- Positional adversarial training showed vulnerabilities despite initial defense.
- Iterated adversarial training resulted in victims largely robust to observed attacks but still vulnerable to new ones.
- ViT-based Go AI was tested and found exploitable by new attacks despite reaching superhuman levels.
- Results showed victims were robust to observed attacks but not new ones, with final victims still vulnerable.
- Final simulated adversary won 42% of the time against the victim even at 65,536 visits.
- Defenses made attacks harder but did not provide a complete solution; attacks were still possible with minimal compute.
- Limitations include the inability to provide a complete solution against adversarial attacks in Go.
- Defenses did not achieve human-level robustness as humans could still execute several attacks.
- Defenses were vulnerable to new attacks, indicating no robustness to new strategies.
- The method was bottlenecked by the attack component, requiring more compute than the defense component.
- Further research is needed to reduce attack time and train against a larger corpus of attacks.

# INSIGHTS:
- Achieving complete robustness in AI systems against adversarial attacks remains a significant challenge.
- Iterated adversarial training improves defense but does not eliminate vulnerability to new attacks.
- Increasing compute requirements for successful attacks enhances defense but doesn't ensure complete protection.
- Balancing offense and defense strategies is crucial for robust AI systems.
- Future research should focus on developing efficient attack algorithms and improving sample efficiency in training.

# QUOTES:
- "The new method aims to build robust AI systems, especially superhuman Go agents resilient to adversarial attacks."
- "The goal is to make AI agents minimally exploitable by adversaries, preventing game-losing blunders."
- "Training continues until the victim's win rate plateaus or a set maximum compute budget is reached."
- "Each defender learned effective defenses but did not achieve 100% win rates, indicating partial protection."
- "The final victim remains vulnerable even at high visits, showing the challenge of complete robustness."
- "None of the defenses make attacks impossible but increase the compute needed for successful attacks."
- "Positional adversarial training showed vulnerabilities despite initial defense."
- "Iterated adversarial training resulted in victims largely robust to observed attacks but still vulnerable to new ones."
- "ViT-based Go AI was tested and found exploitable by new attacks despite reaching superhuman levels."
- "Final simulated adversary won 42% of the time against the victim even at 65,536 visits."
- "Defenses made attacks harder but did not provide a complete solution; attacks were still possible with minimal compute."
- "Defenses did not achieve human-level robustness as humans could still execute several attacks."
- "Defenses were vulnerable to new attacks, indicating no robustness to new strategies."
- "The method was bottlenecked by the attack component, requiring more compute than the defense component."

# HABITS:
- Alternately train victim and adversary agents over multiple rounds for robust AI development.
- Continue training until the victim's win rate plateaus or a set maximum compute budget is reached.

# FACTS:
- Iterated adversarial training involves alternately training a victim agent and an adversary agent over multiple rounds.
- Each defender learned effective defenses but did not achieve 100% win rates, indicating partial protection.
- Final simulated adversary won 42% of the time against the victim even at 65,536 visits.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
Achieving complete robustness in AI systems against adversarial attacks remains challenging despite iterative defense strategies.

# RECOMMENDATIONS:
- Develop efficient attack algorithms requiring less compute for future research in AI robustness.
- Improve sample efficiency in adversarial training for more effective defense strategies.