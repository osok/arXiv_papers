# SUMMARY
The paper discusses methods to build robust AI systems, focusing on defending superhuman Go agents against adversarial attacks using various defense strategies.

# IDEAS:
- The new method aims to build robust AI systems, especially superhuman Go agents, against adversarial attacks.
- Defense strategies include adversarial training with hand-constructed positions, iterated adversarial training, and using a Vision Transformer (ViT).
- The goal is to make AI agents minimally exploitable by adversaries, preventing game-losing blunders.
- Iterated adversarial training involves alternately training a victim agent and an adversary agent over multiple rounds.
- The victim is trained to be robust against the latest adversary, and vice versa, iteratively.
- Training continues until the victim's win rate plateaus or a set compute budget is reached.
- Each defender learned effective defenses but did not achieve a 100% win rate, indicating partial protection.
- The final victim remains vulnerable even at high visits, showing attacks are harder but not impossible.
- The method provides insights into the challenges of achieving robustness in AI systems.
- Practical benefits include evaluating defenses like adversarial training and using ViT instead of CNN.
- None of the defenses make attacks impossible, highlighting the difficulty of achieving complete robustness.
- The method suggests future research avenues like developing new attack algorithms and improving sample efficiency.
- Validation involved testing three defenses: positional adversarial training, iterated adversarial training, and ViT backbone.
- Positional adversarial training showed vulnerabilities despite initial defense.
- Iterated adversarial training resulted in victims largely robust to observed attacks but still vulnerable to new ones.
- ViT-based Go AI was tested and found exploitable by new attacks despite reaching superhuman level.
- Defenses made attacks harder and increased compute needed but did not achieve complete robustness.
- Final victims were still vulnerable to new adversaries, showing partial protection.
- Limitations include the inability to provide a complete solution against adversarial attacks in Go.
- Attack algorithms could always find successful attacks with minimal compute compared to defense training.
- Defenses did not achieve human-level robustness as humans could still execute several attacks.
- Vulnerability to new attacks indicates defenses did not gain robustness to new strategies.
- The method was bottlenecked by the attack component, requiring more compute than the defense component.

# INSIGHTS:
- Iterated adversarial training alternates between training a victim and an adversary over multiple rounds.
- Defenses make attacks harder but do not achieve complete robustness against adversarial attacks.
- Practical benefits include evaluating defenses like adversarial training and using Vision Transformers (ViT).
- Future research should focus on developing new attack algorithms and improving sample efficiency.
- Positional adversarial training showed vulnerabilities despite initial defense efforts.
- Iterated adversarial training resulted in victims robust to observed attacks but vulnerable to new ones.
- ViT-based Go AI was exploitable by new attacks despite reaching superhuman level performance.
- Final victims remained vulnerable to new adversaries, indicating partial protection only.
- Attack algorithms could always find successful attacks with minimal compute compared to defense training.
- Defenses did not achieve human-level robustness as humans could still execute several attacks.

# QUOTES:
- "The new method aims to build robust AI systems, especially superhuman Go agents, against adversarial attacks."
- "Defense strategies include adversarial training with hand-constructed positions, iterated adversarial training, and using a Vision Transformer (ViT)."
- "The goal is to make AI agents minimally exploitable by adversaries, preventing game-losing blunders."
- "Iterated adversarial training involves alternately training a victim agent and an adversary agent over multiple rounds."
- "Training continues until the victim's win rate plateaus or a set compute budget is reached."
- "Each defender learned effective defenses but did not achieve a 100% win rate, indicating partial protection."
- "The final victim remains vulnerable even at high visits, showing attacks are harder but not impossible."
- "The method provides insights into the challenges of achieving robustness in AI systems."
- "Practical benefits include evaluating defenses like adversarial training and using ViT instead of CNN."
- "None of the defenses make attacks impossible, highlighting the difficulty of achieving complete robustness."
- "The method suggests future research avenues like developing new attack algorithms and improving sample efficiency."
- "Validation involved testing three defenses: positional adversarial training, iterated adversarial training, and ViT backbone."
- "Positional adversarial training showed vulnerabilities despite initial defense."
- "Iterated adversarial training resulted in victims largely robust to observed attacks but still vulnerable to new ones."
- "ViT-based Go AI was tested and found exploitable by new attacks despite reaching superhuman level."
- "Defenses made attacks harder and increased compute needed but did not achieve complete robustness."
- "Final victims were still vulnerable to new adversaries, showing partial protection."
- "Limitations include the inability to provide a complete solution against adversarial attacks in Go."
- "Attack algorithms could always find successful attacks with minimal compute compared to defense training."
- "Defenses did not achieve human-level robustness as humans could still execute several attacks."

# HABITS:
- Alternately train a victim agent and an adversary agent over multiple rounds for robustness.
- Continue training until the victim's win rate plateaus or a set compute budget is reached.
- Evaluate defenses like adversarial training and using Vision Transformers (ViT) for practical benefits.
- Focus on developing new attack algorithms and improving sample efficiency for future research.
- Test positional adversarial training despite initial defense vulnerabilities for better insights.

# FACTS:
- Iterated adversarial training alternates between training a victim and an adversary over multiple rounds.
- Defenses make attacks harder but do not achieve complete robustness against adversarial attacks.
- Practical benefits include evaluating defenses like adversarial training and using Vision Transformers (ViT).
- Future research should focus on developing new attack algorithms and improving sample efficiency.
- Positional adversarial training showed vulnerabilities despite initial defense efforts.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
Iterated adversarial training improves AI robustness against attacks but does not achieve complete invulnerability.

# RECOMMENDATIONS:
- Alternately train a victim agent and an adversary agent over multiple rounds for robustness.
- Continue training until the victim's win rate plateaus or a set compute budget is reached.
- Evaluate defenses like adversarial training and using Vision Transformers (ViT) for practical benefits.
- Focus on developing new attack algorithms and improving sample efficiency for future research.
- Test positional adversarial training despite initial defense vulnerabilities for better insights.