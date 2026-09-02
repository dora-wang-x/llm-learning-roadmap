# 大模型对齐（Alignment）

## 1. 对齐原理与综述

- [AI Alignment: A Comprehensive Survey](https://arxiv.org/abs/2310.19852)：以 RICE 四原则（鲁棒性、可解释性、可控性、道德性）为纲，将对齐拆解为前向对齐（从反馈学习、分布偏移下学习）与后向对齐（保证与治理），配套网站持续更新，适合建立领域全景。
- [Large Language Model Alignment: A Survey](https://arxiv.org/abs/2309.15025)：从内/外对齐视角梳理 LLM 对齐方法，覆盖可解释性、对抗脆弱性、对齐评测基准与未来方向。
- [On the Essence and Prospect: An Investigation of Alignment Approaches for Big Models](https://arxiv.org/abs/2403.04204)：追溯对齐的历史脉络与数学本质，比较强化学习、监督微调与上下文学习三条路线的内在联系，并讨论个性化与多模态对齐等新兴前沿。
- [Aligning Large Language Models with Human: A Survey](https://arxiv.org/abs/2307.12966)：从指令数据收集、训练方法（SFT、在线/离线偏好训练、参数高效训练）与模型评估三方面综述 LLM 人类对齐技术。
- <img src="https://img.shields.io/github/stars/garyyufei/alignllmhumansurvey?style=social" height="17" align="texttop"/> [AlignLLMHumanSurvey](https://github.com/garyyufei/alignllmhumansurvey)：上篇综述（arXiv:2307.12966）的配套仓库，持续收录 LLM 对齐最新论文，按数据、训练、评测分类跟踪进展。
- <img src="https://img.shields.io/github/stars/BinFuPKU/LLM-Alignment?style=social" height="17" align="texttop"/> [LLM-Alignment（北大）](https://github.com/BinFuPKU/LLM-Alignment)：北大团队的中文对齐调研报告，含《大语言模型人类对齐技术调研》《参数微调对齐算法调研报告》（覆盖 10 余种离线/在线 RLHF 算法）及安全价值观 RLHF 数据示例。

## 2. SFT 与指令微调

- <img src="https://img.shields.io/github/stars/tatsu-lab/stanford_alpaca?style=social" height="17" align="texttop"/> [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca)：斯坦福 Alpaca 官方仓库，提供 52K 自指令数据与基于 LLaMA 的 SFT 训练/推理代码，是指令微调的奠基性开源项目。
- <img src="https://img.shields.io/github/stars/ymcui/Chinese-LLaMA-Alpaca?style=social" height="17" align="texttop"/> [Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca)：面向中文的开源增补项目，通过扩充中文词表、继续预训练与中文指令微调，显著提升 LLaMA/Alpaca 系列的中文能力。
- <img src="https://img.shields.io/github/stars/PhoebusSi/Alpaca-CoT?style=social" height="17" align="texttop"/> [Alpaca-CoT](https://github.com/PhoebusSi/Alpaca-CoT)：汇集指令微调数据与思维链（CoT）数据集的项目，统一数据格式并分析 CoT 对对齐效果的影响，便于构造多样化指令数据。
- <img src="https://img.shields.io/github/stars/ConardLi/easy-dataset?style=social" height="17" align="texttop"/> [Easy Dataset](https://github.com/ConardLi/easy-dataset)：将 PDF/Markdown/DOCX 等领域文档自动转换为微调数据集的一站式工具，支持问题生成、领域标签树、答案与思维链生成及多格式导出。
- <img src="https://img.shields.io/github/stars/Curated-Awesome-Lists/awesome-llms-fine-tuning?style=social" height="17" align="texttop"/> [awesome-llms-fine-tuning](https://github.com/Curated-Awesome-Lists/awesome-llms-fine-tuning)：微调相关资源汇总，收集参数高效微调、全量微调与对齐训练的论文、工具和实践案例。

## 3. RLHF、RLAIF 与偏好优化

- [Illustrating Reinforcement Learning from Human Feedback](https://huggingface.co/blog/rlhf)：经典 RLHF 图解博客，以直观图示讲解人类反馈强化学习的流程、奖励模型与 PPO 训练机制。
- [From RLHF to DPO](https://huggingface.co/blog/ariG23498/rlhf-to-dpo)：梳理从 RLHF 到直接偏好优化（DPO）的算法演进，比较两类方法的训练目标与实现差异。
- [Deriving the DPO Loss](https://huggingface.co/blog/garg-aayush/derive-dpo-loss)：从数学推导角度拆解 DPO 损失函数的来源，帮助理解偏好优化目标与 RL 目标的等价关系。
- [DPO meets TRL](https://huggingface.co/blog/dpo-trl)：结合 TRL 库演示 DPO 训练的实践教程，涵盖数据格式、训练配置与效果分析。
- [Preference Tuning](https://huggingface.co/blog/pref-tuning)：介绍偏好调优的思路与实现，讨论无需显式奖励模型的偏好对齐方法。
- [DPO vs ORPO 微调技术](https://huggingface.co/blog/Vanessasml/llm-finetuning-techniques-dpo-orpo)：对比 DPO 与 ORPO 等微调技术的原理与适用场景，给出实践中的选择建议。
- [REBEL：极简偏好优化](https://huggingface.co/blog/GitBag/rebel)：讲解 REBEL 偏好优化算法，一种对参考模型依赖更小的偏好对齐方法。
- [面向 LLM 的强化学习指南](https://huggingface.co/blog/ProCreations/guide-to-rl)：面向 LLM 训练的强化学习入门指南，梳理策略梯度、奖励设计等基础概念，为理解 RLHF 打基础。
- [LLM 后训练算法指南](https://huggingface.co/blog/karina-zadorozhny/guide-to-llm-post-training-algorithms)：系统讲解后训练（SFT、RLHF、DPO 等）算法谱系，比较各算法的目标函数与训练特性。
- <img src="https://img.shields.io/github/stars/opendilab/awesome-RLHF?style=social" height="17" align="texttop"/> [awesome-RLHF](https://github.com/opendilab/awesome-RLHF)：知名 RLHF 论文合集，按方法演进与主题收录 RLHF、奖励建模与偏好优化工作。
- <img src="https://img.shields.io/github/stars/vicgalle/awesome-rlaif?style=social" height="17" align="texttop"/> [awesome-rlaif](https://github.com/vicgalle/awesome-rlaif)：聚焦 RLAIF（AI 反馈强化学习）的资源清单，收集相关论文与项目，适合研究自动化反馈信号。

## 4. 安全对齐

- <img src="https://img.shields.io/github/stars/PKU-Alignment/safe-rlhf?style=social" height="17" align="texttop"/> [Safe RLHF](https://github.com/PKU-Alignment/safe-rlhf)：北大对齐团队的安全 RLHF 框架与算法，将人类反馈拆分为有用性与无害性双目标，支持安全对齐训练全流程。
- <img src="https://img.shields.io/github/stars/PKU-Alignment/beavertails?style=social" height="17" align="texttop"/> [BeaverTails](https://github.com/PKU-Alignment/beavertails)：北大发布的安全偏好数据集，含问答安全性标注与偏好对，用于评测和训练模型的有害内容识别能力。
- <img src="https://img.shields.io/github/stars/Sigil-Core/awesome-ai-safety?style=social" height="17" align="texttop"/> [awesome-ai-safety（Sigil-Core）](https://github.com/Sigil-Core/awesome-ai-safety)：AI 安全领域资源合集，收录对齐、可解释性、风险评估与治理相关的论文和资料。
- <img src="https://img.shields.io/github/stars/AccelerationConsortium/awesome-ai-safety?style=social" height="17" align="texttop"/> [awesome-ai-safety（AccelerationConsortium）](https://github.com/AccelerationConsortium/awesome-ai-safety)：多伦多大学加速联盟维护的 AI 安全清单，覆盖安全研究、评测与工程实践资源。
- <img src="https://img.shields.io/github/stars/vincentlelarge/awesome-llm-safety?style=social" height="17" align="texttop"/> [awesome-llm-safety](https://github.com/vincentlelarge/awesome-llm-safety)：LLM 安全资源索引，汇集越狱攻击、红队测试、安全评测与防御方法相关工作。
- <img src="https://img.shields.io/github/stars/0xSweet/awesome-llm-security-alignment?style=social" height="17" align="texttop"/> [awesome-llm-security-alignment](https://github.com/0xSweet/awesome-llm-security-alignment)：汇总 LLM 安全与对齐交叉领域的工具、论文和案例，关注模型安全防线与对齐失效问题。
- <img src="https://img.shields.io/github/stars/awesomelistsio/awesome-ai-safety-alignment?style=social" height="17" align="texttop"/> [awesome-ai-safety-alignment](https://github.com/awesomelistsio/awesome-ai-safety-alignment)：AI 安全与对齐主题的资源列表，可作为前述安全索引的补充导航。

## 5. 前沿方向

### 自动对齐与可扩展监督

- <img src="https://img.shields.io/github/stars/icip-cas/awesome-auto-alignment?style=social" height="17" align="texttop"/> [awesome-auto-alignment（软件所）](https://github.com/icip-cas/awesome-auto-alignment)：中科院软件所自动对齐综述配套仓库，按归纳偏置、行为模仿、模型反馈、环境反馈四类对齐信号系统整理可扩展自动化对齐研究。
- <img src="https://img.shields.io/github/stars/cascip/awesome-auto-alignment?style=social" height="17" align="texttop"/> [awesome-auto-alignment（计算所）](https://github.com/cascip/awesome-auto-alignment)：中科院计算所维护的同主题资源仓库，配套《Towards Scalable Automated Alignment of LLMs》综述，持续更新论文与代码。
- [OpenAI：Introducing Superalignment](https://openai.com/blog/introducing-superalignment)：OpenAI 超级对齐计划发布文，提出以 AI 辅助人类监督实现对齐超级智能的研究方向与团队规划。

### 推理模型与后训练

- <img src="https://img.shields.io/github/stars/rkinas/reasoning_models_how_to?style=social" height="17" align="texttop"/> [Reasoning Models: How To](https://github.com/rkinas/reasoning_models_how_to)：Amazon 研究者的推理模型与 RLHF 研究笔记，覆盖 GRPO 等 RLVR 训练方法、推理数据合成与验证环境。
- <img src="https://img.shields.io/github/stars/mbzuai-oryx/awesome-llm-post-training?style=social" height="17" align="texttop"/> [awesome-llm-post-training](https://github.com/mbzuai-oryx/awesome-llm-post-training)：汇总后训练（post-training）阶段的论文与资源，覆盖 SFT、偏好优化与推理能力训练等方向。

### 多元、个性化与多模态对齐

- <img src="https://img.shields.io/github/stars/anudeex/Awesome-Pluralistic-Alignment?style=social" height="17" align="texttop"/> [Awesome-Pluralistic-Alignment](https://github.com/anudeex/Awesome-Pluralistic-Alignment)：多元对齐资源清单，关注不同人群价值观差异下的对齐方法与偏好聚合。
- <img src="https://img.shields.io/github/stars/liyongqi2002/Awesome-Personalized-Alignment?style=social" height="17" align="texttop"/> [Awesome-Personalized-Alignment](https://github.com/liyongqi2002/Awesome-Personalized-Alignment)：个性化对齐论文合集，研究面向个体或群体定制偏好的对齐技术。
- <img src="https://img.shields.io/github/stars/NiuTrans/Vision-LLM-Alignment?style=social" height="17" align="texttop"/> [Vision-LLM-Alignment](https://github.com/NiuTrans/Vision-LLM-Alignment)：东北大学 NiuTrans 团队的多模态大模型对齐综述资源，覆盖视觉-语言对齐方法与数据。

## 6. 训练框架与工程实践

- <img src="https://img.shields.io/github/stars/huggingface/alignment-handbook?style=social" height="17" align="texttop"/> [Alignment Handbook](https://github.com/huggingface/alignment-handbook)：Hugging Face 官方对齐手册仓库，提供 SFT、DPO、RLHF 全流程可复现配方，覆盖 Llama/Mistral 等主流模型。
- [The Alignment Handbook 发布博客](https://huggingface.co/blog/the-alignment-handbook)：上述手册的配套介绍博客，说明设计理念、训练配方与复现实验结果。
- <img src="https://img.shields.io/github/stars/hiyouga/LlamaFactory?style=social" height="17" align="texttop"/> [LlamaFactory](https://github.com/hiyouga/LlamaFactory)：易用的大模型微调框架，支持多种开源模型与 SFT、偏好优化、量化训练，可通过 WebUI 零代码微调。
- <img src="https://img.shields.io/github/stars/modelscope/ms-swift?style=social" height="17" align="texttop"/> [ms-swift](https://github.com/modelscope/ms-swift)：魔搭社区官方微调与部署框架，支持数百种模型和主流对齐算法，集成训练、推理、评测与部署链路。
- <img src="https://img.shields.io/github/stars/Lightning-AI/litgpt?style=social" height="17" align="texttop"/> [LitGPT](https://github.com/Lightning-AI/litgpt)：基于 Lightning 生态的高性能 LLM 代码库，提供预训练、微调、偏好优化与部署脚本，实现清晰且易于扩展。
- <img src="https://img.shields.io/github/stars/deepspeedai/DeepSpeed?style=social" height="17" align="texttop"/> [DeepSpeed](https://github.com/deepspeedai/DeepSpeed)：Microsoft 的大模型训练优化库，ZeRO 系列技术降低显存占用，是大规模 RLHF 训练的常用底座。
- <img src="https://img.shields.io/github/stars/deepspeedai/DeepSpeedExamples?style=social" height="17" align="texttop"/> [DeepSpeedExamples](https://github.com/deepspeedai/DeepSpeedExamples)：DeepSpeed 官方示例集，包含 DeepSpeed-Chat 的 RLHF 三阶段训练示例等可运行配置。
- [DeepSpeed 官方文档](https://www.deepspeed.ai/)：DeepSpeed 官方文档站，系统说明安装、配置、ZeRO 与各类并行训练的用法。
- [DeepSpeed-Chat 中文教程](https://techdiylife.github.io/big-model-training/deepspeed/deepspeed-chat.html)：中文图文教程，逐步拆解 DeepSpeed-Chat 的 RLHF 三阶段流程（SFT、奖励模型、PPO）与实战细节。
- <img src="https://img.shields.io/github/stars/datawhalechina/self-llm?style=social" height="17" align="texttop"/> [Self-LLM](https://github.com/datawhalechina/self-llm)：Datawhale 开源大模型食用指南，以中文环境为主线讲解开源模型部署、微调与简单对齐实践。
- <img src="https://img.shields.io/github/stars/astorfi/LLM-Alignment-Project?style=social" height="17" align="texttop"/> [LLM-Alignment-Project](https://github.com/astorfi/LLM-Alignment-Project)：以 Notebook 形式讲解对齐训练实现的项目，覆盖 SFT 与偏好优化算法的动手实验。

## 7. 延伸学习与资源导航

### 官方研究与机构动态

- [OpenAI Alignment](https://alignment.openai.com/#page=1)：OpenAI 对齐研究专题站，汇集对齐目标、方法与团队研究的官方介绍。
- [OpenAI：Aligning AI systems with human intent](https://openai.com/research/aligning-ai-systems-with-human-intent)：OpenAI 关于"让 AI 系统符合人类意图"的研究综述页面，梳理对齐问题定义与已有工作。
- [OpenAI：Our approach to alignment research](https://openai.com/blog/our-approach-to-alignment-research)：OpenAI 官方博客阐述其对齐研究方法论：迭代地在能力更强的模型上研究对齐并工程化落地。
- [Anthropic Alignment](https://alignment.anthropic.com/)：Anthropic 对齐研究门户，介绍其宏观对齐策略、可解释性研究与团队工作。
- [Anthropic Research](https://www.anthropic.com/research)：Anthropic 研究主页，覆盖对齐、可解释性、安全与能力研究，可跟踪其技术报告发布。
- [DeepMind：Securing the future of AI agents](https://deepmind.google/blog/securing-the-future-of-ai-agents/)：DeepMind 关于 AI 智能体安全的博客，讨论智能体风险与安全评估框架。
- [DeepMind：Taking a responsible path to AGI](https://deepmind.google/blog/taking-a-responsible-path-to-agi/)：DeepMind 阐述通往 AGI 的负责任路线，涉及安全研究、治理与国际协作。
- [DeepMind Alignment 博客分类](https://deepmind.google/discover/blog/?categories=alignment)：DeepMind 博客的对齐主题聚合页，集中发布对齐与安全相关研究进展。
- [Google DeepMind Research](https://www.deepmind.com/research)：Google DeepMind 研究门户，可按主题浏览基础模型、安全与对齐方向的论文。
- [Google：Responsible AI practices](https://ai.google/responsibility/responsible-ai-practices/)：Google 的负责任 AI 实践页面，提供安全、公平、隐私等维度的开发准则与工具指引。

### 社区与论坛

- [Alignment Forum](https://www.alignmentforum.org/)：对齐研究核心社区，汇聚对齐理论、风险分析与技术方案的高质量讨论与综述帖。
- [LessWrong：AI Alignment 标签](https://www.lesswrong.com/tag/ai-alignment)：LessWrong 的 AI 对齐标签聚合页，收录对齐相关的社区文章与经典讨论。
- <img src="https://img.shields.io/github/stars/chaoss/wg-ai-alignment?style=social" height="17" align="texttop"/> [CHAOSS AI Alignment 工作组](https://github.com/chaoss/wg-ai-alignment)：CHAOSS 开源社区的 AI 对齐工作组，制定"AI 系统理解并尊重开源社区价值"的评估指标与治理方案。
- [GitHub Topic：llm-alignment](https://github.com/topics/llm-alignment)：GitHub 上 llm-alignment 主题页，可按热度浏览相关开源项目与代码仓库。

### 综合索引
- <img src="https://img.shields.io/github/stars/dit7ya/awesome-ai-alignment?style=social" height="17" align="texttop"/> [awesome-ai-alignment](https://github.com/dit7ya/awesome-ai-alignment)：AI 对齐主题的 awesome 清单，覆盖对齐方法、安全与治理资源。
- <img src="https://img.shields.io/github/stars/Hannibal046/Awesome-LLM?style=social" height="17" align="texttop"/> [Awesome-LLM 对齐论文列表](https://github.com/Hannibal046/Awesome-LLM/blob/main/paper_list/alignment.md)：Awesome-LLM 仓库的对齐论文子列表，按 RLHF、安全等主题收录主流工作。
- <img src="https://img.shields.io/github/stars/AiHubCN/Awesome-LLM-Survey?style=social" height="17" align="texttop"/> [Awesome-LLM-Survey](https://github.com/AiHubCN/Awesome-LLM-Survey)：LLM 综述论文大全，按主题汇总各方向 survey，可用于快速定位对齐相关综述全文。
