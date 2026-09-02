# LLM 数据工程资源

## 1. 数据发现与采集

- <img src="https://img.shields.io/github/stars/dlt-hub/dlt?style=social" height="17" align="texttop"/> [dlt](https://github.com/dlt-hub/dlt): 开源 Python 数据加载库，以声明式资源和管道抽象简化 API、数据库及文件数据的抽取、规范化和落库，适合构建可维护的数据接入层。
- <img src="https://img.shields.io/github/stars/UpstageAI/dataverse?style=social" height="17" align="texttop"/> [dataverse](https://github.com/UpstageAI/dataverse): 面向大模型数据的发现、处理和管理框架，提供数据源连接、处理管道与数据集管理能力，适合将多来源语料接入统一的数据工程工作流。
- [LLMs & Data Engineering](https://medium.com/dcsfamily/llms-data-engineering-e3dae13ff8fd)：从实际数据工程工作视角讨论如何让 LLM 辅助理解数据、编写处理逻辑与自动化任务，为将模型引入日常数据管道提供入门案例。
- [Utilizing LLMs for Data Engineers-part1](https://medium.com/@2005669/utilizing-llms-for-data-engineers-a0f39ba28f85)：介绍数据工程师使用 LLM 的常见切入点，包括 SQL 与代码生成、文档辅助和数据任务分析，帮助识别适合人机协作的重复性工作。
- [Utilizing LLMs for Data Engineers-part2](https://medium.com/@2005669/utilising-llms-for-data-engineers-part-2-db47ca42ec8b)：延续前文讨论 LLM 在数据工程中的落地方式，关注提示设计、任务验证与工程限制，适合结合具体管道评估自动化的可靠边界。
- [RAG技术完整学习笔记：从0到1搭建生产级系统](https://www.cnblogs.com/2678066103hs/p/21603089)：中文实践文章，围绕大模型与数据工程结合的场景梳理工具和实现思路，适合快速了解本地开发语境下的数据处理应用方式。

## 2. 清洗、去重与过滤

- <img src="https://img.shields.io/github/stars/huggingface/datatrove?style=social" height="17" align="texttop"/> [datatrove](https://github.com/huggingface/datatrove): Hugging Face 的模块化数据处理库，提供过滤、去重、分词和数据读写等可组合管道模块，适合大规模文本语料的可定制清洗流程。
- <img src="https://img.shields.io/github/stars/allenai/dolma?style=social" height="17" align="texttop"/> [dolma](https://github.com/allenai/dolma): AI2 发布的 OLMo 预训练数据及工具集合，覆盖语料构建、检查和处理流程，可用于研究开放预训练数据的来源、质量与配方。
- <img src="https://img.shields.io/github/stars/NVIDIA-NeMo/Curator?style=social" height="17" align="texttop"/> [NeMo Curator](https://github.com/NVIDIA-NeMo/Curator): NVIDIA 的可扩展数据预处理与整理工具包，支持大规模文本和多模态数据过滤、去重及质量筛选，面向 LLM 训练语料构建场景。
- <img src="https://img.shields.io/github/stars/data-prep-kit/data-prep-kit?style=social" height="17" align="texttop"/> [data-prep-kit](https://github.com/data-prep-kit/data-prep-kit): 面向生成式 AI 的开源数据准备项目，提供可扩展的转换组件和运行管道，用于文档解析、清洗、去重及训练数据加工。
- <img src="https://img.shields.io/github/stars/datajuicer/data-juicer?style=social" height="17" align="texttop"/> [data-juicer](https://github.com/datajuicer/data-juicer): 面向基础模型的数据处理系统，集成多种数据分析、清洗、去重、筛选和增强算子，并支持基于数据反馈优化数据处理配方。
- [Mastering LLM Techniques: Text Data Processing](https://developer.nvidia.com/blog/mastering-llm-techniques-data-preprocessing)：NVIDIA 技术文章系统说明文本清洗、过滤、去重与质量评估对 LLM 训练的作用，并结合 NeMo Curator 展示规模化数据预处理思路。
- [Training data for LLMs: What it is and how to get it right](https://dotdatalabs.ai/blog/training-data-for-llms-what-it-is-and-how-to-get-it-right)：讲解 LLM 训练数据的组成、来源与质量控制要点，强调代表性、去重、偏差和版权等问题，适合作为制定数据准入标准的参考。

## 3. 转换、标注与格式化

- <img src="https://img.shields.io/github/stars/mosaicml/llm-foundry?style=social" height="17" align="texttop"/> [llm-foundry](https://github.com/mosaicml/llm-foundry): MosaicML 的 LLM 训练与数据处理框架，提供数据集转换、流式加载、训练配方与评估能力，适合将原始数据加工为可训练的数据格式。
- <img src="https://img.shields.io/github/stars/FranxYao/Long-Context-Data-Engineering?style=social" height="17" align="texttop"/> [Long-Context-Data-Engineering](https://github.com/FranxYao/Long-Context-Data-Engineering): 聚焦长上下文模型的数据工程资源，整理长文档构造、长度扩展、位置编码相关数据和评测材料，适合研究长序列训练数据设计。
- [Integrating LLMs into Modern Data Engineering Pipelines](https://medium.com/@guntreddideepaksai/integrating-llms-into-modern-data-engineering-pipelines-40422a978584)：讨论在既有数据管道中嵌入 LLM 的方式，包括非结构化内容抽取、分类、转换和自动化决策，适合评估模型调用在 ETL 环节的价值。
- [Data-Centric AI 教程](https://dcaitutorial.github.io/)：围绕数据中心 AI 的在线教程，介绍如何通过系统化的数据采集、标注、诊断和迭代提升模型表现，而不是只依赖模型结构调整。
- [Data-Centric AI KDD 2023 讲义](https://dcaitutorial.github.io/files/data-centric_AI_KDD2023.pdf)：KDD 2023 的 Data-Centric AI 教程讲义，系统覆盖数据质量、标注噪声、数据调试和数据迭代方法，适合作为理论与实践的集中参考。

## 4. 质量评估与数据混合

- <img src="https://img.shields.io/github/stars/mlfoundations/dclm?style=social" height="17" align="texttop"/> [DCLM](https://github.com/mlfoundations/dclm): DataComp for Language Models 基准项目，提供语言模型数据整理竞赛、数据池和评测工具，用于可复现地比较数据筛选策略对预训练效果的影响。
- [Curating Trillion-Token Datasets: Introducing NVIDIA NeMo Data Curator](https://developer.nvidia.com/blog/curating-trillion-token-datasets-introducing-nemo-data-curator/)：介绍 NeMo Data Curator 面向万亿 Token 语料的处理方法，涉及质量筛选、精确与近似去重及 GPU 加速，适合了解超大规模实践。
- [LLM 系列 (十二)：预训练数据工程：大模型的燃料是如何炼成的](https://matt33.com/2026/07/02/llm-pretraining-data-engineering/)：聚焦预训练阶段的数据工程文章，讨论语料收集、清洗、去重、采样与质量控制的协同关系，帮助建立从原始网页到训练集的完整认识。
- [optimal-dataset-mixing](https://huggingface.co/blog/codelion/optimal-dataset-mixing)：Hugging Face 社区文章，讨论如何确定多数据集的训练配比和混合策略，适合在质量、领域覆盖与训练预算之间做实验化权衡。

## 5. 指令、偏好与人工反馈数据

- <img src="https://img.shields.io/github/stars/argilla-io/distilabel?style=social" height="17" align="texttop"/> [distilabel](https://github.com/argilla-io/distilabel): 用于合成数据和 AI 反馈的可扩展框架，基于研究方法构建可复现流水线，支持生成、评判和过滤指令或偏好数据。
- <img src="https://img.shields.io/github/stars/zjunlp/EasyInstruct?style=social" height="17" align="texttop"/> [EasyInstruct](https://github.com/zjunlp/EasyInstruct): ACL 2024 指令数据处理框架，整合指令生成、选择、评估与格式转换等流程，帮助研究者和工程师高效构造 LLM 指令微调数据。
- <img src="https://img.shields.io/github/stars/glgh/awesome-llm-human-preference-datasets?style=social" height="17" align="texttop"/> [awesome-llm-human-preference-datasets](https://github.com/glgh/awesome-llm-human-preference-datasets): 汇集人类偏好数据集的索引，覆盖对话、比较、奖励建模和安全等任务，为 RLHF、DPO 等对齐方法选择数据来源提供导航。
- <img src="https://img.shields.io/github/stars/haolpku/Awesome-LLM-Data-Preparation?style=social" height="17" align="texttop"/> [Awesome-LLM-Data-Preparation](https://github.com/haolpku/Awesome-LLM-Data-Preparation): 整理 LLM 数据准备相关论文、工具、数据集和教程，涵盖预训练、指令微调与偏好数据构造，适合作为方案调研的索引入口。
- <img src="https://img.shields.io/github/stars/raunak-agarwal/instruction-datasets?style=social" height="17" align="texttop"/> [instruction-datasets](https://github.com/raunak-agarwal/instruction-datasets): 指令微调数据集汇总索引，按金标准、模型生成和偏好数据三类收录 P3、FLAN、LIMA、UltraFeedback 等公开数据集及链接，适合快速盘点指令与偏好数据来源（最后更新于 2023 年，注意核对最新状态）。

## 6. 合成数据与数据扩增

- <img src="https://img.shields.io/github/stars/wasiahmad/Awesome-LLM-Synthetic-Data?style=social" height="17" align="texttop"/> [Awesome-LLM-Synthetic-Data](https://github.com/wasiahmad/Awesome-LLM-Synthetic-Data): 围绕 LLM 合成数据生成的阅读清单，按方法、任务和应用收录论文与资源，适合追踪自指令、蒸馏和数据扩增研究脉络。
- <img src="https://img.shields.io/github/stars/chenmengdx/awesome-data-synthesis-for-code-llm?style=social" height="17" align="texttop"/> [awesome-data-synthesis-for-code-llm](https://github.com/chenmengdx/awesome-data-synthesis-for-code-llm): 专注代码大模型的数据合成资源索引，收集代码生成、测试、验证和清洗相关工作，适合构建高质量代码指令与推理数据。
- <img src="https://img.shields.io/github/stars/davanstrien/awesome-synthetic-datasets?style=social" height="17" align="texttop"/> [awesome-synthetic-datasets](https://github.com/davanstrien/awesome-synthetic-datasets): 汇总跨领域合成数据集、工具和研究资源，覆盖文本、视觉与结构化数据，可用于发现不同任务的数据增强方案和公开数据来源。
- <img src="https://img.shields.io/github/stars/pengr/LLM-Synthetic-Data?style=social" height="17" align="texttop"/> [LLM-Synthetic-Data](https://github.com/pengr/LLM-Synthetic-Data): 聚合 LLM 合成数据相关论文与项目，关注由模型生成训练样本的流程、质量控制和应用场景，适合快速建立领域文献地图。
- <img src="https://img.shields.io/github/stars/ahmad-alismail/LLM_based_Synthetic_Data_Generation?style=social" height="17" align="texttop"/> [LLM_based_Synthetic_Data_Generation](https://github.com/ahmad-alismail/LLM_based_Synthetic_Data_Generation): 收集基于 LLM 的合成数据生成资源，覆盖提示驱动生成、评估与应用案例，为设计数据扩增实验提供方法与工具线索。
- [Cosmopedia](https://huggingface.co/blog/cosmopedia)：Hugging Face 对 Cosmopedia 的介绍，说明如何以筛选网页内容和合成教材、故事及网页文本构造大规模高质量训练语料。
- [Advanced Code Generation With LLMs - Building a Synthetic Data Generator](https://towardsdatascience.com/advanced-code-generation-with-llms-building-a-synthetic-data-generator-0e7ed7b496dc/)：以代码生成任务为例讲解合成数据生成器的构建，涉及提示模板、样本生成和结果校验，适合参考端到端的数据扩增原型。

## 7. 数据管道、DataOps 与治理

- <img src="https://img.shields.io/github/stars/sriram488/llm-driven-data-engineering?style=social" height="17" align="texttop"/> [llm-driven-data-engineering（实践项目）](https://github.com/sriram488/llm-driven-data-engineering): 以代码和示例探索 LLM 驱动的数据工程实践，关注利用模型辅助数据处理和工作流自动化，适合与课程型资源对照阅读。
- <img src="https://img.shields.io/github/stars/DataExpert-io/llm-driven-data-engineering?style=social" height="17" align="texttop"/> [llm-driven-data-engineering（课程）](https://github.com/DataExpert-io/llm-driven-data-engineering): DataExpert.io 的公开课程仓库，系统梳理 LLM 驱动数据工程概念与学习材料，适合了解模型如何参与数据平台和工程流程。
- <img src="https://img.shields.io/github/stars/inference-ai-course/MLE_in_Gen_AI-Course?style=social" height="17" align="texttop"/> [MLE_in_Gen_AI-Course](https://github.com/inference-ai-course/MLE_in_Gen_AI-Course): 面向生成式 AI 的机器学习工程课程，覆盖模型开发、数据、部署和应用实践，适合将数据工程知识放到完整的生成式 AI 系统中理解。
- <img src="https://img.shields.io/github/stars/avvorstenbosch/Masterclass-LLMs-for-Data-Science?style=social" height="17" align="texttop"/> [Masterclass-LLMs-for-Data-Science](https://github.com/avvorstenbosch/Masterclass-LLMs-for-Data-Science): 面向数据科学人员的 LLM 学习资料，围绕基础概念、实际应用与案例组织内容，帮助将大模型能力引入分析和数据科学工作流。
- <img src="https://img.shields.io/github/stars/datascale-ai/data_engineering_book?style=social" height="17" align="texttop"/> [大模型数据工程：架构、算法及项目实战](https://github.com/datascale-ai/data_engineering_book): 覆盖预训练清洗、多模态对齐、RAG、合成数据与 DataOps 的系统教材，含端到端项目案例和可运行代码，适合建立完整技术体系。
- [Agentic Data Engineering 课程](https://dlthub.com/blog/agentic-data-engineering-course)：dlt 发布的课程，围绕以智能体辅助构建数据管道的思路展开，帮助理解数据抽取、编排和自动化如何结合 LLM 与 Agent 工作方式。
- [Modern Data Engineering with LLMs](https://www.booksamillion.com/p/Modern-Data-Engineering-LLMs/Alira-Vexel/9798275581041)：介绍《Modern Data Engineering with LLMs》的图书页面，可作为查找该书内容与版本信息的入口，主题聚焦现代数据工程与大模型的结合。
- [Databricks：面向 AI 的数据工程](https://www.databricks.com/blog/data-engineering-for-ai)：Databricks 文章阐述 AI 工作负载对数据工程的要求，讨论统一数据平台、可靠管道和数据质量如何支撑模型开发与生产应用。
- [Databricks：数据工程与生成式 AI 工具](https://www.databricks.com/blog/data-engineering-and-genai-tools-practitioners-need)：面向实践者梳理生成式 AI 时代常用的数据工程能力与工具，关注数据摄取、转换、治理和服务化等工程环节。
- [Databricks：AI First 数据工程、Lakeflow 与 Agent Bricks](https://www.databricks.com/blog/ai-first-approach-data-engineering-lakeflow-and-agent-bricks)：介绍 Databricks 的 AI First 数据工程方向及 Lakeflow、Agent Bricks 等产品概念，用于了解平台化编排与 AI 应用构建的结合。
- [Databricks：什么是 DataOps](https://www.databricks.com/blog/what-is-dataops)：解释 DataOps 的定义、协作方式和自动化原则，强调以测试、监控和持续交付提高数据管道的可靠性、速度与可治理性。

## 8. 综合资源索引与延伸阅读

- <img src="https://img.shields.io/github/stars/Hannibal046/Awesome-LLM?style=social" height="17" align="texttop"/> [Awesome-LLM](https://github.com/Hannibal046/Awesome-LLM): 大语言模型综合资源索引，收录论文、模型、数据集、工具和课程等内容，适合作为跨主题查找 LLM 资料的总入口。
- <img src="https://img.shields.io/github/stars/hannibal046/awesome-llm?style=social" height="17" align="texttop"/> [awesome-llm（小写仓库）](https://github.com/hannibal046/awesome-llm): 与上项名称相近的 LLM 资源索引仓库链接，可用于核对维护状态与收录内容；建议访问时以仓库首页的重定向和说明为准。
- <img src="https://img.shields.io/github/stars/RUCAIBox/awesome-llm-pretraining?style=social" height="17" align="texttop"/> [awesome-llm-pretraining](https://github.com/RUCAIBox/awesome-llm-pretraining): 聚焦 LLM 预训练的资源清单，按数据、模型、训练和评测等主题组织论文及项目，为预训练数据工程的研究和选型提供导航。
- <img src="https://img.shields.io/github/stars/OpenDataBox/awesome-data-llm?style=social" height="17" align="texttop"/> [awesome-data-llm](https://github.com/OpenDataBox/awesome-data-llm): 汇总数据与大语言模型交叉领域的论文、数据集和工具，适合从数据管理、数据分析和 LLM 应用多个角度扩展阅读。
- <img src="https://img.shields.io/github/stars/Alfonsobang/awesome-llm-training-data?style=social" height="17" align="texttop"/> [awesome-llm-training-data](https://github.com/Alfonsobang/awesome-llm-training-data): 聚合 LLM 训练数据集、构造方法和相关项目，帮助快速发现预训练、指令微调和偏好对齐任务的公开数据资源。
- <img src="https://img.shields.io/github/stars/luo-junyu/Awesome-Data-Efficient-LLM?style=social" height="17" align="texttop"/> [Awesome-Data-Efficient-LLM](https://github.com/luo-junyu/Awesome-Data-Efficient-LLM): 整理数据高效大模型的论文和资源，关注在有限样本、计算或标注预算下提高训练效果的方法，适合研究数据效率问题。
- <img src="https://img.shields.io/github/stars/zhenlohuang/awesome-chinese-llm?style=social" height="17" align="texttop"/> [awesome-chinese-llm](https://github.com/zhenlohuang/awesome-chinese-llm): 中文大语言模型数据集与模型资料汇总，收录盘古、Qwen、ChatGLM、Baichuan 等国产模型的仓库、论文与数据集入口，适合查找中文语料和中文生态资源。
- <img src="https://img.shields.io/github/stars/luban-agi/Awesome-Domain-LLM?style=social" height="17" align="texttop"/> [Awesome-Domain-LLM](https://github.com/luban-agi/Awesome-Domain-LLM): 垂直领域大模型生态导航，按医疗、法律、金融、教育等领域整理开源模型、训练数据集与评测基准（如 LawBench、FinEval、CBLUE），适合领域模型选型与领域数据调研。
