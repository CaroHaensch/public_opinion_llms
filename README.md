
# LLM Public Opinion Resources

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 


Public Opinion Polling: a curated list of papers evaluating large language models for public opinion polling.

---

## 💡  Contribution

### Contributing to this repo

🤲 Come collaborate with us to enhance this repository! Have you encountered any notable works that we might have overlooked? We value your additions. Each contribution makes a difference!  

---

*Here are some other paper lists you might be interested in:*

💡 ![Last Commit](https://img.shields.io/github/last-commit/Sahandfer/PersonaPaper.svg) **[Persona Paper 2](https://github.com/Sahandfer/PersonaPaper):** A list of papers related to persona-based dialogue systems and personalized response generation.

💡 ![Last Commit](https://img.shields.io/github/last-commit/penguinnnnn/awesome-llm-and-society.svg) **[LLM and Society](https://github.com/penguinnnnn/awesome-llm-and-society):**  Papers on (1) Psychology of LLMs; (2) Biases in LLMs.

💡 ![Last Commit](https://img.shields.io/github/last-commit/zjunlp/LLMAgentPapers.svg) **[LLM Agent Papers](https://github.com/zjunlp/LLMAgentPapers):**  Papers on Large Language Model Agents.

## 🔔 News

- **2024-04-17 We are looking for collaborators interested in researching this topic as well as conducting a short review. Contact us via email: C.Haensch@lmu.de**

## 📜Content

### US-centric papers

#### Electoral/political science data 

Argyle, L.P. et al. (2023) ‘Out of One, Many: Using Language Models to Simulate Human Samples’, Political Analysis, 31(3), pp. 337–351. doi:10.1017/pan.2023.2.

  - One of the most prominent proposals to use LLM for creating synthetic survey responses. Uses the term *silicon sampling*. Models examined include *GPT-3*. Thematic focus on U.S. politics and public opinion. Uses the 2012, 2016, and 2020 waves of the *American National Election Studies (ANES)* and Rothschild et al.’s “Pigeonholing Partisans” data as comparison.
  - Conclusion from the abstract: "We then compare the silicon and human samples to demonstrate that the information contained in GPT-3 goes far beyond surface similarity. It is nuanced, multifaceted, and reflects the complex interplay between ideas, attitudes, and sociocultural context that characterize human attitudes. We suggest that language models with sufficient algorithmic fidelity thus constitute a novel and powerful tool to advance understanding of humans and society across a variety of disciplines."

Jiang, H., Beeferman, D., Roy, B., & Roy, D. (2022). CommunityLM: Probing Partisan Worldviews from Language Models. arXiv preprint arXiv:2209.07065.

 - GPT-2  models fine-tuned with Tweets from partisan twitter users, eliciting opinions about public figures and groups surveyed by the American National Election Studies (ANES) 2020 Exploratory Testing Survey.

Sun, S., Lee, E., Nan, D., Zhao, X., Lee, W., Jansen, B. J., & Kim, J. H. (2024). Random Silicon Sampling: Simulating Human Sub-Population Opinion Using a Large Language Model Based on Group-Level Demographic Information. arXiv preprint arXiv:2402.18144.

  - Extension of Argyle et al. Focuses on sampling a subsample instead eliciting responses for the full human sample. Also uses ANES data.

Bisbee, J., Clinton, J., Dorff, C., Kenkel, B., and Larson, J., 2023. Synthetic Replacements for Human Survey Data? The Perils of Large Language Models [online]. Available from: osf.io/preprints/socarxiv/5ecfa.

 - Also references Argyle et al.  Evaluate ChatGPT 3.5 Turbo on the standard feeling thermometer survey question (regarding political parties) used by the ANES.
 -  Conclusion from the abstract: "Responses from prompted “persona” profiles in ChatGPT produce measures of partisan and racial affective polarization that are seven times larger than the average opinion of humans who possess the same attributes as the prompted personas. Furthermore, synthetic data are artificially precise, with a standard deviation that is only 31% of the variation found in actual opinions among comparable humans."

 
Sanders, N. E., Ulinich, A., & Schneier, B. (2023). Demonstrations of the Potential of AI-based Political Issue Polling. arXiv preprint arXiv:2307.04781.

  - Uses questions from the Cooperative Election Study (CES) questionnaire, evalutesOpenAI's GPT-3.5-turbo-0301 model.
  - Conclusion from the abstract: "We find that ChatGPT is effective at anticipating both the mean level and distribution of public opinion on a variety of policy issues such as abortion bans and approval of the US Supreme Court, particularly in their ideological breakdown (correlation typically >85%). However, it is less successful at anticipating demographic-level differences. Moreover, ChatGPT tends to overgeneralize to new policy issues that arose after its training data was collected, such as US support for involvement in the war in Ukraine."

#### Other attitudinal and value data

Santurkar, S., Durmus, E., Ladhak, F., Lee, C., Liang, P., & Hashimoto, T. (2023). Whose Opinions Do Language Models Reflect?. arXiv preprint arXiv:2303.17548.

  - Focuses on the alignment of distribution between LLM generated text and US-American demographic groups. As part of the paper, they created *OpinionQA*, a dataset for evaluating LM output with those of 60 US demographic groups with a wide range of topics from abortion to automation, based on *Pew Research’s American Trends Panels*. Partly focuses on the comparison between different *base LMs (ada, davinci, davinci, j1-grande and j1-jumbo), and human feedback (HF)-tuned LMs that (text-* and j1-grande-v2-beta)*. Comparison on the level of group distribution, not on person level.
  - Conclusion from the abstract: "Our analysis not only confirms prior observations about the left-leaning tendencies of some human feedback-tuned LMs, but also surfaces groups whose opinions are poorly reflected by current LMs (e.g., 65+ and widowed individuals)." 

Kim, J., & Lee, B. (2024). AI-Augmented Surveys: Leveraging Large Language Models and Surveys for Opinion Prediction. arXiv preprint arXiv:2305.09620.

  -  Focuses on retrodiction (i.e., predict year-level missing responses) and unasked opinion prediction (i.e., predict entirely missing responses). Data from the General Social Survey from 1972 to 2021, only binarized questions. Examines various fine-tuned models, e.g. Alpaca-7b.
  -  Conclusion from the abstract: "These remarkable prediction capabilities allow us to fill in missing trends with high confidence and pinpoint when public attitudes changed, such as the rising support for same-sex marriage. On the other hand, our fine-tuned Alpaca-7b models show modest success in unasked opinion prediction (AUC = 0.73, ρ = 0.67)."

Chu, E., et al. (2023). Language Models Trained on Media Diets Can Predict Public Opinion. arXiv. Retrieved from https://doi.org/10.48550/arXiv.2303.16779.

  -  Utilizes BERT models that have been fine-tuned on online news articles, TV transcripts, and radio show transcripts. This enables the synthesis of consumer opinions on public health and consumer confidence regarding media diets.
  -  Conclusion from the abstract: "Through random silicon sampling and using only group-level demographic information, we discovered that language models can generate response distributions that are remarkably similar to the actual U.S. public opinion polls. Moreover, we found that the replicability of language models varies depending on the demographic group and topic of the question, and this can be attributed to inherent societal biases in the models."

Dominguez-Olmedo, R., Hardt, M., & Mendler-Dünner, C. (2024). Questioning the Survey Responses of Large Language Models. arXiv preprint arXiv:2306.07951. 

- Utilized 25 multiple-choice questions from the 2019 American Community Survey, covering a range of topics including basic demographic information, education, healthcare, disability status, employment, and income. Surveyed 39 language models of various sizes.
-  Conclusion from the abstract: "Rather, models across the board trend toward uniformly random aggregate statistics over survey responses. This pattern is robust to various different ways of prompting the model, including what is the de-facto standard. Our findings demonstrate that aggregate statistics of a language model's survey responses lack the signals found in human populations. This absence of statistical signal cautions about the use of survey responses from large language models at present time."

Hwang, E., Majumder, B. P., & Tandon, N. (2023). Aligning Language Models to User Opinions. arXiv preprint arXiv:2305.14929.

  - Uses the OpinionQA dataset from Santurkar, evaluate GPT-3. Tries different sets of included information in prompts (dempraphics, ideology and opinions).
  - Conclusion from the abstract: "We use this insight to align LLMs by modeling both user opinions as well as user demographics and ideology, achieving up to 7 points accuracy gains in predicting public opinions from survey questions across a broad set of topics. In addition to the typical approach of prompting LLMs with demographics and ideology, we discover that utilizing the most relevant past opinions from individual users enables the model to predict user opinions more accurately."

### Other countries

#### Germany

von der Heyde, L., Haensch, A.-C., & Wenz, A. (2023). Vox Populi, Vox AI? Using Language Models to Estimate German Public Opinion. SocArXiv, 8je9g, Center for Open Science.

  - Uses data from the 2017 German federal elections and the German Longitudinal election study. Focus on GPT-3.
  - Conclusion from the abstract: "We find that GPT-3 does not predict citizens’ vote choice accurately, exhibiting a bias towards the Green and Left parties, and making better predictions for more “typical” voter subgroups. While the language model is able to capture broad-brush tendencies tied to partisanship, it tends to miss out on the multifaceted factors that sway individual voter choices."

#### Russia

Kalinin, K. (2023, July 9). Improving GPT Generated Synthetic Samples with Sampling-Permutation Algorithm. SSRN. Retrieved from https://ssrn.com/abstract=4548937 or http://dx.doi.org/10.2139/ssrn.4548937
  - Uses Survey of Russian Elites, which covers the period 1993–2020. Focus on GPT-3. Proposes a methodology for prompting to receice more robust average values.

 
### Cross-country comparisons

Durmus, E., Nguyen, K., Liao, T. I., Schiefer, N., Askell, A., Bakhtin, A., Chen, C., Hatfield-Dodds, Z., Hernandez, D., Joseph, N., Lovitt, L., McCandlish, S., Sikder, O., Tamkin, A., Thamkul, J., Kaplan, J., Clark, J., & Ganguli, D. (2024). Towards Measuring the Representation of Subjective Global Opinions in Language Models. arXiv preprint arXiv:2306.16388.

  - Focuses on the alignment of distribution between LLM generated text and survey results from different countries. As part of the paper, they created *GlobalOpinionQA*, a dataset for evaluating LM output World Values Survey (WVS) and Pew Research Center’s Global Attitudes (GAS). Three different set-ups (default, country-specific prompting and language-translated version). Uses a decoder-only transformer model fine-tuned with Reinforcement Learning from Human Feedback (RLHF) and Constitutional AI (CAI).
  - Conclusion from the abstract: "By default, LLM responses tend to be more similar to the opinions of certain populations, such as those from the USA, and some European and South American countries, highlighting the potential for biases. When we prompt the model to consider a particular country's perspective, responses shift to be more similar to the opinions of the prompted populations, but can reflect harmful cultural stereotypes. When we translate GlobalOpinionQA questions to a target language, the model's responses do not necessarily become the most similar to the opinions of speakers of those languages."


## Frameworks, reviews, etc.

Simmons, G., & Hare, C. (2023). Large Language Models as Subpopulation Representative Models: A Review. arXiv preprint arXiv:2310.17888.

  - Survey of implementations.

Clemmensen, L. H., & Kjærsgaard, R. D. (2023). Data Representativity for Machine Learning and AI Systems. arXiv preprint arXiv:2203.04706.

   -  Framework of questions for creating and documenting data with data representativity in mind + measure recommendations.

Tjuatja, L., Chen, V., Wu, S. T., Talwalkar, A., & Neubig, G. (2024). Do LLMs exhibit human-like response biases? A case study in survey design. arXiv preprint arXiv:2311.04076.

    - Explores sensitivity to prompt wording (different to human biases!). 

---



