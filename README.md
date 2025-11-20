Exploring Language Models: My Journey with Probability Distributions
👋 Hey There!
Welcome to my hands-on exploration of a fundamental concept behind Large Language Models (LLMs): probability distributions for next-word prediction! This project is a direct result of diving deep into how these incredible models "think" about what word comes next. It's been a fascinating journey to see how seemingly simple probabilities can lead to coherent (and sometimes amusing!) text generation.

🌟 Project Overview
In this interactive Colab notebook, I've mimicked a core mechanism of language models: predicting the next word in a given text prompt. My goal was to understand how a language model assigns probabilities to a set of candidate words based on the surrounding context, and then uses these probabilities to sample (randomly choose) the next word.

The main prompt I worked with was: "Jide was hungry so she went looking for..." (and its variation: "Jide was thirsty so she went looking for..."). This lab really opened my eyes to the subtle power of context!

✨ What I Explored & Learned:
Assigning Probabilities: I got hands-on with assigning probability values to different candidate words. It was interesting to manually adjust these likelihoods to reflect what I thought was most appropriate based on the prompt.
Stochastic Nature of Generation: Using Python's random.choices function, I saw how a language model doesn't just pick the most likely word every time, but rather samples from the distribution. Running the cell multiple times often yielded different, yet plausible, continuations.
The Power of Context: This was a huge takeaway! I actively manipulated probability distributions based on changes in the prompt's context (e.g., changing "hungry" to "thirsty"). This clearly demonstrated how an effective language model must be context-aware to generate relevant responses.
📊 Visualizing Context-Awareness
One of the coolest parts of this project was creating a visualization to show the impact of context. I generated a bar chart comparing the probability distributions of candidate words when Jide was 'hungry' versus when she was 'thirsty'. This chart vividly illustrates:

How the probability of 'water' dramatically increased when Jide was 'thirsty'.
How the probabilities for 'food'-related words decreased in the 'thirsty' context.
This visualization truly makes the abstract concept of "context-awareness" tangible and is a highlight of my presentation!

🛠️ Technologies Used
Python: The core programming language.
Google Colaboratory: For an interactive coding environment.
random library: For sampling words based on probabilities.
matplotlib & pandas: For data visualization and manipulation.
🏃‍♀️ How to Run the Notebook
Open in Colab: Click on the "Open in Colab" badge (if this README is part of a Colab notebook, you're already here!).
Run Cells in Order: Execute each code cell sequentially. This will guide you through assigning probabilities, generating words, and finally, creating the comparative visualization.
💡 Future Ideas & Enhancements
This project sparked several ideas for further exploration:

Sequential Word Generation: Extend the model to generate not just one, but a sequence of words, building upon each generated word to form a more complete sentence.
More Complex Contexts: Experiment with prompts that require more nuanced probabilistic adjustments.
Quantitative Evaluation: Explore ways to quantitatively evaluate the "sensibleness" or "coherence" of generated text.
I'm excited about the possibilities and look forward to diving deeper into these concepts!

🙏 Acknowledgments
This lab is adapted from the concepts presented in Eldan and Li's 2023 paper TinyStories: How Small Can Language Models Be and Still Speak Coherent English?. Big thanks to the creators of this educational material for providing such a clear and engaging introduction to language models!
