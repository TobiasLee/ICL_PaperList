# Paper List for In-context Learning

<!-- omit in toc -->

## Contents

- [Paper List for In-context Learning](#paper-list-for-in-context-learning)
  - [Contents](#contents)
  - [Introduction](#introduction)
    - [Keywords Convention](#keywords-convention)
  - [Papers](#papers)
    - [Model Warmup for ICL](#model-warmup-for-icl)
    - [Prompt Tuning for ICL](#prompt-tuning-for-icl)
    - [Analysis of ICL](#analysis-of-icl)
      - [Influence Factors for ICL](#influence-factors-for-icl)
      - [Working Mechanism of ICL](#working-mechanism-of-icl)
    - [Evaluation and Resources](#evaluation-and-resources)
    - [Application](#application)
    - [Problems](#problems)
    - [Challenges and Future Directions](#challenges-and-future-directions)
    - [How to contribute?](#how-to-contribute)
  - [Citations](#citations)

## Introduction

This is a paper list (working in progress) about **In-context learning**, for the following paper:

> [**A Survey for In-context Learning**](https://arxiv.org/abs/2301.00234),
> Qingxiu Dong, Lei Li, Damai Dai, Ce Zheng, Zhiyong Wu, Baobao Chang, Xu Sun, Jingjing Xu, Lei Li, Zhifang Sui
> *arXiv preprint ([arXiv 2301.00234](https://arxiv.org/abs/2301.00234))*

### Keywords Convention

![](https://img.shields.io/badge/MetaICL-DCE7F1) abbreviation

![](https://img.shields.io/badge/Analysis-EAD8D9) section in our survey

![](https://img.shields.io/badge/MetaTraining-D8D0E1) main feature

![](https://img.shields.io/badge/ACL2022CL2022-FAEFCA) conference

## Papers

### Model Warmup for ICL

This section contains the pilot works that might contributes to the warmup strategies of ICL.

1. **MetaICL: Learning to Learn In Context NAACL 2022 a pretrained language model is tuned to do in-context learning on a large set of training tasks**. ![](https://img.shields.io/badge/MetaICL-DCE7F1)

   *Sewon Min, Mike Lewis, Luke Zettlemoyer, Hannaneh Hajishirzi*.  [[pdf](https://arxiv.org/abs/2110.15943)], [[project](https://github.com/facebookresearch/metaicl)], 2021.10, ![](https://img.shields.io/badge/NAACL2022-FAEFCA)
   ![](https://img.shields.io/badge/Warmup-EAD8D9) ![](https://img.shields.io/badge/MetaTraining-D8D0E1)
2. **Improving In-Context Few-Shot Learning via Self-Supervised Training**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Mingda Chen, Jingfei Du, Ramakanth Pasunuru, Todor Mihaylov, Srini Iyer, Veselin Stoyanov, Zornitsa Kozareva*.  [[pdf](https://aclanthology.org/2022.naacl-main.260.pdf)], [[project]()], 2022.5, ![](https://img.shields.io/badge/NAACL2022-FAEFCA)
   ![](https://img.shields.io/badge/Warmup-EAD8D9) ![](https://img.shields.io/badge/Self_Supervised_Training-D8D0E1)
3. **Calibrate Before Use: Improving Few-shot Performance of Language Models**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Zihao Zhao, Eric Wallace, Shi Feng, Dan Klein, Sameer Singh*.  [[pdf](http://proceedings.mlr.press/v139/zhao21c.html)], [[project](https://github.com/tonyzhaozh/fewshot_learning)], 2021.2, ![](https://img.shields.io/badge/ICML2021-FAEFCA)
   ![](https://img.shields.io/badge/Warmup-EAD8D9) ![](https://img.shields.io/badge/additional_calibration_parameters-D8D0E1)

   - Using N/A string to calibrate LMs away from common token bias

### Prompt Tuning for ICL

This section contains the pilot works that might contributes to the prompt selection and prompt formulation strategies of ICL.

1. **On the Effect of Pretraining Corpora on In-context Learning by a Large-scale Language Model**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Seongjin Shin, Sang-Woo Lee, Hwijeen Ahn, Sungdong Kim, HyoungSeok Kim, Boseop Kim, Kyunghyun Cho, Gichang Lee, Woomyoung Park, Jung-Woo Ha, Nako Sung*.  [[pdf](https://arxiv.org/abs/2204.13509)], [[project](link)], 2022.04, ![](https://img.shields.io/badge/NAACL2022-FAEFCA)
   ![](https://img.shields.io/badge/section-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)

   - how in-context learning performance changes as the training corpus varies, investigate the effects of the source and size of the pretraining corpus on in-context learning
2. **Chain of Thought Prompting Elicits Reasoning in Large Language Models**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Jason Wei, Xuezhi Wang, Dale Schuurmans, Maarten Bosma, Brian Ichter, Fei Xia, Ed Chi, Quoc Le, Denny Zhou*.  [[pdf](https://arxiv.org/abs/2201.11903)], [[project](link)], 2022.01, ![](https://img.shields.io/badge/conference-FAEFCA)
   ![](https://img.shields.io/badge/section-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
3. **Least-to-Most Prompting Enables Complex Reasoning in Large Language Models**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Denny Zhou, Nathanael Schärli, Le Hou, Jason Wei, Nathan Scales, Xuezhi Wang, Dale Schuurmans, Claire Cui, Olivier Bousquet, Quoc Le, Ed Chi*.  [[pdf](https://arxiv.org/abs/2205.10625)], [[project](link)], 2022.05, ![](https://img.shields.io/badge/conference-FAEFCA)
   ![](https://img.shields.io/badge/section-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
4. **Self-Generated In-Context Learning: Leveraging Auto-regressive Language Models as a Demonstration Generator**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Hyuhng Joon Kim, Hyunsoo Cho, Junyeob Kim, Taeuk Kim, Kang Min Yoo, Sang-goo Lee*.  [[pdf](https://arxiv.org/abs/2206.08082)], [[project](link)], 2022.06, ![](https://img.shields.io/badge/NAACL_2022_Workshop-FAEFCA)
   ![](https://img.shields.io/badge/section-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
5. **Iteratively Prompt Pre-trained Language Models for Chain of Thought**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Boshi Wang, Xiang Deng, Huan Sun*.  [[pdf](https://arxiv.org/abs/2203.08383)], [[project](https://github.com/sunlab-osu/iterprompt)], 2022.03, ![](https://img.shields.io/badge/EMNLP2022-FAEFCA)
   ![](https://img.shields.io/badge/section-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
6. **Automatic Chain of Thought Prompting in Large Language Models**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Zhuosheng Zhang, Aston Zhang, Mu Li, Alex Smola*.  [[pdf](https://arxiv.org/abs/2210.03493)], [[project](https://github.com/amazon-research/auto-cot)], 2022.10, ![](https://img.shields.io/badge/conference-FAEFCA)
   ![](https://img.shields.io/badge/section-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
7. **Learning To Retrieve Prompts for In-Context Learning NAACL 2022 Learn an example retriever via contrastive learning**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Ohad Rubin, Jonathan Herzig, Jonathan Berant*.  [[pdf](https://arxiv.org/abs/2112.08633)], [[project](https://github.com/ohadrubin/epr)], 2022.12, ![](https://img.shields.io/badge/conference-FAEFCA)
   ![](https://img.shields.io/badge/section-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
8. **Finetuned Language Models Are Zero-Shot Learners instruction tuning**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Jason Wei, Maarten Bosma, Vincent Y. Zhao, Kelvin Guu, Adams Wei Yu, Brian Lester, Nan Du, Andrew M. Dai, Quoc V. Le*.  [[pdf](https://arxiv.org/abs/2109.01652)], [[project](https://github.com/google-research/flan)], 2021.09, ![](https://img.shields.io/badge/conference-FAEFCA)
   ![](https://img.shields.io/badge/section-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)

   - finetuning language models on a collection of tasks described via instructions
   - substantially improves zero-shot performance on unseen tasks
9. **Active Example Selection for In-Context Learning**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Yiming Zhang, Shi Feng, Chenhao Tan*.  [[pdf](https://arxiv.org/abs/2211.04486)], [[project](https://github.com/chicagohai/active-example-selection)], 2022.11, ![](https://img.shields.io/badge/conference-FAEFCA)
   ![](https://img.shields.io/badge/section-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
10. **Prompting GPT-3 To Be Reliable establish simple and effective prompts to demonstrate GPT-3's reliability in these four aspects**![](https://img.shields.io/badge/New-EAD8D9)
11. **An lnformation-theoretic Approach to Prompt Engineering Without Ground Truth Labels** ![](https://img.shields.io/badge/New-EAD8D9)
12. **Self-adaptive In-context Learning** ![](https://img.shields.io/badge/New-EAD8D9)
13. **Demystifying Prompts in Language Models via Perplexity Estimation** ![](https://img.shields.io/badge/New-EAD8D9)
14. **Structured Prompting: Scaling In-Context Learning to 1,000 Examples** ![](https://img.shields.io/badge/New-EAD8D9)
    *Yaru Hao, Yutao Sun, Li Dong, Zhixiong Han, Yuxian Gu, Furu Wei*. [[pdf](https://arxiv.org/abs/2212.06713)], [[project](https://github.com/microsoft/LMOps)], 2022.12.
15. **Fantastically Ordered Prompts and Where to Find Them: Overcoming Few-Shot Prompt Order Sensitivity**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Yao Lu, Max Bartolo, Alastair Moore, Sebastian Riedel, Pontus Stenetorp*.  [[pdf](https://arxiv.org/abs/2104.08786)], [[project](link)], 2021.04, ![](https://img.shields.io/badge/ACL2021-FAEFCA)
    ![](https://img.shields.io/badge/Analysis-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)

16. **On the Relation between Sensitivity and Accuracy in In-context Learning**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Yanda Chen, Chen Zhao, Zhou Yu, Kathleen McKeown, He He*.  [[pdf](https://arxiv.org/abs/2209.07661)], [[project](link)], 2022.09, ![](https://img.shields.io/badge/conference-FAEFCA)
    ![](https://img.shields.io/badge/Analysis-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)

17. **Can language models learn from explanations in context?**. ![](https://img.shields.io/badge/New-EAD8D9) ![](https://img.shields.io/badge/explanations-DCE7F1)

   *Andrew K. Lampinen, Ishita Dasgupta, Stephanie C. Y. Chan, Kory Matthewson, Michael Henry Tessler, Antonia Creswell, James L. McClelland, Jane X. Wang, Felix Hill*.  [[pdf](link)], [[project](link)], 2022.04 ![](https://img.shields.io/badge/ArXiv-FAEFCA)
    ![](https://img.shields.io/badge/None-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)

18. **Prototypical Calibration for Few-shot Learning of Language Models** ![](https://img.shields.io/badge/New-EAD8D9)
    *Zhixiong Han, Yaru Hao, Li Dong, Furu Wei*. [[pdf](https://arxiv.org/abs/2205.10183)], [[project](https://github.com/microsoft/LMOps)], 2022.05.

### Analysis of ICL

This section contains the pilot works that might contributes to the influence factors and working mechanism analysis of ICL.

#### Influence Factors for ICL

1. **Rethinking the Role of Demonstrations: What Makes In-Context Learning Work?** ![img](https://img.shields.io/badge/rethinking-DCE7F1)

   *Sewon Min, Xinxi Lyu, Ari Holtzman, Mikel Artetxe, Mike Lewis, Hannaneh Hajishirzi, Luke Zettlemoyer*.  [[pdf](https://arxiv.org/abs/2202.12837)], [[project](https://github.com/alrope123/rethinking-demonstrations)], 2022.03, ![img](https://img.shields.io/badge/ArXiv-FAEFCA)
   ![img](https://img.shields.io/badge/Analysis-EAD8D9) ![img](https://img.shields.io/badge/feature-D8D0E1)
2. **What Makes Good In-Context Examples for GPT-3?** ![img](https://img.shields.io/badge/similarity-DCE7F1)

   *Jiachang Liu, Dinghan Shen, Yizhe Zhang, Bill Dolan, Lawrence Carin, Weizhu Chen*.  [[pdf](https://arxiv.org/abs/2101.06804)], [[project](link)], 2022.08, ![img](https://img.shields.io/badge/DeeLIO@ACL-FAEFCA)
   ![img](https://img.shields.io/badge/Analysis-EAD8D9) ![img](https://img.shields.io/badge/feature-D8D0E1)
3. **Emergent Abilities of Large Language Models** ![](https://img.shields.io/badge/emergent-DCE7F1)

   *Jason Wei, Yi Tay, Rishi Bommasani, Colin Raffel, Barret Zoph, Sebastian Borgeaud, Dani Yogatama, Maarten Bosma, Denny Zhou, Donald Metzler, Ed H. Chi, Tatsunori Hashimoto, Oriol Vinyals, Percy Liang, Jeff Dean, William Fedus*.  [[pdf](https://arxiv.org/abs/2206.07682)], [[project](link)], 2022.07, ![](https://img.shields.io/badge/TMLR2022-FAEFCA)
   ![](https://img.shields.io/badge/Analysis-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
4. **Ground-Truth Labels Matter: A Deeper Look into Input-Label Demonstrations** ![](https://img.shields.io/badge/ground_truth-DCE7F1)

   *Junyeob Kim, Hyuhng Joon Kim, Hyunsoo Cho, Hwiyeol Jo, Sang-Woo Lee, Sang-goo Lee, Kang Min Yoo, Taeuk Kim*.  [[pdf](https://arxiv.org/abs/2205.12685)], [[project](link)], 2022.05, ![](https://img.shields.io/badge/EMNLP2022-FAEFCA)
   ![](https://img.shields.io/badge/Analysis-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
5. **On the Effect of Pretraining Corpora on In-context Learning by a Large-scale Language Model** ![](https://img.shields.io/badge/corpus-DCE7F1)

   *Seongjin Shin, Sang-Woo Lee, Hwijeen Ahn, Sungdong Kim, HyoungSeok Kim, Boseop Kim, Kyunghyun Cho, Gichang Lee, Woo-Myoung Park, Jung-Woo Ha, Nako Sung*.  [[pdf](https://arxiv.org/abs/2204.13509)], [[project](link)], 2022.08, ![](https://img.shields.io/badge/NAACL2022-FAEFCA)
   ![](https://img.shields.io/badge/Analysis-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
6. **Rethinking the Role of Scale for In-Context Learning: An Interpretability-based Case Study at 66 Billion Scale** ![](https://img.shields.io/badge/rethinking-DCE7F1)

   *Hritik Bansal, Karthik Gopalakrishnan, Saket Dingliwal, Sravan Bodapati, Katrin Kirchhoff, Dan Roth*.  [[pdf](https://arxiv.org/abs/2212.09095)], [[project](https://github.com/amazon-science/llm-interpret)], 2022.12, ![](https://img.shields.io/badge/arxiv-FAEFCA)
   ![](https://img.shields.io/badge/New-EAD8D9) ![](https://img.shields.io/badge/rethinking_scale-D8D0E1)
7. **Data Distributional Properties Drive Emergent In-Context Learning in Transformers** ![](https://img.shields.io/badge/corpus-DCE7F1)

   *Stephanie C.Y. Chan, Adam Santoro, Andrew K. Lampinen, Jane X. Wang, Aaditya Singh, Pierre H. Richemond, Jay McClelland, Felix Hill*.  [[pdf](https://arxiv.org/pdf/2205.05055.pdf)], [[project](https://github.com/deepmind/emergent_in_context_learning)], 2022.05, ![](https://img.shields.io/badge/NeurIPS2022-FAEFCA)

#### Working Mechanism of ICL

1. **An Explanation of In-context Learning as Implicit Bayesian Inference** ![](https://img.shields.io/badge/bayesian-DCE7F1)

   *Sang Michael Xie, Aditi Raghunathan, Percy Liang, Tengyu Ma*.  [[pdf](link)], [[project](link)], 2022.08, ![](https://img.shields.io/badge/ICLR-FAEFCA)
   ![](https://img.shields.io/badge/Analysis-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
2. **In-context Learning and Induction Heads** ![](https://img.shields.io/badge/induction_head-DCE7F1)

   *Catherine Olsson, Nelson Elhage, Neel Nanda, Nicholas Joseph, Nova DasSarma, Tom Henighan, Ben Mann, Amanda Askell, Yuntao Bai, Anna Chen, Tom Conerly, Dawn Drain, Deep Ganguli, Zac Hatfield-Dodds, Danny Hernandez, Scott Johnston, Andy Jones, Jackson Kernion, Liane Lovitt, Kamal Ndousse, Dario Amodei, Tom Brown, Jack Clark, Jared Kaplan, Sam McCandlish, Chris Olah*.  [[pdf](link)], [[project](link)], 2022.10, ![](https://img.shields.io/badge/ArXiv-FAEFCA)
   ![](https://img.shields.io/badge/Analysis-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
3. **What Can Transformers Learn In-Context? A Case Study of Simple Function Classes** ![](https://img.shields.io/badge/case_study-DCE7F1)

   *Shivam Garg, Dimitris Tsipras, Percy Liang, Gregory Valiant*.  [[pdf](link)], [[project](link)], 2022.08, ![](https://img.shields.io/badge/ArXiv-FAEFCA)
   ![](https://img.shields.io/badge/Analysis-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
4. **"Data Distributional Properties Drive Emergent In-Context Learning in Transformers"** ![](https://img.shields.io/badge/data_distributional-DCE7F1)

   *Stephanie C. Y. Chan, Adam Santoro, Andrew K. Lampinen, Jane X. Wang, Aaditya Singh, Pierre H. Richemond, Jay McClelland, Felix Hill*.  [[pdf](link)], [[project](link)], 2022.05, ![](https://img.shields.io/badge/ArXiv-FAEFCA)
   ![](https://img.shields.io/badge/Analysis-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
5. **What learning algorithm is in-context learning? Investigations with linear models** ![](https://img.shields.io/badge/learning_algorithm-DCE7F1)

   *Ekin Akyürek, Dale Schuurmans, Jacob Andreas, Tengyu Ma, Denny Zhou*.  [[pdf](link)], [[project](link)], 2022.11, ![](https://img.shields.io/badge/ArXiv-FAEFCA)
   ![](https://img.shields.io/badge/Analysis-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
6. **Transformers learn in-context by gradient descent** ![](https://img.shields.io/badge/gd-DCE7F1)

   *von Oswald, Johannes, Eyvind Niklasson, Ettore Randazzo, João Sacramento, Alexander Mordvintsev, Andrey Zhmoginov, Max Vladymyrov*.  [[pdf](link)], [[project](link)], 2022.12, ![](https://img.shields.io/badge/ArXiv-FAEFCA)
   ![](https://img.shields.io/badge/Analysis-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)

7. **Why Can GPT Learn In-Context? Language Models Secretly Perform Gradient Descent as Meta-Optimizers** ![](https://img.shields.io/badge/meta_optimizer-DCE7F1)

   *Damai Dai, Yutao Sun, Li Dong, Yaru Hao, Zhifang Sui, Furu Wei*.  [[pdf](https://arxiv.org/abs/2212.10559)], [[project](https://github.com/microsoft/LMOps)], 2022.12 ![](https://img.shields.io/badge/ArXiv-FAEFCA)
   ![](https://img.shields.io/badge/Analysis-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)

<!-- 10. **Can Large Language Models Truly Understand Prompts? A Case Study with Negated Prompts**. ![](https://img.shields.io/badge/New-EAD8D9) ![](https://img.shields.io/badge/negated-DCE7F1)
   
   *Joel Jang, Seonghyeon Ye, Minjoon Seo*.  [[pdf](link)], [[project](link)], 2022.10, ![](https://img.shields.io/badge/ArXiv-FAEFCA) 
![](https://img.shields.io/badge/None-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
 -->

<!-- 11.**Does GPT-3 Generate Empathetic Dialogues? A Novel In-Context Example Selection Method and Automatic Evaluation Metric for Empathetic Dialogue Generation**. ![](https://img.shields.io/badge/New-EAD8D9) ![](https://img.shields.io/badge/empathetic-DCE7F1)
   
   *Young-Jun Lee, Chae-Gyun Lim, Ho-Jin Choi*.  [[pdf](link)], [[project](link)], 2022.10, ![](https://img.shields.io/badge/COLING-FAEFCA) 
![](https://img.shields.io/badge/None-EAD8D9) ![](https://img.shields.io/badge/feature-D8D0E1)
 -->

### Evaluation and Resources

This section contains the pilot works that might contributes to the evaluation or resources of ICL.

1. **Beyond the Imitation Game: Quantifying and extrapolating the capabilities of language models**. ![](https://img.shields.io/badge/BigBench-DCE7F1)

   *Aarohi Srivastava, Abhinav Rastogi, Abhishek Rao, Abu Awal Md Shoeb, Abubakar Abid, Adam Fisch, Adam R. Brown, Adam Santoro, Aditya Gupta, Adrià Garriga-Alonso, Agnieszka Kluska, Aitor Lewkowycz, Akshat Agarwal, Alethea Power, Alex Ray, Alex Warstadt et. al.*.  [[pdf](https://arxiv.org/abs/2206.04615)], [[project](https://github.com/google/BIG-bench)], 2022.06, ![](https://img.shields.io/badge/conference-FAEFCA)
   ![](https://img.shields.io/badge/evaluation-EAD8D9) ![](https://img.shields.io/badge/large_scale-D8D0E1)
2. **SUPER-NATURALINSTRUCTIONS: Generalization via Declarative Instructions on 1600+ NLP Task**. ![](https://img.shields.io/badge/natural_instructions-DCE7F1)

   *Yizhong Wang, Swaroop Mishra, Pegah Alipoormolabashi, Yeganeh Kordi, Amirreza Mirzaei, Anjana Arunkumar, Arjun Ashok, Arut Selvan Dhanasekaran, Atharva Naik, David Stap, Eshaan Pathak, Giannis Karamanolakis, Haizhi Gary Lai, Ishan Purohit et. al.*.  [[pdf](https://arxiv.org/abs/2204.07705)], [[project](https://github.com/allenai/natural-instructions)], 2022.04, ![](https://img.shields.io/badge/EMNLP2022-FAEFCA)
   ![](https://img.shields.io/badge/None-EAD8D9) ![](https://img.shields.io/badge/instruction_tuning-D8D0E1)
3. **Language Models are Multilingual Chain-of-Thought Reasoners**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Freda Shi, Mirac Suzgun, Markus Freitag, Xuezhi Wang, Suraj Srivats, Soroush Vosoughi, Hyung Won Chung, Yi Tay, Sebastian Ruder, Denny Zhou, Dipanjan Das, Jason Wei*.  [[pdf](https://arxiv.org/abs/2210.03057)], [[project](link)], 2022.10, ![](https://img.shields.io/badge/conference-FAEFCA)
   ![](https://img.shields.io/badge/evaluation-EAD8D9) ![](https://img.shields.io/badge/multilingual-D8D0E1)

   - evaluate the reasoning abilities of large language models in multilingual settings, introduce the Multilingual Grade School Math (MGSM) benchmark, by manually translating 250 grade-school math problems from the GSM8K dataset into ten typologically diverse languages.
4. **Instruction Induction: From Few Examples to Natural Language Task Descriptions**. ![](https://img.shields.io/badge/Instruction_Induction-DCE7F1)

   *Or Honovich, Uri Shaham, Samuel R. Bowman, Omer Levy*.  [[pdf](https://arxiv.org/abs/2205.10782)], [[project](https://github.com/orhonovich/instruction-induction)], 2022.05, ![](https://img.shields.io/badge/conference-FAEFCA)
   ![](https://img.shields.io/badge/evaluation-EAD8D9) ![](https://img.shields.io/badge/learn_task_instructions-D8D0E1)

   - how to learn task instructions from input output demonstrations
5. **Language Models Are Greedy Reasoners: A Systematic Formal Analysis of Chain-of-Thought**2022.10.3  ![](https://img.shields.io/badge/New-EAD8D9)
6. **What is Not in the Context? Evaluation of Few-shot Learners with Informative Demonstrations** 2212.01692.pdf (arxiv.org)  ![](https://img.shields.io/badge/New-EAD8D9)

### Application

This section contains the pilot works that expands the application of ICL.

1. **Meta-learning via Language Model In-context Tuning**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Yanda Chen, Ruiqi Zhong, Sheng Zha, George Karypis, He He*.  [[pdf](https://arxiv.org/abs/2110.07814)], [[project](https://github.com/yandachen/in-context-tuning)], 2021.10, ![](https://img.shields.io/badge/ACL2022-FAEFCA)
   ![](https://img.shields.io/badge/application-EAD8D9) ![](https://img.shields.io/badge/Meta-learning-D8D0E1)
2. **Does GPT-3 Generate Empathetic Dialogues? A Novel In-Context Example Selection Method and Automatic Evaluation Metric for Empathetic Dialogue Generation**. ![](https://img.shields.io/badge/Abbre-DCE7F1)

   *Young-Jun Lee, Chae-Gyun Lim, Ho-Jin Choi*.  [[pdf](https://aclanthology.org/2022.coling-1.56/)], [[project](link)], 2022.10, ![](https://img.shields.io/badge/COLING2022-FAEFCA)
   ![](https://img.shields.io/badge/application-EAD8D9) ![](https://img.shields.io/badge/dialogue_generation-D8D0E1)
3. **In-context Learning Distillation: Transferring Few-shot Learning Ability of Pre-trained Language Models**. ![](https://img.shields.io/badge/ICL_Distillation-DCE7F1)

   *Yukun Huang, Yanda Chen, Zhou Yu, Kathleen McKeown*.  [pdf](https://arxiv.org/abs/2212.10670), [[project](link)], 2022.12, ![](https://img.shields.io/badge/conference-FAEFCA)
   ![](https://img.shields.io/badge/challenge-EAD8D9) ![](https://img.shields.io/badge/distillation-D8D0E1)
4. **In-context Learning Distillation: Transferring Few-shot Learning Ability of Pre-trained Language Models** ![](https://img.shields.io/badge/New-EAD8D9)
5. **Interleaving Retrieval with Chain-of-Thought Reasoning for Knowledge-Intensive Multi-Step Questions**![](https://img.shields.io/badge/New-EAD8D9)

### Problems

This section contains the pilot works that points out the problems of ICL.

1. **The Inductive Bias of In-Context Learning: Rethinking Pretraining Example Design** ![](https://img.shields.io/badge/New-EAD8D9). ![](https://img.shields.io/badge/knn_Pretraining-DCE7F1)

   *Yoav Levine, Noam Wies, Daniel Jannai, Dan Navon, Yedid Hoshen, Amnon Shashua*.  [[pdf](https://arxiv.org/abs/2110.04541)], [[project](link)], 2021.10, ![](https://img.shields.io/badge/ICLR2022-FAEFCA)
   ![](https://img.shields.io/badge/problem-EAD8D9) ![](https://img.shields.io/badge/knn_Pretraining-D8D0E1)

### Challenges and Future Directions

This section contains the pilot works that might contributes to the challenges and future directions of ICL.

### How to contribute?

- Add new papers to the corresponding part and mark with ![](https://img.shields.io/badge/New-EAD8D9) if the paper has not been included in our survey.
- If the ![](https://img.shields.io/badge/New-EAD8D9) paper is included in the survey, please replace the ![](https://img.shields.io/badge/New-EAD8D9) to the specific section. e.g., ![](https://img.shields.io/badge/Analysis-EAD8D9), and add other basic info about this paper, such as authors, conference.
- If you think the paper does not belong in your section, please move it to another section with the ![](https://img.shields.io/badge/New-EAD8D9) tag.

## Citations

Please consider citing our papers in your publications if the project helps your research. BibTeX reference is as follows.

```
@misc{dong2022survey,
      title={A Survey for In-context Learning}, 
      author={Qingxiu Dong and Lei Li and Damai Dai and Ce Zheng and Zhiyong Wu and Baobao Chang and Xu Sun and Jingjing Xu and Lei Li and Zhifang Sui},
      year={2022},
      eprint={2301.00234},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```

<!-- - **Recent todo:** 
  - I will add the paper link, project link, date, conference for all the paper (except the new papers), please renew the ![](https://img.shields.io/badge/Abbre-DCE7F1), ![](https://img.shields.io/badge/section-EAD8D9) and ![](https://img.shields.io/badge/feature-D8D0E1) for each paper belongs to your section.
  - Since there is a section title, why should we renew ![](https://img.shields.io/badge/section-EAD8D9)? This is for you to check and make sure that the paper is already added in your section.
  - As there's no paper for intro, lei please add the basic info for all the ![](https://img.shields.io/badge/New-EAD8D9) papers, but please retain the ![](https://img.shields.io/badge/New-EAD8D9) tag, rather than replace it with the ![](https://img.shields.io/badge/XXXSection-EAD8D9). -->
