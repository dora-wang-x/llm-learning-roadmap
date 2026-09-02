# Prompt、Context、Harness 与 Loop Engineering 资源


## 1. Prompt Engineer

### 1.1 基础方法与官方指南

- [ChatGPT Prompting](https://learn.chatgpt.com/docs/prompting)：ChatGPT 官方提示编写指南，介绍目标表达、上下文提供、示例设计和迭代改写方法，适合作为面向通用对话任务的提示设计入门参考。
- [OpenAI Prompt Engineering Guide](https://platform.openai.com/docs/guides/prompt-engineering)：OpenAI 平台的提示工程指南，覆盖消息组织、指令优先级、结构化输出和提示迭代，适合在 API 应用中建立可维护的提示规范。
- [OpenAI Prompt Best Practices](https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-the-openai-api)：OpenAI 帮助中心的提示最佳实践，说明如何清晰描述任务、拆分复杂要求并根据输出进行调整，适合快速排查质量不稳定的问题。
- [OpenAI Using Prompts](https://help.openai.com/en/articles/6654000-using-prompts)：OpenAI 关于提示使用方式的基础说明，帮助理解提示、上下文和模型行为之间的关系，为后续的实验与生产化设计建立共同术语。
- [OpenAI GPT-4.1 Prompting Guide](https://developers.openai.com/cookbook/examples/gpt4-1_prompting_guide)：OpenAI Cookbook 中面向 GPT-4.1 的提示指南，给出指令层级、工具调用与输出控制的具体模式，便于直接迁移到应用代码。

### 1.2 课程、书籍与学习路径
- <img src="https://img.shields.io/github/stars/anthropics/prompt-eng-interactive-tutorial?style=social" height="17" align="texttop"/> [prompt-eng-interactive-tutorial](https://github.com/anthropics/prompt-eng-interactive-tutorial): Anthropic 的交互式提示工程教程，以练习形式讲解清晰指令、示例和输出格式控制，帮助开发者理解每项提示改动对模型行为的影响。
- <img src="https://img.shields.io/github/stars/microsoft/generative-ai-for-beginners?style=social" height="17" align="texttop"/> [generative-ai-for-beginners](https://github.com/microsoft/generative-ai-for-beginners): 面向初学者的生成式 AI 课程，结合代码练习讲解提示设计、模型调用、应用开发和安全实践，适合建立从概念到实现的完整基础。
- <img src="https://img.shields.io/github/stars/datawhalechina/ai-prompting-for-everyone?style=social" height="17" align="texttop"/> [ai-prompting-for-everyone](https://github.com/datawhalechina/ai-prompting-for-everyone): Datawhale 编写的中文提示工程课程，围绕任务拆解、角色设定、约束表达和结果校验展开，适合非技术与技术读者共同学习。
- [AI Prompting for Everyone 文档](https://datawhalechina.github.io/ai-prompting-for-everyone)：配套在线课程文档，以中文系统说明提示设计的基础原则和案例，可作为 Datawhale 开源课程的网页阅读入口和持续更新版本。
- [AI Prompting for Everyone](https://www.deeplearning.ai/courses/ai-prompting-for-everyone)：DeepLearning.AI 的通识课程，解释如何在工作与学习中使用提示完成分析、创作与决策任务，强调可靠沟通而非特定模型技巧。
- [ChatGPT Prompt Engineering for Developers](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers)：DeepLearning.AI 面向开发者的短课程，通过代码示例讲解提示原则、文本转换、摘要与扩展任务，适合快速掌握 API 场景的实践方式。
- [ChatGPT Prompt Engineering](https://www.deeplearning.ai/courses/chatgpt-prompt-eng)：DeepLearning.AI 的提示工程课程页面，集中介绍 ChatGPT 的任务表达和迭代策略，可作为学习路径和课程材料的官方入口。

### 1.3 实战教程与开发者手册
- [Prompt Engineering Guide 中文版](https://www.promptingguide.ai/zh)：Prompt Engineering Guide 的中文站点，涵盖零样本、少样本、思维链与安全提示等主题，适合按知识图谱系统查阅方法和论文。
- [Prompt Guide 基础教程](https://prompt-guide.xiniushu.com/category/-basics)：中文提示工程基础教程，按概念和案例组织常见的指令写法与调试思路，适合作为短篇、可检索的日常学习资料。
- [Claude Code Overview](https://code.claude.com/docs/en/overview)：Claude Code 官方概览，说明代码智能体的交互模型、项目上下文和执行边界，适合理解面向软件工程任务的提示协作方式。
- <img src="https://img.shields.io/github/stars/lintsinghua/claude-code-book?style=social" height="17" align="texttop"/> [claude-code-book](https://github.com/lintsinghua/claude-code-book): 面向 Claude Code 的中文实践手册，讲解提示编写、项目协作与代码智能体使用方式，适合将通用提示技巧落到真实仓库工作流。
- [Hermes Agent 教程](https://www.runoob.com/hermes-agent/hermes-agent-tutorial.html)：菜鸟教程提供的 Hermes Agent 入门内容，介绍智能体配置、提示和工具执行流程，适合快速了解带工具调用的对话应用开发。

### 1.4 提示模式与结构化设计

- <img src="https://img.shields.io/github/stars/dair-ai/Prompt-Engineering-Guide?style=social" height="17" align="texttop"/> [Prompt-Engineering-Guide](https://github.com/dair-ai/Prompt-Engineering-Guide): 系统整理提示工程概念、方法、论文和实践案例，覆盖推理、检索、智能体等场景，是构建团队提示知识库的重要参考。
- <img src="https://img.shields.io/github/stars/NirDiamant/prompt_engineering?style=social" height="17" align="texttop"/> [prompt_engineering](https://github.com/NirDiamant/prompt_engineering): 通过可运行示例展示结构化输出、少样本提示和复杂任务编排，便于开发者修改参数并观察提示策略在不同任务中的效果。
- <img src="https://img.shields.io/github/stars/phodal/prompt-patterns?style=social" height="17" align="texttop"/> [prompt-patterns](https://github.com/phodal/prompt-patterns): 以模式语言总结常见提示结构，为需求分析、角色设定和输出约束提供可复用模板，帮助团队形成一致且可审查的提示写法。
- <img src="https://img.shields.io/github/stars/langgptai/wonderful-prompts?style=social" height="17" align="texttop"/> [wonderful-prompts](https://github.com/langgptai/wonderful-prompts): 提供结构化中文提示词模板，强调角色、目标、约束和工作流的组合设计，便于快速构造稳定的任务指令。
- <img src="https://img.shields.io/github/stars/brexhq/prompt-engineering?style=social" height="17" align="texttop"/> [prompt-engineering](https://github.com/brexhq/prompt-engineering): 分享企业级提示工程规范与实践，关注一致性、可维护性和生产环境中的提示管理，适合团队协作落地与建立版本化改进流程。
- <img src="https://img.shields.io/github/stars/asgeirtj/system_prompts_leaks?style=social" height="17" align="texttop"/> [system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks): 收录 ChatGPT、Claude、Gemini、Grok、Copilot 等主流 AI 产品泄露的系统提示词（逐字保留），覆盖多厂商多版本，可作为研究生产级系统提示词结构、工具定义与安全约束设计的真实案例参考（注：使用时注意知识产权与合规，宜作学习参考而非直接复制）。

### 1.5 提示词库、社区资源

- <img src="https://img.shields.io/github/stars/snwfdhmp/awesome-gpt-prompt-engineering?style=social" height="17" align="texttop"/> [awesome-gpt-prompt-engineering](https://github.com/snwfdhmp/awesome-gpt-prompt-engineering): 汇集 GPT 提示工程文章、工具、方法和案例，可快速查找不同任务的提示思路，并用于比较常见实践方案的适用范围。
- <img src="https://img.shields.io/github/stars/promptslab/Awesome-Prompt-Engineering?style=social" height="17" align="texttop"/> [Awesome-Prompt-Engineering](https://github.com/promptslab/Awesome-Prompt-Engineering): 聚合提示工程论文、框架、数据集和应用资源，涵盖文本生成、推理与智能体场景，适合研究选题梳理和工程工具选型。
- <img src="https://img.shields.io/github/stars/oxbshw/Prompt-Engineering-Guide?style=social" height="17" align="texttop"/> [Prompt-Engineering-Guide](https://github.com/oxbshw/Prompt-Engineering-Guide): 汇总提示工程知识、模板与实践文章，提供从基础概念到应用技巧的学习路径，适合作为中文读者的提示资料导航入口。
- <img src="https://img.shields.io/github/stars/lathashree01/prompt-engineering-guides?style=social" height="17" align="texttop"/> [prompt-engineering-guides](https://github.com/lathashree01/prompt-engineering-guides): 按主题整理提示工程指南和示例，帮助开发者理解不同提示模式的使用边界，并建立从基础学习到实际应用的实践路线。
- <img src="https://img.shields.io/github/stars/ai-boost/awesome-prompts?style=social" height="17" align="texttop"/> [awesome-prompts](https://github.com/ai-boost/awesome-prompts): 收集写作、编程、分析和创作任务的高质量提示词与资源，可作为日常工作流的模板起点，并用于快速比较不同表达方式。
- <img src="https://img.shields.io/github/stars/f/awesome-chatgpt-prompts?style=social" height="17" align="texttop"/> [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts): 经典 ChatGPT 角色提示词集合，展示如何结合角色、目标和约束构造任务提示，适合提炼为个人或团队的提示模板。
- <img src="https://img.shields.io/github/stars/f/prompts.chat?style=social" height="17" align="texttop"/> [prompts.chat](https://github.com/f/prompts.chat): 由 awesome-chatgpt-prompts 作者构建的开源提示词平台（前身即 awesome-chatgpt-prompts），含提示词库、25+ 章交互式提示工程书籍、自托管部署与 MCP/CLI/Claude Code 插件集成，适合作为团队提示资产库的工程化起点。
- <img src="https://img.shields.io/github/stars/PlexPt/awesome-chatgpt-prompts-zh?style=social" height="17" align="texttop"/> [awesome-chatgpt-prompts-zh](https://github.com/PlexPt/awesome-chatgpt-prompts-zh): 面向中文用户整理 ChatGPT 角色提示词，覆盖办公、学习、编程和内容创作场景，可直接改写为适应本地任务的初始模板。
- <img src="https://img.shields.io/github/stars/K-Render/best-chinese-prompt?style=social" height="17" align="texttop"/> [best-chinese-prompt](https://github.com/K-Render/best-chinese-prompt): 精选中文提示词和使用示例，帮助改进任务表达、角色定义与目标描述，覆盖多种常见办公和创作应用场景。
- <img src="https://img.shields.io/github/stars/madhavbuilds/awesome-ai-universe?style=social" height="17" align="texttop"/> [awesome-ai-universe](https://github.com/madhavbuilds/awesome-ai-universe): 汇总生成式 AI 工具、提示资源和应用项目，为探索提示驱动产品实践提供入口，便于发现可以直接试用的方案。
- [LangSmith Hub](https://smith.langchain.com/hub)：LangSmith 的提示资产中心，支持查找、复用和版本化管理公开提示，适合团队沉淀模板并把提示资产与评测流程关联。
- [FlowGPT](https://flowgpt.com/zh-CN)：面向中文用户的提示分享社区，聚合不同模型和任务场景的提示模板，适合获得表达灵感，但应在生产使用前自行验证效果。
- [PromptPort](https://promptport.ai)：提示词资源与管理平台，帮助浏览和组织可复用提示资产，适合作为构建个人提示库和探索不同任务模板的辅助入口。
- [PromptHero](https://prompthero.com)：以图像与生成式创作为主的提示搜索平台，适合观察描述方式、风格词和参数组合如何影响生成结果，并沉淀视觉生成模板。

- [提示工程实践一](https://zhuanlan.zhihu.com/p/686139236)：中文提示工程实践文章，围绕任务描述、角色设定和输出约束梳理常用写法，适合结合具体业务需求理解提示迭代的思考过程。
- [提示工程实践二](https://zhuanlan.zhihu.com/p/687416466)：中文提示工程实践文章，补充提示构造和模型交互中的常见问题，适合在阅读模板资源后进一步建立问题拆解与调试意识。

### 1.6 优化、版本与评测

- <img src="https://img.shields.io/github/stars/malteos/awesome-prompt-optimization?style=social" height="17" align="texttop"/> [awesome-prompt-optimization](https://github.com/malteos/awesome-prompt-optimization): 收集自动提示优化、提示搜索和基于反馈改写提示的论文、工具与实现，支持系统比较不同优化策略的效果与成本。
- <img src="https://img.shields.io/github/stars/openai/evals?style=social" height="17" align="texttop"/> [evals](https://github.com/openai/evals): OpenAI 的模型评测框架，可编写自定义基准比较提示、模型和应用输出质量，适用于将提示调整纳入可重复的持续验证流程。
- <img src="https://img.shields.io/github/stars/benchflow-ai/awesome-evals?style=social" height="17" align="texttop"/> [awesome-evals](https://github.com/benchflow-ai/awesome-evals): 汇集大模型评测框架、数据集和观测工具，覆盖离线与在线评估场景，为提示迭代和应用质量验证提供选型参考。
- <img src="https://img.shields.io/github/stars/EleutherAI/lm-evaluation-harness?style=social" height="17" align="texttop"/> [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness): 通用语言模型评测工具，提供标准基准、批量推理和可复现实验能力，适合横向比较模型、模板和推理配置。
- <img src="https://img.shields.io/github/stars/openai/openai-cookbook?style=social" height="17" align="texttop"/> [OpenAI Tools Evaluation Notebook](https://github.com/openai/openai-cookbook/blob/main/examples/evaluation/use-cases/tools-evaluation.ipynb): OpenAI Cookbook 的工具调用评测示例，展示如何构造用例、定义评分指标并分析失败路径，适合完善带工具提示的测试集。

### 1.7 专项提示应用工具

- [PromptPerfect](https://promptperfect.jina.ai)：在线提示优化工具，帮助针对目标模型重写和扩展初始指令，可用于快速产生对照方案，但需通过独立评测确认改写收益。
- [FlowGPT Prompt Enhancer](https://flowgpt.com/zh-CN/p/promptenhancer)：FlowGPT 提供的提示增强器，用于将简短需求扩展为更具体的任务描述，适合生成候选提示，但不替代领域约束与回归测试。
- [Midjourney Prompt Helper](https://promptfolder.com/midjourney-prompt-helper)：面向 Midjourney 的提示构建工具，以可选参数组织主体、风格和构图描述，适合快速学习视觉生成提示的结构化表达。
- [img2prompt](https://replicate.com/methexis-inc/img2prompt)：Replicate 上的图像转提示模型，可从参考图片生成描述性提示文本，适合视觉创作场景的反向提示探索与灵感采集。

## 2. Context Engineer

### 2.1 上下文设计与构建

- <img src="https://img.shields.io/github/stars/mlnjsh/context-engineering?style=social" height="17" align="texttop"/> [context-engineering](https://github.com/mlnjsh/context-engineering): 汇总上下文工程概念、论文和实践方法，关注信息选择、组织以及上下文窗口管理，适合设计复杂智能体的输入构建策略。
- [Anthropic Effective Context Engineering](https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents)：Anthropic 关于智能体上下文工程的实践文章，讨论任务状态、工具结果和记忆的取舍，为长任务中的信息编排提供原则。
- [Gemini Long Context](https://ai.google.dev/gemini-api/docs/long-context)：Google Gemini 的长上下文官方文档，说明长输入的能力、限制和使用模式，适合设计大文档分析或多轮任务的上下文策略。
- [OpenAI Context Personalization](https://developers.openai.com/cookbook/examples/agents_sdk/context_personalization)：OpenAI Agents SDK 的上下文个性化示例，展示如何为不同用户与任务注入相关信息，同时避免将无关历史带入模型输入。
- [Production-ready Context Engineering](https://guidesfor.dev/context-engineering-guide/production-ready-context-best-practices)：面向生产环境的上下文工程指南，讨论上下文边界、质量控制和可观测性，适合将原型中的提示拼接升级为可维护的流程。
- [Context Engineering Book](https://augmentedadvisors.com/downloads/context-engineering-book.pdf)：上下文工程电子书，系统讨论信息选择、压缩、记忆和检索等策略，适合在构建复杂智能体前建立方法论框架。
- [Context Engineering in LLM-based Agents](https://jtanruan.medium.com/context-engineering-in-llm-based-agents-d670d6b439bc)：关于 LLM 智能体上下文工程的实践文章，解释上下文构成、状态维护和信息筛选方式，适合结合实际 Agent 流程阅读。
- [What Is Context Engineering for LLMs](https://medium.com/@tahirbalarabe2/%EF%B8%8F-what-is-context-engineering-for-llms-90109f856c1c)：介绍 LLM 上下文工程基本定义和常见组件的文章，适合初步理解它与单次提示设计的差别及其在应用系统中的位置。
- [Beyond Prompting: Context Engineering](https://towardsdatascience.com/beyond-prompting-the-power-of-context-engineering)：从提示工程延展到上下文工程的概念文章，强调外部知识、会话状态和任务信息对模型表现的共同作用。

### 2.2 检索、记忆与上下文优化

- [Anthropic Contextual Retrieval](https://www.anthropic.com/engineering/contextual-retrieval)：Anthropic 提出的上下文化检索实践，说明如何在嵌入和检索前补充文档语境，以减少分块脱离原文造成的召回歧义。
- [FlowHunt Context Engineering](https://www.flowhunt.io/blog/context-engineering-ai-agents-token-optimization)：聚焦智能体 Token 优化的上下文工程文章，讨论精简历史、摘要和选择性注入信息的策略，适合评估成本与质量平衡。
- [LLM Context Engineering: A Practical Guide](https://medium.com/the-low-end-disruptor/llm-context-engineering-a-practical-guide-248095d4bf71)：上下文工程实践指南，围绕提示之外的检索、记忆和状态设计展开，帮助识别导致模型输出不稳定的上下文问题。
- [Enhance LLMs with Context Engineering](https://towardsdatascience.com/how-to-significantly-enhance-llms-by-leveraging-context-engineering-2)：讨论如何利用上下文工程提升 LLM 效果的文章，侧重检索与信息组织的实践思路，适合用来补充方案设计视角。
- [OpenAI Cookbook](https://developers.openai.com/cookbook)：OpenAI 官方示例库，覆盖提示、检索、评测、工具调用和智能体应用，可按具体问题查找可运行实现并改造成自己的工程组件。

### 2.3 学习路径与资源索引

- <img src="https://img.shields.io/github/stars/yzfly/awesome-context-engineering?style=social" height="17" align="texttop"/> [awesome-context-engineering](https://github.com/yzfly/awesome-context-engineering): 整理上下文工程文章、工具和案例，覆盖检索、记忆、压缩与智能体上下文构建，强调信息质量、上下文预算和成本控制。
- <img src="https://img.shields.io/github/stars/datawhalechina/prompt-engineering-for-developers?style=social" height="17" align="texttop"/> [prompt-engineering-for-developers](https://github.com/datawhalechina/prompt-engineering-for-developers): 面向开发者的中文课程，介绍上下文注入、文档问答和可控输出等应用技术，并配有 API 调用示例，适合从提示走向应用集成。

## 3. Harness Engineer

### 3.1 Harness 架构、边界与交互契约

- <img src="https://img.shields.io/github/stars/ovmap/harness-engineering?style=social" height="17" align="texttop"/> [harness-engineering](https://github.com/ovmap/harness-engineering): 探索智能体 Harness 的架构实现，关注工具编排、任务边界和长期运行可靠性，适合研究如何把模型能力封装为稳定的服务。
- <img src="https://img.shields.io/github/stars/lopopolo/harness-engineering?style=social" height="17" align="texttop"/> [harness-engineering](https://github.com/lopopolo/harness-engineering): 记录构建编码智能体 Harness 的工程经验，涉及环境隔离、反馈机制和失败恢复，适合参考面向实际软件仓库的执行控制设计。
- <img src="https://img.shields.io/github/stars/keyuchen21/agentic-engineering-handbook?style=social" height="17" align="texttop"/> [agentic-engineering-handbook](https://github.com/keyuchen21/agentic-engineering-handbook): 提供智能体工程手册，覆盖 Harness、工具、评测和部署等生产化环节，帮助团队建立代码智能体的交付规范与协作流程。
- [Anthropic Harness Design for Long-running Apps](https://www.anthropic.com/engineering/harness-design-long-running-apps)：Anthropic 关于长运行应用 Harness 设计的文章，讨论执行环境、状态保存和恢复策略，为持续运行的智能体提供架构参考。

### 3.2 执行运行时、SDK 与交付集成

- <img src="https://img.shields.io/github/stars/HKUDS/OpenHarness?style=social" height="17" align="texttop"/> [OpenHarness](https://github.com/HKUDS/OpenHarness): 面向智能体的开源 Harness 框架，围绕任务执行、工具协作和运行环境提供工程化能力，适合研究和搭建可扩展、可复现实验的智能体系统。
- <img src="https://img.shields.io/github/stars/browser-use/browser-harness?style=social" height="17" align="texttop"/> [browser-harness](https://github.com/browser-use/browser-harness): 为浏览器智能体提供可控执行环境与评测支撑，帮助管理网页交互、任务状态和结果反馈，适合构建可靠的 Web 自动化智能体工作流。
- <img src="https://img.shields.io/github/stars/strands-agents/harness-sdk?style=social" height="17" align="texttop"/> [harness-sdk](https://github.com/strands-agents/harness-sdk): Strands Agents 的 Harness SDK，提供构建和运行智能体 Harness 的开发接口，适合将工具、上下文、状态和执行约束整合到应用代码中。
- <img src="https://img.shields.io/github/stars/deepseek-ai/deepseek-harness?style=social" height="17" align="texttop"/> [deepseek-harness](https://github.com/deepseek-ai/deepseek-harness): DeepSeek 提供的智能体 Harness 项目，面向代码与任务执行场景组织运行环境和交互流程，适合研究可复现的智能体工程实现。
- <img src="https://img.shields.io/github/stars/harness/harness?style=social" height="17" align="texttop"/> [harness](https://github.com/harness/harness): 持续交付与工程自动化平台，提供构建、部署和治理能力，适合将智能体应用纳入标准化的软件交付、环境管理和运维流程。

### 3.3 可靠性、长任务运行与治理

- [Anthropic Effective Harnesses](https://www.anthropic.com/engineering/effective-harnesses-for-long-running-agents)：Anthropic 介绍长运行智能体有效 Harness 的文章，聚焦任务分解、可观测性、持久化状态和失败处理，适合生产系统设计评审。
- [Anthropic Managed Agents](https://www.anthropic.com/engineering/managed-agents)：Anthropic 对托管智能体运行方式的工程说明，涉及协调、执行边界和运维考虑，适合了解长期任务的服务化管理模式。
- <img src="https://img.shields.io/github/stars/RasaHQ/why-agents-fails?style=social" height="17" align="texttop"/> [why-agents-fails](https://github.com/RasaHQ/why-agents-fails): 总结智能体常见失败模式及根因，帮助工程师通过约束、监控和测试改进 Harness 设计，并为故障复盘提供系统化视角。
- [OpenAI Agentic Governance Cookbook](https://developers.openai.com/cookbook/examples/partners/agentic_governance_guide/agentic_governance_cookbook)：OpenAI 的智能体治理示例，说明如何设计监督、审计和风险控制机制，适合把安全与合规要求纳入工具调用和任务执行过程。

### 3.4 学习路径、社区与资料索引

- <img src="https://img.shields.io/github/stars/walkinglabs/awesome-harness-engineering?style=social" height="17" align="texttop"/> [awesome-harness-engineering](https://github.com/walkinglabs/awesome-harness-engineering): 汇集 Harness Engineering 概念、文章和项目，关注为智能体搭建可靠运行环境，帮助理解工具、状态与执行边界的系统设计。
- <img src="https://img.shields.io/github/stars/apollowald/awesome-harness-engineering?style=social" height="17" align="texttop"/> [awesome-harness-engineering](https://github.com/apollowald/awesome-harness-engineering): 聚合智能体 Harness 设计资料，涵盖工具接口、状态、权限和执行约束等主题，适合为生产智能体建立工程设计检查项。
- <img src="https://img.shields.io/github/stars/Jiaaqiliu/Awesome-Harness-Engineering?style=social" height="17" align="texttop"/> [Awesome-Harness-Engineering](https://github.com/Jiaaqiliu/Awesome-Harness-Engineering): 整理 Harness Engineering 论文和案例，帮助构建可观测、可恢复的智能体工作空间，并将工具调用与状态管理纳入统一架构。
- <img src="https://img.shields.io/github/stars/ai-boost/awesome-harness-engineering?style=social" height="17" align="texttop"/> [awesome-harness-engineering](https://github.com/ai-boost/awesome-harness-engineering): 收录 Harness 工程学习资料与实践链接，侧重编码智能体和生产系统集成，涵盖环境、工具、治理和部署等关键环节。
- <img src="https://img.shields.io/github/stars/jpcmf/learn-harness-engineering?style=social" height="17" align="texttop"/> [learn-harness-engineering](https://github.com/jpcmf/learn-harness-engineering): 面向学习者讲解 Harness Engineering 的基本组成、设计原则和智能体工程实践，适合在搭建首个可执行智能体系统前建立整体认知。
- <img src="https://img.shields.io/github/stars/walkinglabs/learn-harness-engineering?style=social" height="17" align="texttop"/> [learn-harness-engineering](https://github.com/walkinglabs/learn-harness-engineering): 面向实践者的 Harness Engineering 学习仓库，组织概念、案例与实现路径，适合循序掌握智能体运行环境、工具接入和可靠性设计。
- [Harness Engineering Course](https://harnesscourse.com)：围绕智能体 Harness 设计的在线课程资源，覆盖运行环境、工具接入和可靠性等内容，适合以课程化方式建立工程知识框架。
- [Harness Engineering Masterclass](https://www.udemy.com/course/harness-engineering-masterclass-ai-coding-agents)：面向 AI 编程智能体的 Harness 工程课程，介绍运行环境、任务编排和质量控制等主题，适合需要系统练习的开发者。

## 4. Loop Engineer

### 4.1 社区资源与项目索引

- <img src="https://img.shields.io/github/stars/cobusgreyling/loop-engineering?style=social" height="17" align="texttop"/> [loop-engineering](https://github.com/cobusgreyling/loop-engineering): 聚焦 Loop Engineering 方法论，讨论智能体如何通过计划、执行、观察和反馈持续完成任务，适合设计可迭代的自主工作流。
- <img src="https://img.shields.io/github/stars/invincible04/awesome-loop-engineering?style=social" height="17" align="texttop"/> [awesome-loop-engineering](https://github.com/invincible04/awesome-loop-engineering): 汇总循环式智能体论文、框架和工程案例，覆盖反馈、重试和状态推进机制，便于设计闭环任务执行器和改进策略。
- <img src="https://img.shields.io/github/stars/rudy2steiner/awesome-agent-loops?style=social" height="17" align="texttop"/> [awesome-agent-loops](https://github.com/rudy2steiner/awesome-agent-loops): 收集智能体循环与状态管理案例，包含记忆、工具结果和历史上下文的组织方法，帮助构建可持续执行的多步骤流程。
- <img src="https://img.shields.io/github/stars/spinningideas/resources?style=social" height="17" align="texttop"/> [AI-Agent-Loop-Engineering Wiki](https://github.com/spinningideas/resources/wiki/AI-Agent-Loop-Engineering): 以 Wiki 形式收录 AI Agent Loop Engineering 资源，围绕循环设计、执行反馈与工程实践整理链接，适合快速浏览该领域的概念和实现入口。
- [Loop Engineering Topic](https://github.com/topics/loop-engineering)：GitHub 上按 loop-engineering 主题聚合的项目导航页，可用于发现新出现的循环编排、任务反思和智能体状态管理实现。
- [EveryDev Loop Engineering](https://www.everydev.ai/tools/loop-engineering)：EveryDev 收录的 Loop Engineering 工具页面，提供相关产品和实践资源入口，适合在调研阶段了解现有工作流编排方案。

### 4.2 书籍、指南与方法论

- [Prompt, Context, Harness, Loop](https://azureauthority.in/prompt-context-harness-loop-the-four-layers-of-engineering-reliable-ai-agents)：从 Prompt、Context、Harness 和 Loop 四层解释可靠智能体工程的文章，适合用于对齐团队角色分工并识别系统设计中的缺失层次。
