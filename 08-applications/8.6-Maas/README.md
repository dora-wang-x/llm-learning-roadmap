# 8.6 MaaS（模型即服务）

## 1 API 网关与模型聚合

将多家模型统一为一个 OpenAI 兼容接口，提供协议互转、智能路由、计费与资产管理能力，是 MaaS 编排层的关键基础设施。

- <img src="https://img.shields.io/github/stars/QuantumNous/new-api?style=social" height="17" align="texttop"/> [new-api](https://github.com/QuantumNous/new-api): 下一代 LLM 网关与 AI 资产管理系统，由 QuantumNous 团队维护。支持将 30+ 主流服务商（OpenAI、Claude、Gemini、DeepSeek、Midjourney、Suno 等）聚合为统一接口，提供 OpenAI ↔ Claude / Gemini 协议互转、智能路由、故障切换、精细计费、令牌分组与用户管理，兼容 One API 数据库。适合自建 AI 接口中转站或企业 AI 中台（AGPLv3）。
- [New API 官方文档](https://www.newapi.ai/zh)：new-api 的官方文档站，覆盖安装部署、渠道管理、令牌分发、计费与格式转换的完整说明，是使用与二开 new-api 的权威参考。
- [RixAPI](https://platform.rixapi.com/)：商业 MaaS 聚合平台，持续集成最新 AI 模型（Google Gemini、OpenAI GPT 系列等 300+ 模型），提供统一 API 与按量计费（Input/Output 分别计价），面向开发者与企业提供高性能 AI 基础设施，适合需要免自托管、开箱即用的多模型接入场景。

## 2 企业级 AI 应用平台

开箱即用的全栈 AI 助手 / 知识库平台，覆盖多模型管理、本地 RAG、Agent 编排与搜索问答等能力，可自行托管。

- <img src="https://img.shields.io/github/stars/ageerle/ruoyi-ai?style=social" height="17" align="texttop"/> [ruoyi-ai](https://github.com/ageerle/ruoyi-ai): 企业级 AI 助手平台（若依 AI），基于 Spring Boot 3.5 + Langchain4j + Vue 3 全栈开发。提供多模型管理（DeepSeek/Zhipu/OpenAI 等）、本地 RAG + 向量库（Milvus/Weaviate/Qdrant）、MCP 与 Skills 工具集成、可视化工作流编排与多智能体协作（Supervisor 模式），兼容 Coze/DIFY/FastGPT/RAGFlow，支持 Docker 一键部署（MIT 开源）。
- [PandaRobot 官方文档](https://doc.pandarobot.chat/)：ruoyi-ai 的官方配套文档站，涵盖项目部署、核心功能与二次开发说明，是落地与扩展 ruoyi-ai 的权威参考。
- <img src="https://img.shields.io/github/stars/onyx-dot-app/onyx?style=social" height="17" align="texttop"/> [onyx](https://github.com/onyx-dot-app/onyx): 开源 AI 搜索与助手平台（原 Danswer），定位为「LLM 的应用层」。提供 Agentic RAG（混合索引 + AI Agent）、深度研究、自定义 Agent、网页搜索、代码执行、图像生成等能力，内置 50+ 索引连接器并支持 MCP 扩展。社区版 MIT 许可，可 Docker / Kubernetes / Helm 自托管，也有 Onyx Cloud 免部署选项。
