# LLM 评测资源索引

## 1. 评测原理与综述

- [A Survey on Evaluation of Large Language Models](https://arxiv.org/abs/2307.03109): LLM 评测经典综述，从"评什么/在哪评/怎么评"三维度系统梳理 NLP 任务、推理、医疗、伦理、教育与 Agent 等评测方法、基准与成败案例，适合建立评测知识全景。
- [A Practical Guide for Evaluating LLMs and LLM-Reliant Systems](https://arxiv.org/abs/2506.13023): LLM 评测实用指南论文，讨论真实场景下代表性数据集策划、指标选择与方法论，弥补合成基准与默认指标的不足，适合落地评测体系设计。
- [Survey on Evaluation of LLM-based Agents](https://arxiv.org/abs/2503.16416): LLM Agent 评测综述，覆盖核心能力（规划/工具使用）、应用基准（Web/SWE）、通用 Agent、基准维度与评测工具五视角，适合追踪 Agent 评测前沿。
- [LLMs-as-Judges: A Comprehensive Survey on LLM-based Evaluation Methods](https://arxiv.org/abs/2412.05579): LLM 作为评判者综述，从功能性、方法论、应用、元评测与局限五方面系统梳理，配套仓库 [CSHaitao/Awesome-LLMs-as-Judges](https://github.com/CSHaitao/Awesome-LLMs-as-Judges)。
- <img src="https://img.shields.io/github/stars/huggingface/evaluation-guidebook?style=social" height="17" align="texttop"/> [evaluation-guidebook](https://github.com/huggingface/evaluation-guidebook): Hugging Face 的 LLM 评测指南书，覆盖自动基准、人工评测、LLM-as-Judge、故障排查与通识，含中文社区翻译，适合系统学习评测设计（注：仓库已迁移至 [HF Space](https://huggingface.co/spaces/OpenEvals/evaluation-guidebook) 持续更新）。

## 2. 评测框架与工具

- <img src="https://img.shields.io/github/stars/EvolvingLMMs-Lab/lmms-eval?style=social" height="17" align="texttop"/> [lmms-eval](https://github.com/EvolvingLMMs-Lab/lmms-eval): 多模态大模型评测框架，提供统一接口运行多模态基准，支持多模型并发评测，适合 VLM 能力评估。
- <img src="https://img.shields.io/github/stars/EleutherAI/lm-evaluation-harness?style=social" height="17" align="texttop"/> [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness): EleutherAI 的开源 LLM 评测框架，支持数百项基准、少样本评测与多后端模型对接，是学术界最常用的评测工具之一。
- <img src="https://img.shields.io/github/stars/openai/evals?style=social" height="17" align="texttop"/> [evals](https://github.com/openai/evals): OpenAI 的早期评测框架，提供数据集、评测流程与基准模板，适合构建模型行为评测，注：已被 simple-evals 等新方案逐步替代。
- <img src="https://img.shields.io/github/stars/openai/simple-evals?style=social" height="17" align="texttop"/> [simple-evals](https://github.com/openai/simple-evals): OpenAI 的轻量评测库，提供简洁 API 运行 MMLU、GPQA 等基准，适合快速复现模型评测结果。
- <img src="https://img.shields.io/github/stars/confident-ai/deepeval?style=social" height="17" align="texttop"/> [deepeval](https://github.com/confident-ai/deepeval): LLM 应用评测框架，提供单元测试式断言、指标库与 CI 集成，适合对 RAG、对话等应用做回归评测。
- <img src="https://img.shields.io/github/stars/Arize-ai/phoenix?style=social" height="17" align="texttop"/> [phoenix](https://github.com/Arize-ai/phoenix): Arize 的 AI 可观测与评测平台，支持 LLM trace、评测、RAG 检索分析与告警，适合生产应用监控与质量回归。
- <img src="https://img.shields.io/github/stars/promptfoo/promptfoo?style=social" height="17" align="texttop"/> [promptfoo](https://github.com/promptfoo/promptfoo): 提示与模型评测工具，支持批量测试、红队、A/B 对比与 CI 集成，适合在提示迭代中保证质量。
- <img src="https://img.shields.io/github/stars/truera/trulens?style=social" height="17" align="texttop"/> [trulens](https://github.com/truera/trulens): LLM 应用评测与可观测框架，提供 RAG 三元组指标、反馈函数与链路追踪，适合评估与优化 RAG 应用。
- <img src="https://img.shields.io/github/stars/meta-llama/llama-recipes?style=social" height="17" align="texttop"/> [llama-recipes/evaluation](https://github.com/meta-llama/llama-recipes/tree/main/recipes/evaluation): Llama 官方仓库的评测示例集合，演示如何对 Llama 系列模型跑 MMLU 等基准，适合上手 Meta 模型评测。
- <img src="https://img.shields.io/github/stars/open-compass/opencompass?style=social" height="17" align="texttop"/> [opencompass](https://github.com/open-compass/opencompass): 上海 AI Lab 的开源评测框架，支持百余基准、多模态与分布式评测，是中文社区主流的评测工具之一。
- <img src="https://img.shields.io/github/stars/huggingface/lighteval?style=social" height="17" align="texttop"/> [lighteval](https://github.com/huggingface/lighteval): Hugging Face 的轻量评测框架，对接 Open LLM Leaderboard 任务集与 Transformers/TRL，适合在 HF 栈内做模型评测。
- <img src="https://img.shields.io/github/stars/UKGovernmentBEIS/inspect_ai?style=social" height="17" align="texttop"/> [inspect_ai](https://github.com/UKGovernmentBEIS/inspect_ai): 英国政府的 LLM 评测框架，支持任务设计、求解器、评分器与可扩展评测，适合构建安全与能力评测套件。
- <img src="https://img.shields.io/github/stars/alopatenko/LLMEvaluation?style=social" height="17" align="texttop"/> [LLMEvaluation](https://github.com/alopatenko/LLMEvaluation): LLM 评测资源与工具合集，收录基准、方法与实现，适合作为评测调研的补充参考。

## 3. 排行榜与公开基准

- [Facts Benchmark Suite](https://deepmind.google/blog/facts-benchmark-suite-systematically-evaluating-the-factuality-of-large-language-models/)：DeepMind 的事实性基准，系统评测 LLM 的事实准确性与幻觉，适合评估模型可信度。
- <img src="https://img.shields.io/github/stars/huggingface/open-llm-leaderboard?style=social" height="17" align="texttop"/> [Open LLM Leaderboard](https://huggingface.co/spaces/open-llm-leaderboard/open_llm_leaderboard)：Hugging Face 的开源 LLM 排行榜，基于 MMLU、ARC、GSM8K 等基准对开源模型统一排名，是追踪开源模型能力演进的主入口。
- [HELM](https://crfm.stanford.edu/helm/)：Stanford CRFM 的整体评测基准，覆盖多任务、指标、场景与公平性，提供模型能力的多维剖析报告。
- [The Big Benchmarks Collection](https://huggingface.co/collections/open-llm-leaderboard/the-big-benchmarks-collection-64faca6335a7fc7d4ffe974a)：Open LLM Leaderboard 维护的主流基准集合，汇总 MMLU、BBH、GSM8K、ARC、HellaSwag 等，适合选型与复测。
- <img src="https://img.shields.io/github/stars/lm-sys/FastChat?style=social" height="17" align="texttop"/> [FastChat](https://github.com/lm-sys/FastChat)：LMSYS 的对话模型训练与服务框架，也是 Chatbot Arena 的底层平台，提供多模型对战与人类偏好数据采集能力。
- [Chatbot Arena](https://chat.lmsys.org/)：LMSYS 的众包人类偏好对战排行榜，通过盲对比投票对模型进行 Elo 排名，是当前最具公信力的人类评测之一。
- [Artificial Analysis](https://artificialanalysis.ai/)：AI 模型性能分析与排行榜平台，横向对比各模型在质量、延迟、价格上的表现，适合模型选型决策。
- [Arena Leaderboard](https://arena.ai/leaderboard)：AI 模型对战竞技场排行榜，通过众包投票对各类模型做能力排名，适合从用户偏好视角看模型差异。
- [SWE-bench](https://www.swebench.com/)：软件工程能力基准，基于真实 GitHub issue 评测模型解决代码问题的能力，是评估代码 Agent 的权威基准。
- [OpenCompass 司南](https://opencompass.org.cn/home)：上海 AI Lab 的模型评测榜单，覆盖语言、多模态、代码、Agent 等能力，是中文社区主流的模型能力评测入口。
- [LiveBench](https://livebench.ai/#/)：持续更新的抗污染评测基准，定期刷新题目以防止模型记忆，适合获得不易被刷分的真实能力排名。
- [Arena](https://arena.atease.dev/)：AI 模型对战竞技场，提供多模型盲对比与投票排名，适合从对战视角了解模型相对强弱。

## 4. LLM-as-Judge 与自动评测

- <img src="https://img.shields.io/github/stars/lm-sys/FastChat?style=social" height="17" align="texttop"/> [FastChat/llm_judge](https://github.com/lm-sys/FastChat/tree/main/fastchat/llm_judge): FastChat 的 LLM 评判模块，提供基于强模型（如 GPT-4）自动打分的 prompt 模板与流程，是 LLM-as-Judge 的早期参考实现。
- <img src="https://img.shields.io/github/stars/dependentsign/Awesome-LLM-based-Evaluators?style=social" height="17" align="texttop"/> [Awesome-LLM-based-Evaluators](https://github.com/dependentsign/Awesome-LLM-based-Evaluators): LLM 作为评测者资源索引，收录相关论文、方法与工具，适合追踪自动评测研究。
- <img src="https://img.shields.io/github/stars/xsankar/Awesome-LLM-Eval-MetricMinds?style=social" height="17" align="texttop"/> [Awesome-LLM-Eval-MetricMinds](https://github.com/xsankar/Awesome-LLM-Eval-MetricMinds): LLM 评测指标资源索引，汇总自动评测与人工评测中常用指标及其原理，适合理解指标选型。
- <img src="https://img.shields.io/github/stars/haizelabs/awesome-llm-judges?style=social" height="17" align="texttop"/> [awesome-llm-judges](https://github.com/haizelabs/awesome-llm-judges): LLM 评判者资源合集，收录评判方法、prompt 设计与元评测研究，适合构建自动评判流程。
- <img src="https://img.shields.io/github/stars/CSHaitao/Awesome-LLMs-as-Judges?style=social" height="17" align="texttop"/> [Awesome-LLMs-as-Judges](https://github.com/CSHaitao/Awesome-LLMs-as-Judges): LLM-as-Judge 综述《LLMs-as-Judges: A Comprehensive Survey》的配套资源仓库，系统整理评判范式、元评测与局限研究。
- [Evaluation Best Practices](https://developers.openai.com/api/docs/guides/evaluation-best-practices)：OpenAI 的评测最佳实践指南，讲解评测目标设定、数据构造、指标选择与迭代流程，适合制定评测规范。
- [Develop & Test with Claude](https://docs.anthropic.com/en/docs/build-with-claude/develop-tests)：Anthropic 关于使用 Claude 进行测试开发的文档，介绍测试用例构造与评测集成，适合 Claude 应用质量保障。
- [Bloom Auto-Evals](https://alignment.anthropic.com/2025/bloom-auto-evals/)：Anthropic Alignment 的自动评测研究，探索用模型自动评估模型能力与对齐属性，适合了解可扩展监督前沿。
- [A Statistical Approach to Model Evals](https://www.anthropic.com/research/statistical-approach-to-model-evals)：Anthropic 关于模型评测统计方法的博客，讨论显著性、置信区间与样本量设计，适合提升评测结论的统计严谨性。

## 5. 应用与安全评测

- [Demystifying Evals for AI Agents](https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents)：Anthropic 关于 AI Agent 评测的工程博客，拆解 Agent 评测的维度、指标与难点，适合设计 Agent 评测方案。
- <img src="https://img.shields.io/github/stars/explodinggradients/ragas?style=social" height="17" align="texttop"/> [ragas](https://github.com/explodinggradients/ragas): RAG 应用评测框架，提供上下文相关性、答案忠实度与有用性等指标，适合量化与优化 RAG 链路质量。
- <img src="https://img.shields.io/github/stars/EdinburghNLP/awesome-hallucination-detection?style=social" height="17" align="texttop"/> [awesome-hallucination-detection](https://github.com/EdinburghNLP/awesome-hallucination-detection): 幻觉检测资源索引，收录检测方法、数据集与论文，适合研究模型事实性与幻觉缓解。
- [OpenAI × Anthropic Safety Evaluation](https://openai.com/index/openai-anthropic-safety-evaluation/)：OpenAI 与 Anthropic 联合发布的安全评测合作，介绍前沿模型安全评测的方法与协作方向。
- [Exploit Evals](https://www.anthropic.com/research/exploit-evals)：Anthropic 关于利用性评测的研究，评估模型在对抗性利用场景下的风险，适合红队与安全测试。
- [Gemini 3.1 Pro Model Evaluation](https://storage.googleapis.com/deepmind-media/gemini/gemini_3-1_pro_model_evaluation.pdf)：Google DeepMind 的 Gemini 3.1 Pro 模型评测报告，披露其在各类基准上的能力与安全评测结果。
- [Eval Skills](https://developers.openai.com/blog/eval-skills)：OpenAI 开发者博客关于评测技能的讨论，介绍如何构建与运用评测能力评估模型表现。
- [Scaling Cyber Defenders with Daybreak](https://developers.openai.com/blog/scaling-cyber-defenders-with-daybreak)：OpenAI 关于用模型提升网络安全的实践，涉及安全场景下的能力评测与部署。
- [Challenges in Red Teaming AI Systems](https://www.anthropic.com/news/challenges-in-red-teaming-ai-systems)：Anthropic 关于 AI 红队挑战的讨论，梳理红队评测的难点、方法与组织经验。
- [Strategic Warning for AI Risk](https://www.anthropic.com/news/strategic-warning-for-ai-risk-progress-and-insights-from-our-frontier-red-team)：Anthropic 前沿红队的 AI 风险进展与洞察，分享红队评测在风险发现中的作用。
- [Auditing Hidden Objectives](https://www.anthropic.com/research/auditing-hidden-objectives)：Anthropic 关于审计模型隐藏目标的研究，探讨发现模型潜在未对齐行为的方法，适合前沿安全研究。

## 6. 官方平台与云评测服务

- [OpenAI Evals API Guide](https://developers.openai.com/api/docs/guides/evals)：OpenAI 的 Evals API 指南，讲解通过 API 运行评测、定义评测任务与查看结果，适合在 OpenAI 栈内做模型评测。
- [OpenAI Platform Evals Guide](https://platform.openai.com/docs/guides/evals)：OpenAI 平台的评测功能指南，介绍从界面与 API 运行自定义评测的完整流程。
- [Evaluate with Claude](https://docs.anthropic.com/en/docs/build-with-claude/evaluate)：Anthropic 关于使用 Claude 进行评测的文档，介绍如何用 Claude 做生成质量与对齐评测。
- [Vertex AI Model Evaluation](https://cloud.google.com/vertex-ai/generative-ai/docs/models/evaluate-models)：Google Vertex AI 的模型评测文档，说明如何在云端对生成式模型做自动与人工评测。
- [Azure AI Studio Evaluation](https://learn.microsoft.com/en-us/azure/ai-studio/concepts/evaluation-approach-gen-ai)：Azure AI Studio 的生成式 AI 评测文档，覆盖评测方法、指标与内置工具，适合在 Azure 上做模型与应用评测。
- [LangSmith Evaluation](https://docs.smith.langchain.com/evaluation)：LangSmith 的评测文档，介绍如何在 LangChain 应用中对链与 RAG 做数据集驱动评测与回归测试。

## 7. 学习资源与社区导航

### 7.1 教程与课程

- [Getting Started with OpenAI Evals](https://developers.openai.com/cookbook/examples/evaluation/getting_started_with_openai_evals.md)：OpenAI Cookbook 的 Evals 入门教程，演示从零构建评测任务并运行，适合快速上手 OpenAI 评测体系。
- [OpenAI Cookbook Evaluation](https://cookbook.openai.com/examples/evaluation)：OpenAI Cookbook 的评测示例合集，提供分步代码与场景案例，适合边学边做。
- [Evaluating & Debugging Generative AI](https://www.deeplearning.ai/short-courses/evaluating-debugging-generative-ai/)：DeepLearning.AI 的生成式 AI 评测与调试短课程，讲解评测方法、指标与误差分析，适合建立评测实践基础。
- [W&B LLM Evaluation Course](https://www.wandb.courses/courses/take/llm-evaluation)：Weights & Biases 的 LLM 评测课程，覆盖评测流程、工具与实验追踪，适合结合实验管理做评测。
- [Full Stack Deep Learning LLM Bootcamp](https://fullstackdeeplearning.com/llm-bootcamp/)：全栈深度学习的 LLM 训练营，含 LLM 应用开发与评测模块，适合从工程全栈视角理解评测定位。

### 7.2 博客文章

- [Hugging Face: LLM Evaluation](https://huggingface.co/blog/evaluation)：Hugging Face 关于 LLM 评测的入门博客，讲解为何评测、常见方法与陷阱，是评测指南书的配套导读。
- [Lilian Weng: LLM Evaluation](https://lilianweng.github.io/posts/2023-06-23-evaluation/)：Lilian Weng 的 LLM 评测综述博客，系统梳理评测基准、方法与挑战，是该领域被广泛引用的综述性长文。
- [Arize: LLM Evaluation](https://arize.com/blog-course/llm-evaluation/)：Arize 的 LLM 评测系列博客与课程，覆盖指标、可观测与 RAG 评测，适合工程视角的评测实践。
- [Confident AI Blog](https://www.confident-ai.com/blog)：DeepEval 维护方的博客，发布 LLM 评测方法、案例与工具实践，适合跟踪应用评测动态。
- [Chip Huyen: LLM Evaluation](https://huyenchip.com/2024/03/26/llm-evaluation.html)：Chip Huyen 关于 LLM 评测的博客，讨论评测方法学、指标局限与生产评测设计，适合理解评测落地难点。
- [Fourrier: LLM Evaluation](https://huggingface.co/blog/clefourrier/llm-evaluation)：Hugging Face 的 Clémentine Fourrier 撰写的评测入门博客，讲解评测的原理、方法与误区，是评测指南书的导读。
- [Multilingual Evaluation Best Practices](https://huggingface.co/blog/catherinearnett/multilingual-best-practices)：Hugging Face 关于多语言模型评测的最佳实践博客，讨论语言覆盖、公平性与指标选择。
- [Open LLM Leaderboard & MMLU](https://huggingface.co/blog/open-llm-leaderboard-mmlu)：Hugging Face 关于 Open LLM Leaderboard 与 MMLU 基准的讨论博客，剖析基准局限与改进方向。
- [Hamel Husain: Evals FAQ](https://hamel.dev/blog/posts/evals-faq/)：Hamel Husain 的评测常见问题博客，回答何时做评测、如何设计评测等问题，适合建立评测直觉。
- [Hamel Husain: Error Analysis in LLM Evals](https://hamel.dev/blog/posts/evals-faq/why-is-error-analysis-so-important-in-llm-evals-and-how-is-it-performed.html)：Hamel Husain 关于错误分析在 LLM 评测中重要性的博客，讲解如何开展错误分析以改进模型。
- [Hamel Husain: Office Hours - Error Analysis](https://hamel.dev/notes/llm/officehours/erroranalysis.html)：Hamel Husain 的 office hours 笔记，通过案例演示 LLM 评测中的错误分析方法与流程。
- [Eugene Yan: Product Evals](https://eugeneyan.com/writing/product-evals/)：Eugene Yan 关于产品评测的博客，讨论如何在产品迭代中设计评测、收集反馈与衡量效果。
- [Eugene Yan: AlignEval](https://eugeneyan.com/writing/aligneval/)：Eugene Yan 关于对齐评测的博客，探讨如何让评测与业务目标对齐，避免指标与目标错位。
- [Hamel Husain: Eval Tools](https://hamel.dev/blog/posts/eval-tools/)：Hamel Husain 关于评测工具的博客，梳理与点评常用评测工具，适合工具选型。
- [Hamel Husain: Evals Skills](https://hamel.dev/blog/posts/evals-skills/)：Hamel Husain 关于评测技能的博客，讨论构建评测能力所需的方法与实践。

### 7.3 中文资料

- [SegmentFault：LLM 评测文章](https://segmentfault.com/a/1190000047645758)：SegmentFault 上的中文 LLM 评测文章，面向中文开发者讲解评测方法与实践经验。
- [人人都是产品经理：LLM 评测](https://www.woshipm.com/share/6176886.html)：人人都是产品经理上的 LLM 评测分享，从产品视角讨论模型评测与选型。
- [腾讯云开发者社区：LLM 评测](https://developer.cloud.tencent.com/article/2691939)：腾讯云开发者社区的 LLM 评测文章，提供中文实践视角与工具介绍。
- [CSDN：LLM 评测实践](https://blog.csdn.net/qq_51885001/article/details/163528159)：CSDN 上的中文 LLM 评测实践文章，覆盖评测方法、基准与工具使用。
- [CSDN：LLM 评测方法](https://blog.csdn.net/sinat_39620217/article/details/149352126)：CSDN 上的中文 LLM 评测方法文章，梳理评测指标、流程与案例。

### 7.4 Awesome 索引与综合导航

- <img src="https://img.shields.io/github/stars/x-tahosin/awesome-llm-benchmarks?style=social" height="17" align="texttop"/> [awesome-llm-benchmarks](https://github.com/x-tahosin/awesome-llm-benchmarks): LLM 评测基准资源索引，集中收录各类基准与排行榜，适合快速完成基准调研。
- <img src="https://img.shields.io/github/stars/jakemeany523/awesome-llm-evaluation?style=social" height="17" align="texttop"/> [awesome-llm-evaluation](https://github.com/jakemeany523/awesome-llm-evaluation): LLM 评测资源合集，收录框架、工具、基准与论文，适合建立评测调研清单。
- <img src="https://img.shields.io/github/stars/ankitkapur1992-hlido/Awesome-LLM-Eval?style=social" height="17" align="texttop"/> [Awesome-LLM-Eval](https://github.com/ankitkapur1992-hlido/Awesome-LLM-Eval): LLM 评测资源导航，整理评测方法、工具与基准，适合作为补充索引。
- <img src="https://img.shields.io/github/stars/sdelahaies/llm-eval?style=social" height="17" align="texttop"/> [llm-eval](https://github.com/sdelahaies/llm-eval): LLM 评测资源合集，收录工具与资料，适合扩展调研视野。
- <img src="https://img.shields.io/github/stars/leobeeson/llm_benchmarks?style=social" height="17" align="texttop"/> [llm_benchmarks](https://github.com/leobeeson/llm_benchmarks): LLM 基准资源索引，汇总主流基准与说明，适合基准选型参考。
- <img src="https://img.shields.io/github/stars/onejune2018/Awesome-LLM-Eval?style=social" height="17" align="texttop"/> [Awesome-LLM-Eval](https://github.com/onejune2018/Awesome-LLM-Eval): LLM 评测资源导航，收录评测工具、基准与论文，适合补充调研。
- <img src="https://img.shields.io/github/stars/tjunlp-lab/Awesome-LLMs-Evaluation-Papers?style=social" height="17" align="texttop"/> [Awesome-LLMs-Evaluation-Papers](https://github.com/tjunlp-lab/Awesome-LLMs-Evaluation-Papers): LLM 评测论文索引，按主题收录评测方法、基准与元评测研究，适合追踪学术进展。
- <img src="https://img.shields.io/github/stars/e06084/Awesome-LLM?style=social" height="17" align="texttop"/> [Awesome-LLM](https://github.com/e06084/Awesome-LLM): LLM 综合资源索引，涵盖训练、评测、应用与工具，适合在评测之外扩展视野。
- <img src="https://img.shields.io/github/stars/KylinC/Awesome-Awesome-LLM?style=social" height="17" align="texttop"/> [Awesome-Awesome-LLM](https://github.com/KylinC/Awesome-Awesome-LLM): LLM 元导航仓库，收录并分类各类 LLM awesome list，适合在海量资源中定位方向。
- <img src="https://img.shields.io/github/stars/adongwanai/Awesome-Awesome-LLMs?style=social" height="17" align="texttop"/> [Awesome-Awesome-LLMs](https://github.com/adongwanai/Awesome-Awesome-LLMs): LLM 元导航仓库，收录 200+ 个 awesome list 并按 40+ 细分类与星级评级，适合一站式资源发现。
- <img src="https://img.shields.io/github/stars/Spico197/awesome-lm-evaluation?style=social" height="17" align="texttop"/> [awesome-lm-evaluation](https://github.com/Spico197/awesome-lm-evaluation): 语言模型评测资源索引，收录方法、工具与基准，适合评测调研。
- <img src="https://img.shields.io/github/stars/Vvkmnn/awesome-ai-eval?style=social" height="17" align="texttop"/> [awesome-ai-eval](https://github.com/Vvkmnn/awesome-ai-eval): AI 评测资源合集，覆盖模型与应用评测，适合从更广视角理解评测。
- <img src="https://img.shields.io/github/stars/benchflow-ai/awesome-evals?style=social" height="17" align="texttop"/> [awesome-evals](https://github.com/benchflow-ai/awesome-evals): 评测资源索引，汇总基准、工具与评测研究，适合扩充调研清单。
- <img src="https://img.shields.io/github/stars/AiHubCN/Awesome-LLM-Survey?style=social" height="17" align="texttop"/> [Awesome-LLM-Survey](https://github.com/AiHubCN/Awesome-LLM-Survey): LLM 综述论文导航，收录训练、评测、安全等方向的综述，适合从综述切入了解评测全貌。
- [Awesome LLM Resources](https://wangrongsheng.github.io/awesome-LLM-resources/)：LLM 综合资源导航站，覆盖模型、数据、评测与工具，适合在评测之外扩展学习。
- [GitHub Topic: llm-evaluation](https://github.com/topics/llm-evaluation)：GitHub 的 llm-evaluation 主题页，聚合该标签下的仓库与项目，适合发现新评测资源。
- <img src="https://img.shields.io/github/stars/ConardLi/easy-dataset?style=social" height="17" align="texttop"/> [easy-dataset](https://github.com/ConardLi/easy-dataset): 数据集构建与管理工具，可用于评测数据准备与标注，作为评测流程的前置环节辅助。
