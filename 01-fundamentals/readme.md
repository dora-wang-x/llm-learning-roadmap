# LLM 基础资源索引

## 1. 前置基础：深度学习、NLP 与 Transformer

- <img src="https://img.shields.io/github/stars/Kensuke-Hinata/statistic?style=social" height="17" align="texttop"/> [BERT基础教程：Transformer大模型实战](https://github.com/Kensuke-Hinata/statistic/blob/master/AI/books/BERT%E5%9F%BA%E7%A1%80%E6%95%99%E7%A8%8B%EF%BC%9ATransformer%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%AE%9E%E6%88%98.pdf): 以 BERT 和 Transformer 为主线讲解预训练、微调与下游任务，配合代码和实验说明模型结构，适合 NLP 与大模型入门。
- [Stanford CS224N](https://web.stanford.edu/class/cs224n)：斯坦福 CS224N 系统讲授词向量、序列模型、注意力、Transformer 与现代 NLP，包含作业和项目，适合建立语言理解基础。
- [CMU Advanced NLP](https://cmu-l3.github.io/anlp-spring2025)：CMU Advanced NLP 课程从神经 NLP 基础延伸到检索、生成和大模型前沿，强调研究论文与技术分析，适合有基础的学习者。
- [Transformer models](https://huggingface.co/learn/llm-course/chapter1/1)：Hugging Face 的 LLM 课程介绍 Transformers、Datasets、Tokenizers 和 Hub，配合代码讲解模型使用与微调流程。
- [Transformer 论文精读与深度学习系列](https://space.bilibili.com/1567748478)：李沐深度学习系列以论文精读和代码实践讲解 Transformer、注意力及相关模型，配套动手学深度学习内容，适合中文系统学习。
- <img src="https://img.shields.io/github/stars/google-research/bert?style=social" height="17" align="texttop"/> [bert](https://github.com/google-research/bert): BERT 官方实现包含 MLM、NSP 预训练代码及 GLUE、SQuAD 微调脚本，是理解双向 Transformer 预训练和复现实验的经典参考。
- <img src="https://img.shields.io/github/stars/datawhalechina/learn-nlp-with-transformers?style=social" height="17" align="texttop"/> [learn-nlp-with-transformers](https://github.com/datawhalechina/learn-nlp-with-transformers): Datawhale 中文教程结合 NLP 理论与 Transformers 实战，覆盖文本分类、序列标注和预训练模型使用，适合初学者边学边练。
- <img src="https://img.shields.io/github/stars/huggingface/transformers?style=social" height="17" align="texttop"/> [transformers](https://github.com/huggingface/transformers): Hugging Face Transformers 是主流预训练模型库，提供模型、Tokenizer、训练器和推理接口，支持文本、多模态模型的训练与部署。

## 2. LLM 核心原理与模型架构

- <img src="https://img.shields.io/github/stars/LLMBook-zh/LLMBook-zh.github.io?style=social" height="17" align="texttop"/> [LLMBook-zh.github.io](https://github.com/LLMBook-zh/LLMBook-zh.github.io): 中文《大语言模型》教材，系统讲解语言建模、Transformer、预训练、微调和对齐，适合具备深度学习基础的读者系统阅读。
- [大规模语言模型：从理论到实践](https://intro-llm.github.io)：中文《大规模语言模型：从理论到实践》覆盖语言模型、分布式训练、强化学习和 DeepSpeed-Chat，连接理论学习与系统实现。
- <img src="https://img.shields.io/github/stars/HandsOnLLM/Hands-On-Large-Language-Models?style=social" height="17" align="texttop"/> [Hands-On-Large-Language-Models](https://github.com/HandsOnLLM/Hands-On-Large-Language-Models): 《动手学大语言模型》配套代码库，以图解和 Notebook 讲解模型表示、微调、检索增强和智能体应用。
- <img src="https://img.shields.io/youtube/views/JGtqpQXfJis?style=social" height="17" align="texttop"/> [Introduction to Generative AI 2024‑Spring](https://speech.ee.ntu.edu.tw/~hylee/genai/2024-spring.php): 李宏毅生成式 AI 课程讲解自回归生成、预训练、上下文学习、指令微调、RLHF、幻觉和 Agent 等核心主题，适合全面入门。
- <img src="https://img.shields.io/youtube/views/TigfpYPJk1s?style=social" height="17" align="texttop"/> [Introduction to GenAI and ML 2025 Fall](https://speech.ee.ntu.edu.tw/~hylee/GenAI-ML/2025-fall.php): 李宏毅课程结合机器学习与生成式 AI，覆盖 Tokenizer、Transformer、Mamba、后训练、KV Cache、投机解码和 Agent 推理。
- <img src="https://img.shields.io/youtube/views/JKbtWimlzAE?style=social" height="17" align="texttop"/> [CS25: Transformers United V5 (2025)](https://web.stanford.edu/class/cs25): Stanford CS25 汇集 Transformer 研究者专题报告，聚焦架构、训练、推理和应用前沿，适合跟踪最新研究方向。
- <img src="https://img.shields.io/github/stars/amitshekhariitbhu/llm-internals?style=social" height="17" align="texttop"/> [llm-internals](https://github.com/amitshekhariitbhu/llm-internals): 通过循序渐进的代码和笔记拆解 LLM 内部机制，从分词、Embedding、注意力到推理优化，适合用实验理解模型工作过程。
- <img src="https://img.shields.io/github/stars/walkinglabs/modern-llm-notebook?style=social" height="17" align="texttop"/> [modern-llm-notebook](https://github.com/walkinglabs/modern-llm-notebook): 以 Jupyter Notebook 组织现代 LLM 学习内容，结合代码演示模型结构、训练和应用技术，适合边阅读边运行实验。
- <img src="https://img.shields.io/github/stars/karpathy/nanoGPT?style=social" height="17" align="texttop"/> [nanoGPT](https://github.com/karpathy/nanoGPT): Andrej Karpathy 的极简 GPT 实现，用短小 PyTorch 代码展示数据处理、模型训练和生成流程，适合快速掌握 GPT 核心结构。
- [斯坦福 CS324](https://stanford-cs324.github.io/winter2022)：斯坦福 CS324 课程讨论基础模型的训练数据、规模化、能力、评测和社会影响，适合从研究与系统视角理解 Foundation Models。

## 3. 从零训练与后训练实践

- <img src="https://img.shields.io/github/stars/rasbt/LLMs-from-scratch?style=social" height="17" align="texttop"/> [LLMs-from-scratch](https://github.com/rasbt/LLMs-from-scratch): 从零用 PyTorch 实现 GPT 风格语言模型，覆盖 Tokenizer、注意力、预训练、微调和分类任务，适合深入掌握模型构建细节。
- <img src="https://img.shields.io/github/stars/skindhu/Build-A-Large-Language-Model-CN?style=social" height="17" align="texttop"/> [中文翻译版](https://github.com/skindhu/Build-A-Large-Language-Model-CN): 《从零构建大语言模型》中文翻译与代码资源，跟随原书实现 GPT、训练与微调，适合中文读者动手实践。
- [Stanford CS336](https://cs336.stanford.edu/spring2025)：斯坦福 CS336 从零讲解语言模型数据、Tokenizer、Transformer、训练系统、Scaling 和推理，配合作业实现完整训练链路。
- [Build and Train an LLM with JAX](https://learn.deeplearning.ai/courses/build-and-train-an-llm-with-jax/lesson/gy364z/introduction)：使用 JAX 从零构建并训练约两千万参数语言模型，实践函数式编程、自动微分和向量并行，适合理解现代训练系统基础。
- <img src="https://img.shields.io/github/stars/bbruceyuan/LLMs-Zero-to-Hero?style=social" height="17" align="texttop"/> [LLMs-Zero-to-Hero](https://github.com/bbruceyuan/LLMs-Zero-to-Hero): 从零手写大语言模型核心组件，配合视频和代码解释分词、注意力、训练与推理，适合不满足于调用现成框架的学习者。
- <img src="https://img.shields.io/github/stars/datawhalechina/code-your-own-llm?style=social" height="17" align="texttop"/> [code-your-own-llm](https://github.com/datawhalechina/code-your-own-llm): Datawhale 的全栈 LLM 实践指南，从模型定义、数据和训练到推理部署逐步实现，帮助读者建立端到端工程视角。
- <img src="https://img.shields.io/github/stars/datawhalechina/so-large-lm?style=social" height="17" align="texttop"/> [so-large-lm](https://github.com/datawhalechina/so-large-lm): 结合 Stanford CS324 与李宏毅课程，整理数据、模型、训练、评估、安全和伦理内容，适合作为中文 LLM 全链路学习路线。
- <img src="https://img.shields.io/github/stars/Lordog/dive-into-llms?style=social" height="17" align="texttop"/> [dive-into-llm](https://github.com/Lordog/dive-into-llms): 《动手学大模型》编程实践教程，通过循序渐进的代码讲解模型结构、训练和应用，适合将理论知识转化为可运行实验。
- <img src="https://img.shields.io/github/stars/datawhalechina/self-llm?style=social" height="17" align="texttop"/> [self-llm](https://github.com/datawhalechina/self-llm): 《开源大模型食用指南》面向中文开发者，覆盖国内外开源模型部署、全参数微调、LoRA 和多模态实践。

## 4. LLM 工程与应用开发基础

- <img src="https://img.shields.io/github/stars/PacktPublishing/LLM-Engineers-Handbook?style=social" height="17" align="texttop"/> [LLM-Engineers-Handbook](https://github.com/PacktPublishing/LLM-Engineers-Handbook): 《LLM Engineers Handbook》配套代码覆盖数据处理、微调、评测、部署和 RAG 等工程环节，适合从模型原理过渡到生产应用。
- [Generative AI with Large Language Models](https://www.deeplearning.ai/courses/generative-ai-with-llms)：讲解 Transformer、规模化训练、多 GPU、PEFT/LoRA 与 RLHF，适合系统理解 LLM 的训练与开发流程。
- <img src="https://img.shields.io/github/stars/datawhalechina/llm-cookbook?style=social" height="17" align="texttop"/> [llm-cookbook](https://github.com/datawhalechina/llm-cookbook): Datawhale 中文 LLM Cookbook 汇总模型调用、提示、微调、部署和应用案例，适合开发者快速查阅并复现大模型工程实践。
- <img src="https://img.shields.io/github/stars/liguodongiot/llm-action?style=social" height="17" align="texttop"/> [llm-action](https://github.com/liguodongiot/llm-action): 按技术原理与落地实践整理 LLM 学习内容，覆盖训练、推理、部署和应用开发，适合作为工程化学习与问题排查参考。
- <img src="https://img.shields.io/github/stars/openai/openai-cookbook?style=social" height="17" align="texttop"/> [openai-cookbook](https://github.com/openai/openai-cookbook): OpenAI 官方 Cookbook 提供 API、结构化输出、Embedding、函数调用和评测示例，适合快速搭建并验证 LLM 应用功能。
- <img src="https://img.shields.io/github/stars/datawhalechina/llm-universe?style=social" height="17" align="texttop"/> [llm-universe](https://github.com/datawhalechina/llm-universe): Datawhale《动手学大模型》系列实践教程，围绕开源模型、训练、微调和应用开发组织 notebook 与代码，适合持续动手学习。

## 5. 扩展主题与持续学习资源

- <img src="https://img.shields.io/github/stars/HCPLab-SYSU/Book-of-MLM?style=social" height="17" align="texttop"/> [Book-of-MLM](https://github.com/HCPLab-SYSU/Book-of-MLM): 多模态语言模型教材与配套资源，介绍视觉语言模型、跨模态对齐、基础模型和典型应用，适合作为 LLM 基础后的扩展阅读。
- <img src="https://img.shields.io/github/stars/bojieli/ai-agent-book?style=social" height="17" align="texttop"/> [深入理解 AI Agent：设计原理与工程实践](https://github.com/bojieli/ai-agent-book): 开源《深入理解 AI Agent》教材，讲解智能体设计原理、规划、记忆、工具调用和工程实现，适合从 LLM 过渡到 Agent 系统。
- <img src="https://img.shields.io/github/stars/wikit-ai/awesome-llm-courses?style=social" height="17" align="texttop"/> [awesome-llm-courses](https://github.com/wikit-ai/awesome-llm-courses): 精选 LLM 在线课程与学习资料索引，覆盖基础理论、训练、应用和前沿方向，适合按主题寻找系统课程和公开视频。
- [generative-ai-for-everyone](https://www.deeplearning.ai/courses/generative-ai-for-everyone)：吴恩达面向零基础学习者的生成式 AI 通识课程，介绍模型能力、应用场景、风险与使用方法，不要求深度学习先验。
- <img src="https://img.shields.io/github/stars/mlabonne/llm-course?style=social" height="17" align="texttop"/> [llm-course](https://github.com/mlabonne/llm-course): 以路线图、笔记和 Colab 实验组织 LLM 学习，从基础概念延伸到微调、量化、部署和应用，适合按阶段自学。
- <img src="https://img.shields.io/github/stars/microsoft/generative-ai-for-beginners?style=social" height="17" align="texttop"/> [generative-ai-for-beginners](https://github.com/microsoft/generative-ai-for-beginners): Microsoft 的生成式 AI 入门课程，通过渐进式示例讲解提示、模型 API、应用开发和安全实践，适合初学者建立动手能力。
- <img src="https://img.shields.io/github/stars/steven2358/awesome-generative-ai?style=social" height="17" align="texttop"/> [awesome-generative-ai](https://github.com/steven2358/awesome-generative-ai): 生成式 AI 项目与应用资源清单，覆盖文本、图像、音频、视频和开发工具，适合发现生态项目与进一步学习入口。
- <img src="https://img.shields.io/github/stars/fengdu78/deeplearning_ai_books?style=social" height="17" align="texttop"/> [deeplearning_ai_books](https://github.com/fengdu78/deeplearning_ai_books): 整理 DeepLearning.AI 课程的中文笔记、翻译和配套资料，覆盖深度学习、机器学习与生成式 AI，适合中文读者辅助学习。

