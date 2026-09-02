# 大模型预训练

## 1. 预训练原理与 Scaling

- [Stanford CS336: Language Modeling from Scratch](https://cs336.stanford.edu/): 斯坦福从零构建语言模型课程，覆盖分词、Transformer、数据处理、训练、评测及推理系统，强调在受控实验中理解预训练全流程。
- [Stanford CS336 2024 课程资料](https://stanford-cs336.github.io/spring2024/): CS336 春季课程网站，保留从零训练语言模型的讲义、作业与项目资料，可用于对照理论推导和端到端工程实现。
- [EleutherAI: Transformer Math](https://blog.eleuther.ai/transformer-math/): 以矩阵运算视角拆解 Transformer 前向与反向传播，解释注意力、归一化和参数规模，为阅读训练代码和排查数值问题打基础。
- [Lilian Weng: How to Train Really Large Models on Many GPUs?](https://lilianweng.github.io/posts/2021-09-25-train-large/): 系统说明数据、张量和流水线并行，以及 ZeRO、检查点等技术的通信与显存取舍，适合作为大规模训练方案的理论导读。
- [Lilian Weng 博客](https://lilianweng.github.io/): 汇集语言模型、对齐、推理和训练系统的长文，适合围绕具体概念建立从论文方法到工程实践的理解。
- [CMU ANLP: Pretraining 讲义](https://cmu-l3.github.io/anlp-spring2025/static_files/anlp-s2025-06-pretraining.pdf): CMU 高级自然语言处理课程的预训练讲义，梳理自监督目标、语料、规模化训练和模型能力的关联。
- [AI-PhD: Pretraining 幻灯片](https://github.com/rphilipzhang/AI-PhD-S25/blob/main/Slides/AI-PhD-S2025-6-Pretraining.pdf): AI-PhD 课程预训练专题幻灯片，概览数据配比、训练目标、规模规律与常见训练决策，便于快速建立整体框架。
- [CUHK: Pretraining 课件](https://mobitec.ie.cuhk.edu.hk/ierg5050Fall2025/static_files/slides/Pretraining.pdf): 香港中文大学课程的预训练课件，介绍语言模型预训练的目标函数、数据构成、训练策略及其对下游能力的影响。
- [EleutherAI: Deep Ignorance](https://blog.eleuther.ai/deep-ignorance/): 从数据、评测和研究方法反思大模型中的未知与偏差，帮助在制定预训练实验时明确结论边界和证据质量。
- [HuggingChat 论文内容页](https://huggingface.co/buckets/huggingchat/papers-content/tree/2501/2501.09223.md): Hugging Face 上以 Markdown 发布的论文内容页，可直接阅读对应研究的摘要、方法和实验细节，并作为追踪近期论文的入口。

## 2. 模型实现与单机实验

- <img src="https://img.shields.io/github/stars/rasbt/LLMs-from-scratch?style=social" height="17" align="texttop"/> [Build a Large Language Model (From Scratch)](https://github.com/rasbt/LLMs-from-scratch): 配套《Build a Large Language Model》逐步实现分词、注意力、GPT 训练和微调，以小规模代码实验贯通预训练模型的核心组件。
- <img src="https://img.shields.io/github/stars/MLNLP-World/LLMs-from-scratch-CN?style=social" height="17" align="texttop"/> [LLMs-from-scratch-CN](https://github.com/MLNLP-World/LLMs-from-scratch-CN): 《从零构建大语言模型》中文翻译与配套资料，帮助中文读者跟随代码理解 GPT 的数据管线、训练循环和生成机制。
- <img src="https://img.shields.io/github/stars/karpathy/nanoGPT?style=social" height="17" align="texttop"/> [nanoGPT](https://github.com/karpathy/nanoGPT): 极简 GPT 训练仓库，提供可读性很高的模型、数据加载和训练脚本，适合在单机或少量 GPU 上复现实验。
- <img src="https://img.shields.io/github/stars/karpathy/llm.c?style=social" height="17" align="texttop"/> [llm.c](https://github.com/karpathy/llm.c): 用 C/CUDA 实现 GPT-2 训练的低层项目，直接展示前向、反向、优化器和 GPU 内核，适合理解框架之下的训练机制。
- <img src="https://img.shields.io/github/stars/jammastergirish/BuildAnLLM?style=social" height="17" align="texttop"/> [BuildAnLLM](https://github.com/jammastergirish/BuildAnLLM): 面向实践者的语言模型构建教程与代码，覆盖 tokenizer、Transformer、数据准备、预训练和推理，可作为从概念到原型的补充路径。
- <img src="https://img.shields.io/github/stars/Lightning-AI/litgpt?style=social" height="17" align="texttop"/> [LitGPT](https://github.com/Lightning-AI/litgpt): 基于 Lightning 生态的高性能 LLM 代码库，提供多模型预训练、微调、量化与部署脚本，兼顾清晰实现和可扩展实验。
- <img src="https://img.shields.io/github/stars/huggingface/course?style=social" height="17" align="texttop"/> [Hugging Face Course](https://github.com/huggingface/course): Hugging Face 官方课程源码，围绕 Transformers、Datasets、Tokenizers 与模型训练组织教程，适合补齐使用生态工具的基础。
- [Hugging Face LLM Course](https://huggingface.co/learn/llm-course): 互动式大语言模型课程，覆盖 Transformer 原理、数据处理、训练与推理实践，并配合 Hugging Face 工具链开展练习。
- [Introduction to Large Language Models](https://intro-llm.github.io/): 面向入门者的 LLM 在线教材，系统介绍模型架构、预训练、对齐、提示和应用，为进入训练主题提供共同基础。

## 3. 大规模分布式训练

- <img src="https://img.shields.io/github/stars/EleutherAI/gpt-neox?style=social" height="17" align="texttop"/> [GPT-NeoX](https://github.com/EleutherAI/gpt-neox): 面向大规模自回归模型训练的分布式框架，集成 DeepSpeed 和并行策略，曾用于训练 EleutherAI 系列开放语言模型。
- <img src="https://img.shields.io/github/stars/nvidia/megatron-lm?style=social" height="17" align="texttop"/> [Megatron-LM](https://github.com/nvidia/megatron-lm): NVIDIA 的大模型训练框架，提供张量、流水线、数据和上下文并行，以及高效 Transformer 实现，面向多 GPU 与多节点训练。
- <img src="https://img.shields.io/github/stars/microsoft/DeepSpeed?style=social" height="17" align="texttop"/> [DeepSpeed](https://github.com/microsoft/DeepSpeed): Microsoft 的深度学习优化库，核心 ZeRO 技术降低显存占用，并提供并行训练、混合精度和大模型推理能力。
- <img src="https://img.shields.io/github/stars/microsoft/DeepSpeedExamples?style=social" height="17" align="texttop"/> [DeepSpeedExamples](https://github.com/microsoft/DeepSpeedExamples): DeepSpeed 官方示例集，包含语言模型训练、ZeRO、MoE、流水线并行等可运行配置，适合从概念过渡到集群实践。
- <img src="https://img.shields.io/github/stars/huggingface/nanotron?style=social" height="17" align="texttop"/> [Nanotron](https://github.com/huggingface/nanotron): Hugging Face 开源的大规模 Transformer 训练框架，提供并行策略、检查点和配置化工作流，侧重可复现的预训练实验。
- [Transformers 文档](https://huggingface.co/docs/transformers/index): Hugging Face Transformers 的官方 API 文档，说明模型、训练器、分词器和集成接口，可用于快速搭建及扩展训练实验。

## 4. 训练效率与工程优化

- <img src="https://img.shields.io/github/stars/kellerjordan/modded-nanogpt?style=social" height="17" align="texttop"/> [modded-nanogpt](https://github.com/kellerjordan/modded-nanogpt): 对 nanoGPT 训练配方进行现代化优化的实验项目，集中展示内核、优化器、批量大小和训练策略对吞吐与效果的影响。
- <img src="https://img.shields.io/github/stars/horseee/Awesome-Efficient-LLM?style=social" height="17" align="texttop"/> [Awesome-Efficient-LLM](https://github.com/horseee/Awesome-Efficient-LLM): 汇集高效大模型训练、推理、压缩和服务化论文与项目，可按显存、计算、通信和延迟问题查找技术路线。
- [UltraScale Playbook](https://huggingface.co/spaces/nanotron/ultrascale-playbook): Hugging Face 的超大规模训练实践手册，讲解并行选择、故障恢复、性能分析和集群运行中的实际决策。
- <img src="https://img.shields.io/github/stars/SylphAI-Inc/LLM-engineer-handbook?style=social" height="17" align="texttop"/> [LLM Engineer Handbook](https://github.com/SylphAI-Inc/LLM-engineer-handbook): 面向 LLM 工程师的实践手册，涵盖数据、训练、评测、部署与监控，可将预训练知识放入完整生产生命周期理解。
- <img src="https://img.shields.io/github/stars/saucam/awesome-llm-prod?style=social" height="17" align="texttop"/> [Awesome LLM Production](https://github.com/saucam/awesome-llm-prod): 收集生产环境中构建、部署和运营 LLM 的工具与文章，适合补充训练完成后模型交付、观测和成本控制知识。
- [Awesome Production Machine Learning](https://ethicalml.github.io/awesome-production-machine-learning/): 面向机器学习生产化的资源导航，覆盖实验管理、数据版本、部署、监控与治理，可迁移到预训练工程体系。

## 5. 语料获取与清洗

- <img src="https://img.shields.io/github/stars/facebookresearch/lingua?style=social" height="17" align="texttop"/> [Lingua](https://github.com/facebookresearch/lingua): Meta 开源的语言数据处理工具，提供语言识别、质量过滤、去重和敏感内容处理，服务于大规模语料构建。
- <img src="https://img.shields.io/github/stars/NVIDIA/NeMo-Curator?style=social" height="17" align="texttop"/> [NeMo Curator](https://github.com/NVIDIA/NeMo-Curator): NVIDIA 的可扩展数据治理框架，支持网页语料清洗、去重、分类、质量过滤及 GPU 加速处理，面向训练数据管线。
- <img src="https://img.shields.io/github/stars/datajuicer/data-juicer?style=social" height="17" align="texttop"/> [data-juicer](https://github.com/datajuicer/data-juicer): 面向基础模型的数据处理系统，集成数据分析、清洗、去重、筛选与增强算子，并支持基于数据反馈迭代优化处理配方，适合搭建和实验预训练语料管线。
- <img src="https://img.shields.io/github/stars/unclecode/crawl4ai?style=social" height="17" align="texttop"/> [Crawl4AI](https://github.com/unclecode/crawl4ai): 为 AI 场景设计的网页抓取与 Markdown 转换工具，可按结构化规则获取内容，为构建领域预训练或继续预训练语料提供入口。
- <img src="https://img.shields.io/github/stars/haolpku/Awesome-LLM-Data-Preparation?style=social" height="17" align="texttop"/> [Awesome LLM Data Preparation](https://github.com/haolpku/Awesome-LLM-Data-Preparation): 集中索引大模型数据获取、清洗、去重、质量评估与配比相关论文、数据集和工具，适合快速定位数据工程方案。
- [Hugging Face Datasets 文档](https://huggingface.co/docs/datasets/index): 官方数据集库文档，说明数据下载、流式读取、映射处理、缓存与共享机制，可作为训练语料管线的通用基础设施。

## 6. 数据质量、检查与标注

- <img src="https://img.shields.io/github/stars/cleanlab/cleanlab?style=social" height="17" align="texttop"/> [Cleanlab](https://github.com/cleanlab/cleanlab): 利用模型预测发现标签错误、异常样本和数据质量问题的开源库，可用于筛选监督数据并量化训练集可信度。
- <img src="https://img.shields.io/github/stars/argilla-io/argilla?style=social" height="17" align="texttop"/> [Argilla](https://github.com/argilla-io/argilla): 开源数据标注与人类反馈平台，支持文本、偏好和评估工作流，可沉淀高质量指令数据并审查模型输出。

## 7. 延伸学习与前沿追踪

### 系统课程与教材

- <img src="https://img.shields.io/github/stars/ZJU-LLMs/Foundations-of-LLMs?style=social" height="17" align="texttop"/> [Foundations of LLMs](https://github.com/ZJU-LLMs/Foundations-of-LLMs): 浙江大学大模型基础课程资料，梳理语言模型发展、Transformer、预训练、对齐与应用，适合系统化复习核心概念。
- <img src="https://img.shields.io/github/stars/mlabonne/llm-course?style=social" height="17" align="texttop"/> [LLM Course](https://github.com/mlabonne/llm-course): 从基础到生产应用的开源 LLM 课程，涵盖数学、Transformer、微调、量化、RAG 与智能体，提供清晰的学习路径。
- <img src="https://img.shields.io/github/stars/datawhalechina/happy-llm?style=social" height="17" align="texttop"/> [Happy-LLM](https://github.com/datawhalechina/happy-llm): Datawhale 中文大模型教程，以 Transformer、预训练、微调和应用为主线，配套代码和通俗讲解，适合作为中文入门资料。
- <img src="https://img.shields.io/github/stars/LLMBook-zh/LLMBook-zh.github.io?style=social" height="17" align="texttop"/> [大语言模型原理与工程实践](https://github.com/LLMBook-zh/LLMBook-zh.github.io): 中文开源书籍项目，覆盖大语言模型理论、训练、推理、对齐与应用实践，可用于建立完整知识地图。
- <img src="https://img.shields.io/github/stars/datawhalechina/so-large-lm?style=social" height="17" align="texttop"/> [So Large LM](https://github.com/datawhalechina/so-large-lm): Datawhale 的大模型学习资料，聚焦预训练、指令微调、部署和应用案例，为中文读者提供结构化导览。
- <img src="https://img.shields.io/github/stars/ZHUANGHP/llm-training?style=social" height="17" align="texttop"/> [LLM Training](https://github.com/ZHUANGHP/llm-training): 面向训练大语言模型的中文资料汇总，覆盖数据、预训练、对齐和分布式训练，适合按专题检索参考实现。
- <img src="https://img.shields.io/github/stars/datawhalechina/llm-universe?style=social" height="17" align="texttop"/> [LLM Universe](https://github.com/datawhalechina/llm-universe): Datawhale 大模型知识库，整理基础概念、技术路线和应用实践，可作为跨预训练、微调与部署主题的导航入口。
- <img src="https://img.shields.io/github/stars/datawhalechina/llm-cookbook?style=social" height="17" align="texttop"/> [LLM Cookbook](https://github.com/datawhalechina/llm-cookbook): 面向开发实践的大模型案例集，包含提示、微调、RAG 和应用搭建示例，适合理解训练成果如何服务业务任务。
- <img src="https://img.shields.io/github/stars/hiyouga/LlamaFactory?style=social" height="17" align="texttop"/> [LlamaFactory](https://github.com/hiyouga/LlamaFactory): 易用的大模型微调框架，支持多种开源模型、监督微调、偏好优化与量化训练，可用于衔接预训练模型和下游对齐实验。
- <img src="https://img.shields.io/github/stars/dirtyA/LLMForEverybody?style=social" height="17" align="texttop"/> [LLM For Everybody](https://github.com/dirtyA/LLMForEverybody): 为大众整理的大模型学习资料，涵盖基础概念、论文、课程、工具与实践路径，可作为初学者的资源索引。
- <img src="https://img.shields.io/github/stars/liguodongiot/llm-action?style=social" height="17" align="texttop"/> [LLM Action](https://github.com/liguodongiot/llm-action): 聚焦大模型实战的中文项目，整理模型原理、训练、微调、应用与工程资料，提供可持续扩展的学习目录。
- <img src="https://img.shields.io/github/stars/microsoft/generative-ai-for-beginners?style=social" height="17" align="texttop"/> [Generative AI for Beginners](https://github.com/microsoft/generative-ai-for-beginners): Microsoft 面向初学者的生成式 AI 课程，按课程单元讲解模型、提示、应用和安全，适合作为进入 LLM 领域的前置学习。
- <img src="https://img.shields.io/github/stars/HandsOnLLM/Hands-On-Large-Language-Models?style=social" height="17" align="texttop"/> [Hands-On Large Language Models](https://github.com/HandsOnLLM/Hands-On-Large-Language-Models): 配套实践书籍的代码库，以嵌入、Transformer、微调、RAG 和代理为主题，通过 Notebook 把理论连接到可运行实验。
- <img src="https://img.shields.io/github/stars/DipanjanSanyal/llm-fundamentals?style=social" height="17" align="texttop"/> [LLM Fundamentals](https://github.com/DipanjanSanyal/llm-fundamentals): 以 Notebook 汇总语言模型的关键基础，包括文本表示、注意力、Transformer 和生成任务，适合补足预训练前的机器学习知识。
- <img src="https://img.shields.io/github/stars/FreedomIntelligence/CSC6203-LLM?style=social" height="17" align="texttop"/> [CSC6203-LLM](https://github.com/FreedomIntelligence/CSC6203-LLM): 大语言模型课程资源库，收录教学大纲、讲义和阅读材料，覆盖预训练、对齐、推理与评估等研究主题。
- [Stanford CS324: Large Language Models](https://stanford-cs324.github.io/winter2023/): 斯坦福大语言模型课程，讨论数据、训练、能力、社会影响和部署，将预训练技术置于更完整的模型生命周期中审视。
- [Stanford CS25: Transformers United](https://web.stanford.edu/class/cs25/): Transformer 专题课程网站，邀请领域研究者讲解架构演进、视觉语言、多模态和大模型实践，适合追踪研究脉络。
- [LLM Class 课程日程](https://llm-class.github.io/schedule.html): 大语言模型课程的授课日程与阅读安排，可按主题找到预训练、对齐、检索、推理和评测相关材料。

### 资源导航

- <img src="https://img.shields.io/github/stars/RUCAIBox/awesome-llm-pretraining?style=social" height="17" align="texttop"/> [Awesome LLM Pretraining](https://github.com/RUCAIBox/awesome-llm-pretraining): 专门整理语言模型预训练的论文、模型、数据集、代码和课程，是扩展本页各工作流类别的高密度导航资源。
- <img src="https://img.shields.io/github/stars/hannibal046/awesome-llm?style=social" height="17" align="texttop"/> [Awesome LLM](https://github.com/hannibal046/awesome-llm): 汇总大语言模型论文、开源项目、数据集、课程和应用，覆盖训练与使用全生命周期，适合进行横向检索。
- <img src="https://img.shields.io/github/stars/adongwanai/Awesome-Awesome-LLMs?style=social" height="17" align="texttop"/> [Awesome Awesome LLMs](https://github.com/adongwanai/Awesome-Awesome-LLMs): 聚合多个大模型资源清单，按模型、数据、工具、应用和社区收录链接，适合发现细分领域的专题导航。
- <img src="https://img.shields.io/github/stars/iflabx/Awesome-LLM-Learning?style=social" height="17" align="texttop"/> [Awesome LLM Learning](https://github.com/iflabx/Awesome-LLM-Learning): 面向学习者整理课程、书籍、论文、代码和中文资料，可结合学习阶段快速补充本页未覆盖的主题。
- <img src="https://img.shields.io/github/stars/eugeneyan/open-llms?style=social" height="17" align="texttop"/> [Open LLMs](https://github.com/eugeneyan/open-llms): 汇总开放权重大模型及其许可、能力和相关资源，便于比较可研究、微调或部署的模型基座。

### 研究与行业动态

- [Hugging Face Blog](https://huggingface.co/blog): Hugging Face 官方博客，发布开源模型、数据集、训练工具和研究解读，常含可复现代码及工程经验。
- [OpenAI Blog](https://openai.com/blog): OpenAI 官方博客，发布模型研究、产品能力与安全实践，可用于追踪前沿模型训练和部署方向。
- [Meta AI Blog](https://ai.meta.com/blog/): Meta AI 官方博客，介绍基础模型、开源研究、数据与系统进展，并提供 Llama 等项目的背景与技术解读。
- [Google DeepMind Blog](https://deepmind.google/blog/): Google DeepMind 官方研究博客，覆盖通用模型、多模态、科学智能和安全研究，适合了解行业前沿问题。
- [Microsoft Research Blog](https://www.microsoft.com/en-us/research/blog/): Microsoft Research 研究博客，发布机器学习、系统和生产化研究成果，可补充训练基础设施与应用视角。
- [Mistral News](https://mistral.ai/news): Mistral AI 官方新闻页，更新模型发布、研究进展和产品动态，可用于关注欧洲开源模型生态。
- [Anthropic Blog](https://www.anthropic.com/blog): Anthropic 官方博客，重点分享模型能力、可靠性、对齐和安全研究，适合观察预训练之后的风险控制方向。
- [NVIDIA Developer Blog](https://developer.nvidia.com/blog/): NVIDIA 开发者博客，发布 GPU、CUDA、训练框架与推理优化实践，适合排查和优化大模型训练性能。
- [NVIDIA Research](https://research.nvidia.com/): NVIDIA Research 研究门户，收录图形、系统、AI 与基础模型论文，便于从硬件与算法协同角度追踪新工作。
- [BAIR Blog](https://bair.berkeley.edu/blog/): Berkeley AI Research 博客，以通俗文章介绍学术研究成果，涵盖语言模型、智能体、评测、可靠性与生成式 AI。
- [Stanford HAI](https://hai.stanford.edu/): 斯坦福以人为本人工智能研究院网站，发布研究、政策和社会影响内容，为训练技术补充治理与公共影响视角。

### 社区与技术文章

- [Hacker News](https://news.ycombinator.com/): 技术社区新闻聚合站，可追踪开源模型发布、训练工具、论文讨论和工程实践的即时反馈。
- [r/LocalLLaMA](https://www.reddit.com/r/LocalLLaMA/): 本地运行与开源大模型社区，集中讨论模型发布、微调、量化、硬件配置和复现经验，信息更新较快。
- [Towards Data Science](https://towardsdatascience.com/): 数据科学技术社区，包含机器学习与大模型教程、案例和观点文章，适合从实践角度补充概念理解。
- [掘金](https://juejin.cn/): 中文技术社区，可搜索大模型训练、数据工程、推理部署等实战文章；阅读时应结合官方文档核验版本和结论。
- [腾讯云开发者社区](https://cloud.tencent.com/developer/): 中文开发者内容平台，提供云上 AI、模型训练和工程实践文章，可用作国产工具与落地案例的补充来源。
- [博客园](https://www.cnblogs.com/): 中文技术博客社区，包含算法原理、代码实现和踩坑记录；适合作为问题检索入口，需注意文章时效与质量差异。
