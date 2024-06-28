# SUMMARY
The paper discusses the development of AutoWeb GLM, a deployable webpage browsing agent based on the ChatGLM 3 to 6B model, designed to autonomously accomplish complex real-world missions by navigating and operating on real web browsers like humans.

# IDEAS:
- AutoWeb GLM aims to create a deployable webpage browsing agent based on the ChatGLM 3 to 6B model.
- The agent can autonomously accomplish complex real-world missions by navigating and operating on real web browsers.
- AutoWeb GLM addresses the lack of a unified action space and absence of webpage simplification methods.
- It also tackles the scarcity of high-quality training trajectories for strong LLM-based web agents.
- Efficient data strategies and training methods like supervised and reinforcement learning are leveraged.
- The goal is to optimize webpage comprehension, enhance interactive capacity, and improve webpage navigation precision.
- AutoWeb GLM aims to revolutionize how technology assists in daily tasks and digital interactions.
- It differs from WebGLM by focusing on autonomously accomplishing complex real-world missions.
- WebGLM focuses on retrieval-augmented web-scale question answering.
- AutoWeb GLM enhances interactive capacity and webpage navigation precision by amalgamating components into a singular framework.
- It provides a comprehensive observation and action space for robust web browsing.
- WebGLM lacks the capability for correct inference and self-checking on web tasks.
- AutoWeb GLM introduces rejection sampling fine-tuning for lifelong learning in specific web environments.
- The observation space includes task description, simplified HTML, current location, and past operation records.
- Task description helps the model understand the objective of the task.
- Simplified HTML provides structural and content information about the web page.
- Current location information assists the model in understanding its position on the web page.
- Past operation records offer historical context for generating consistent subsequent operations.
- A unified observation space enables the model to handle complexity and variability in web browsing tasks.
- The action space includes various potential browsing operations such as click, scroll, and type.
- State transition is determined by the current webpage state and the agent's output action.
- The task ends when the agent outputs finish or reaches the maximum number of interactions.
- Challenges in constructing the training data set include task collection, privacy and security, objective annotation, and model limitations.
- A hybrid human-AI data construction method is proposed to address these challenges.
- The training process involves supervised fine-tuning (SFT), reinforcement learning, and rejection sampling fine-tuning (RFT).
- SFT trains the model to comprehend web pages and perform basic operations based on user instructions.
- Reinforcement learning enhances the model's ability to operate the browser and infer tasks accurately.
- Rejection sampling fine-tuning optimizes the model for specific webpage environments in targeted domains.
- The model transitions from SFT to reinforcement learning by first equipping it with basic web browsing capabilities.
- RFT allows the model to learn from its mistakes and enhance its capabilities by focusing on specific domains.
- AutoWeb GLM excels in predicting general user operation patterns and showcases superior performance compared to other baselines.

# INSIGHTS:
- AutoWeb GLM leverages efficient data strategies to optimize webpage comprehension and navigation precision.
- The unified observation space includes task description, simplified HTML, current location, and past operation records.
- The action space includes click, scroll, and type operations for effective web page interaction.
- Challenges in training data set construction include task collection, privacy, security, and objective annotation.
- A hybrid human-AI data construction method addresses challenges in training data set construction.
- Supervised fine-tuning (SFT) trains the model to comprehend web pages and perform basic operations.
- Reinforcement learning enhances the model's ability to operate browsers and infer tasks accurately.
- Rejection sampling fine-tuning (RFT) optimizes the model for specific webpage environments in targeted domains.
- The model transitions from SFT to reinforcement learning by equipping it with basic web browsing capabilities first.
- AutoWeb GLM excels in predicting general user operation patterns and outperforms other baselines.

# QUOTES:
- "AutoWeb GLM aims to create a deployable webpage browsing agent based on the ChatGLM 3 to 6B model."
- "The agent can autonomously accomplish complex real-world missions by navigating and operating on real web browsers."
- "AutoWeb GLM addresses the lack of a unified action space and absence of webpage simplification methods."
- "Efficient data strategies and training methods like supervised and reinforcement learning are leveraged."
- "The goal is to optimize webpage comprehension, enhance interactive capacity, and improve webpage navigation precision."
- "AutoWeb GLM aims to revolutionize how technology assists in daily tasks and digital interactions."
- "It differs from WebGLM by focusing on autonomously accomplishing complex real-world missions."
- "AutoWeb GLM enhances interactive capacity and webpage navigation precision by amalgamating components into a singular framework."
- "It provides a comprehensive observation and action space for robust web browsing."
- "WebGLM lacks the capability for correct inference and self-checking on web tasks."
- "AutoWeb GLM introduces rejection sampling fine-tuning for lifelong learning in specific web environments."
- "The observation space includes task description, simplified HTML, current location, and past operation records."
- "Task description helps the model understand the objective of the task."
- "Simplified HTML provides structural and content information about the web page."
- "Current location information assists the model in understanding its position on the web page."
- "Past operation records offer historical context for generating consistent subsequent operations."
- "A unified observation space enables the model to handle complexity and variability in web browsing tasks."
- "The action space includes various potential browsing operations such as click, scroll, and type."
- "State transition is determined by the current webpage state and the agent's output action."
- "Challenges in constructing the training data set include task collection, privacy and security, objective annotation, and model limitations."

# HABITS:
- Leveraging efficient data strategies for optimizing webpage comprehension and navigation precision.
- Utilizing a unified observation space including task description, simplified HTML, current location, past operation records.
- Incorporating various potential browsing operations such as click, scroll, type into action space.
- Addressing challenges in training data set construction through hybrid human-AI data construction method.
- Training models through supervised fine-tuning (SFT) to comprehend web pages perform basic operations.

# FACTS:
- AutoWeb GLM is based on ChatGLM 3 to 6B model for autonomous webpage browsing tasks.
- It addresses lack of unified action space, absence of webpage simplification methods scarcity of high-quality training trajectories.
- Efficient data strategies training methods like supervised reinforcement learning are leveraged for optimization.
- Unified observation space includes task description, simplified HTML, current location past operation records.

# REFERENCES:
None mentioned.

# ONE-SENTENCE TAKEAWAY
AutoWeb GLM revolutionizes autonomous web browsing by leveraging efficient data strategies for optimized comprehension and navigation.

# RECOMMENDATIONS:
- Leverage efficient data strategies to optimize webpage comprehension navigation precision in autonomous agents.
- Utilize a unified observation space including task description simplified HTML current location past operation records.