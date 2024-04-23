
# LLM Public Opition Resources

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 


Public Opinion Polling: a curated list of resources evaluating large language models for public opinion polling.

---

*Here are some other paper lists you might be interested in:*

💡 ![Last Commit](https://img.shields.io/github/last-commit/Neph0s/awesome-llm-role-playing-with-persona.svg)**[Persona Paper 1](https://github.com/Neph0s/awesome-llm-role-playing-with-persona/):** A list of papers related to role-playing/persona papers and resources and the inspiration for this list

💡 ![Last Commit](https://img.shields.io/github/last-commit/Sahandfer/PersonaPaper.svg)**[Persona Paper 2](https://github.com/Sahandfer/PersonaPaper):** A list of papers related to persona-based dialogue systems and personalized response generation.

💡 ![Last Commit](https://img.shields.io/github/last-commit/penguinnnnn/awesome-llm-and-society.svg)**[LLM and Society](https://github.com/penguinnnnn/awesome-llm-and-society):**  Papers on (1) Psychology of LLMs; (2) Biases in LLMs.

💡 ![Last Commit](https://img.shields.io/github/last-commit/zjunlp/LLMAgentPapers.svg)**[LLM Agent Papers](https://github.com/zjunlp/LLMAgentPapers):**  Papers on Large Language Model Agents.

## 🔔 News

- **2024-04-17 We are looking for collaborators interested in research on this topic. Contact us via email: C.Haensch@lmu.de**

## 📜Content

### US-centric papers

#### Electoral data 

Argyle, L.P. et al. (2023) ‘Out of One, Many: Using Language Models to Simulate Human Samples’, Political Analysis, 31(3), pp. 337–351. doi:10.1017/pan.2023.2.

  - One of the most prominent proposals to use LLM for creating synthetic survey responses. Uses the term *silicon sampling*. Models examined include *GPT-3*. Thematic focus on U.S. politics and public opinion. Uses the 2012, 2016, and 2020 waves of the *American National Election Studies (ANES)* and Rothschild et al.’s “Pigeonholing Partisans” data as comparison.
  - Conclusion from the abstract: "We then compare the silicon and human samples to demonstrate that the information contained in GPT-3 goes far beyond surface similarity. It is nuanced, multifaceted, and reflects the complex interplay between ideas, attitudes, and sociocultural context that characterize human attitudes. We suggest that language models with sufficient algorithmic fidelity thus constitute a novel and powerful tool to advance understanding of humans and society across a variety of disciplines."

#### Other attitudinal and value data

Santurkar, S., Durmus, E., Ladhak, F., Lee, C., Liang, P., & Hashimoto, T. (2023). Whose Opinions Do Language Models Reflect?. arXiv preprint arXiv:2303.17548.

  - Focuses on the alignment of distribution between LLM generated text and US-American demographic groups. As part of the paper, they created *OpinionQA*, a dataset for evaluating LM output with those of 60 US demographic groups with a wide range of topics from abortion to automation, based on *Pew Research’s American Trends Panels*. Partly focuses on the comparison between different *base LMs (ada, davinci, davinci, j1-grande and j1-jumbo), and human feedback (HF)-tuned LMs that (text-* and j1-grande-v2-beta)*. Comparison on the level of group distribution, not on person level.
  - Conclusion from the abstract: "Our analysis not only confirms prior observations about the left-leaning tendencies of some human feedback-tuned LMs, but also surfaces groups whose opinions are poorly reflected by current LMs (e.g., 65+ and widowed individuals)." 



### Other countries

#### Germany

von der Heyde, L., Haensch, A.-C., & Wenz, A. (2023). Vox Populi, Vox AI? Using Language Models to Estimate German Public Opinion. SocArXiv, 8je9g, Center for Open Science.

  - Uses data from the 2017 German federal elections and the German Longitudinal election study. Focus on GPT-3.
  - Conclusion from the abstract: "We find that GPT-3 does not predict citizens’ vote choice accurately, exhibiting a bias towards the Green and Left parties, and making better predictions for more “typical” voter subgroups. While the language model is able to capture broad-brush tendencies tied to partisanship, it tends to miss out on the multifaceted factors that sway individual voter choices."
 
### Cross-country comparisons

Durmus, E., Nguyen, K., Liao, T. I., Schiefer, N., Askell, A., Bakhtin, A., Chen, C., Hatfield-Dodds, Z., Hernandez, D., Joseph, N., Lovitt, L., McCandlish, S., Sikder, O., Tamkin, A., Thamkul, J., Kaplan, J., Clark, J., & Ganguli, D. (2024). Towards Measuring the Representation of Subjective Global Opinions in Language Models. arXiv preprint arXiv:2306.16388.

  - Focuses on the alignment of distribution between LLM generated text and survey results from different countries. As part of the paper, they created *GlobalOpinionQA*, a dataset for evaluating LM output World Values Survey (WVS) and Pew Research Center’s Global Attitudes (GAS). Three different set-ups (default, country-specific prompting and language-translated version).
  - Conclusion from the abstract: "By default, LLM responses tend to be more similar to the opinions of certain populations, such as those from the USA, and some European and South American countries, highlighting the potential for biases. When we prompt the model to consider a particular country's perspective, responses shift to be more similar to the opinions of the prompted populations, but can reflect harmful cultural stereotypes. When we translate GlobalOpinionQA questions to a target language, the model's responses do not necessarily become the most similar to the opinions of speakers of those languages."

---

## 💡  Contribution

### Contributing to this repo

🤲" **Join us in improving this repository!** Spotted any notable works we might have missed? We welcome your additions. Every contribution counts!   "

