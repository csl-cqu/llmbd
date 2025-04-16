## LLMBD:BackdoorDefenseviaLargeLanguage Model ParaphrasingandDataVotingin NLP

### Abstract
With the rapid development of natural language processing (NLP), backdoor attacks have emerged as a significant security threat. These attacks inject malicious triggers into NLP models, causing them to produce adversarial outputs while remaining functional under normal input. To eliminate backdoors, existing data-driven defense methods typically transform backdoored samples into normal samples. However, these defenses lack the scalability to adapt effectively to various backdoor attacks.

To address this challenge, we propose LLMBD, a novel data-driven backdoor defense method that leverages large language models (LLMs) for paraphrasing. Specifically, LLMBD uses large language models with optimized prompts to paraphrase the input text, eliminating potential backdoors while maintaining semantic integrity and textual fluency. During the training and inference phases, we apply grouping and majority voting mechanisms to bypass residual backdoors in the paraphrased dataset.

We validate the robustness and defense effectiveness of LLMBD through comprehensive model evaluations. Experimental results on datasets including SST-2, IMDB, and HSOL under various backdoor attack types (BadNets, AddSent, Synbkd, Stylebkd) show that LLMBD significantly outperforms existing methods such as RAP, STRIP, ParaFuzz, and TextGuard. On the SST-2, HSOL, and IMDB datasets, LLMBD achieves an average ASR drop of 0.278, while maintaining an average CACC of 0.897. LLMBD exhibits superior robustness, generalization, and performance preservation without requiring modifications to the backdoored model, providing an efficient and model-agnostic defense strategy against diverse backdoor threats.
### Framework

![](llmbd.png)

