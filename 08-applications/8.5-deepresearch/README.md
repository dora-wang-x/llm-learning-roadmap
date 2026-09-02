# 8.5 Deep Research 深度研究


## 1. LangGraph 状态机系
- <img src="https://img.shields.io/github/stars/bytedance/deer-flow?style=social" height="17" align="texttop"/> [deer-flow](https://github.com/bytedance/deer-flow): 字节跳动开源的社区化深度研究框架，基于 LangGraph 编排多智能体协作，集成搜索、爬取、写作全流程并支持人机交互修正，功能完整度在开源方案中领先。
- <img src="https://img.shields.io/github/stars/google-gemini/gemini-fullstack-langgraph-quickstart?style=social" height="17" align="texttop"/> [gemini-fullstack-langgraph-quickstart](https://github.com/google-gemini/gemini-fullstack-langgraph-quickstart): Google 官方 Gemini 团队出品的全栈模板，前端 Next.js + 后端 LangGraph，演示如何用 Gemini 模型构建多步骤研究 Agent，适合作为官方起步骨架快速二次开发。
- <img src="https://img.shields.io/github/stars/langchain-ai/open_deep_research?style=social" height="17" align="texttop"/> [open_deep_research](https://github.com/langchain-ai/open_deep_research): LangChain 官方深度研究参考实现，定义了"规划-检索-合成-反思"的标准研究循环，是学习 LangGraph 多步 Agent 编排与状态机设计的首选样板。
- <img src="https://img.shields.io/github/stars/nickscamara/open-deep-research?style=social" height="17" align="texttop"/> [open-deep-research](https://github.com/nickscamara/open-deep-research): LangChain 生态下的轻量研究智能体，采用 smolagents 实现思路，代码精简，适合快速理解 LangGraph 状态机如何驱动研究循环，可与官方版对照学习。

## 2. RAG + 向量检索系

- <img src="https://img.shields.io/github/stars/zilliztech/deep-searcher?style=social" height="17" align="texttop"/> [deep-searcher](https://github.com/zilliztech/deep-searcher): Zilliz（Milvus 出品方）开源的 agentic RAG 框架，面向私有数据深度检索，支持查询路由、上下文聚合与多源知识融合，适合企业内部知识库的精准问答与研究场景。

## 3. 轻量级实现 / 复刻系

- <img src="https://img.shields.io/github/stars/dzhng/deep-research?style=social" height="17" align="texttop"/> [deep-research](https://github.com/dzhng/deep-research): 极简 CLI 复刻版，GPT + Jina 搜索组合，核心逻辑约百行，是最小可行的 Deep Research 实现，源码精读入门首选，便于理解研究循环本质。
- <img src="https://img.shields.io/github/stars/jina-ai/node-DeepResearch?style=social" height="17" align="texttop"/> [node-DeepResearch](https://github.com/jina-ai/node-DeepResearch): Jina AI 出品的 Node.js 复刻实现，结合 Jina 搜索/读取 API，演示前端友好的流式输出与进度展示，可作 TypeScript 栈对照学习参考。
- <img src="https://img.shields.io/github/stars/mshumer/OpenDeepResearcher?style=social" height="17" align="texttop"/> [OpenDeepResearcher](https://github.com/mshumer/OpenDeepResearcher): 强调并行子任务拆分与异步调度，将研究问题分解为多路并发检索再聚合结果，架构设计对处理复杂长尾问题与缩短研究耗时具有参考价值。
- <img src="https://img.shields.io/github/stars/btahir/open-deep-research?style=social" height="17" align="texttop"/> [open-deep-research](https://github.com/btahir/open-deep-research): Next.js 全栈开箱即用版本，自带可视化界面与实时研究进度，部署即用，适合快速体验 Deep Research 的产品形态与交互设计。

## 4. 泛 AI 应用 / 相邻方向
- <img src="https://img.shields.io/github/stars/volcengine/ai-app-lab?style=social" height="17" align="texttop"/> [ai-app-lab](https://github.com/volcengine/ai-app-lab): 火山方舟 AI 应用实验室，集合多类智能体应用示例与工程化脚手架，可作 Deep Research 落地生产环境时的工程参考与最佳实践来源。
- <img src="https://img.shields.io/github/stars/ruc-datalab/DeepAnalyze?style=social" height="17" align="texttop"/> [DeepAnalyze](https://github.com/ruc-datalab/DeepAnalyze): 中国人民大学团队出品的深度数据分析智能体，同样基于 agentic 工作流，但聚焦数据分析与可视化，与 Deep Research 形成"研究 vs 分析"的对照参考。
- <img src="https://img.shields.io/github/stars/deepchecks/deepchecks?style=social" height="17" align="texttop"/> [deepchecks](https://github.com/deepchecks/deepchecks): ML 模型测试与验证库，覆盖数据完整性检查、分布漂移检测、性能回归测试等，与 Deep Research 主题不同，作为模型质量保障工具列入延伸阅读，可按需移至评测章节。
