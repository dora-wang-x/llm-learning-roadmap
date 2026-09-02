# 🚀 llm-learning-roadmap

<p align="center">
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="PRs Welcome">
  <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" alt="License">
  <img src="https://img.shields.io/github/stars/dora-wang-x/llm-learning-roadmap?style=flat-square" alt="Stars">
  <img src="https://img.shields.io/github/forks/dora-wang-x/llm-learning-roadmap?style=flat-square" alt="Forks">
</p>

> 涵盖大语言模型（LLM）从底层原理、数据工程、预训练、对齐微调，到 RAG、Agent、推理部署与安全评估的**全栈学习资源汇总与工程落地路线图**。

---

## 📖 关于本项目 (About)

**llm-learning-roadmap**旨在建立一套符合 **“底层原理 ➔ 数据工程 ➔ 预训练 ➔ 微调 / 对齐 ➔ 推理部署 ➔ 评估 / 安全 ➔ 应用落地”** 工程逻辑的大模型知识图谱与资源索引库。

无论你是刚入行 AI 的开发者、高校研究者，还是寻求落地实践的企业架构师，都可以沿着本项目梳理的路径，系统性地建立大模型知识体系。

### ✨ 项目亮点

- **覆盖完整**：13 个主题章节、**900+ 条**精选资源，从理论到生产全链路打通。
- **工程导向**：按真实研发流程组织目录，而非按论文分类堆砌。
- **中英并重**：兼顾国际前沿（论文 / 官方博客）与中文社区优质内容。
- **持续维护**：每章配有独立 README，可逐章增量更新而不破坏整体结构。

---

## � 目录 (Table of Contents)

- [1. LLM 基础理论与核心原理 (Fundamentals)](#1-llm-基础理论与核心原理-fundamentals)
- [2. 数据工程 (Data Engineering)](#2-数据工程-data-engineering)
- [3. 预训练与基座模型 (Pre-training & Base Models)](#3-预训练与基座模型-pre-training--base-models)
- [4. 微调、对齐与强化学习 (Fine-tuning & Alignment)](#4-微调对齐与强化学习-fine-tuning--alignment)
- [5. 推理加速与工程部署 (Inference & Deployment)](#5-推理加速与工程部署-inference--deployment)
- [6. 模型评估 (LLM Evaluation)](#6-模型评估-llm-evaluation)
- [7. 安全与伦理 (Safety & Ethics)](#7-安全与伦理-safety--ethics)
- [8. 应用开发 (Applications)](#8-应用开发-applications)
  - [8.1 提示词工程 (Prompt Engineering)](#81-提示词工程-prompt-engineering)
  - [8.2 检索增强生成 (RAG)](#82-检索增强生成-rag)
  - [8.3 Agent、Skill 与 MCP](#83-agentskill-与-mcp)
  - [8.4 AI 编程 (AI Coding)](#84-ai-编程-ai-coding)
  - [8.5 Deep Research 深度研究](#85-deep-research-深度研究)
  - [8.6 MaaS 模型即服务](#86-maas-模型即服务)
- [9. 综合资源 (Resources)](#9-综合资源-resources)
- [🛠 目录结构 (Project Structure)](#-目录结构-project-structure)
- [🤝 贡献指南 (Contributing)](#-贡献指南-contributing)
- [📄 开源协议 (License)](#-开源协议-license)

---

## 1. LLM 基础理论与核心原理 (Fundamentals)

从经典 Transformer 到现代 LLM 架构演进的理论基石。

从深度学习与 NLP 前置基础出发，梳理 LLM 核心架构、从零训练与后训练实践，并延伸到工程与应用开发入门。详见 [`01-fundamentals/README.md`](./01-fundamentals/README.md)。

- 前置基础：深度学习、NLP 与 Transformer
- LLM 核心原理与模型架构
- 从零训练与后训练实践
- LLM 工程与应用开发基础
- 扩展主题与持续学习资源

---

## 2. 数据工程 (Data Engineering)

“Data is all you need” —— 决定模型上限的生命线。

覆盖从数据发现、清洗去重、转换标注到质量评估与数据治理的完整流水线，含指令 / 偏好数据与合成数据方向。详见 [`02-data-engineering/README.md`](./02-data-engineering/README.md)。

- 数据发现与采集
- 清洗、去重与过滤
- 转换、标注与格式化
- 质量评估与数据混合
- 指令、偏好与人工反馈数据
- 合成数据与数据扩增
- 数据管道、DataOps 与治理



---

## 3. 预训练与基座模型 (Pre-training & Base Models)

从 Scaling Laws 到大规模分布式训练的基座模型构建。

围绕预训练原理、模型实现、分布式并行、训练效率优化与语料工程展开，并跟踪前沿进展。详见 [`03-pretraining/README.md`](./03-pretraining/README.md)。

- 预训练原理与 Scaling
- 模型实现与单机实验
- 大规模分布式训练
- 训练效率与工程优化
- 语料获取与清洗
- 数据质量、检查与标注


---

## 4. 微调、对齐与强化学习 (Fine-tuning & Alignment)

让基座模型“听话”的关键阶段。

梳理对齐原理综述、SFT 指令微调、RLHF / 偏好优化、安全对齐与前沿方向，含训练框架与工程实践。详见 [`04-alignment/README.md`](./04-alignment/README.md)。

- 对齐原理与综述
- SFT 与指令微调
- RLHF、RLAIF 与偏好优化（PPO / DPO / ORPO / SimPO / KTO）
- 安全对齐
- 前沿方向
- 训练框架与工程实践

---

## 5. 推理加速与工程部署 (Inference & Deployment)

从模型权重到生产服务的最后一公里。

覆盖推理引擎与运行时、性能优化、服务化部署、本地轻量化推理与 LLMOps，含博客教程与工程实践。详见 [`05-inference-deployment/README.md`](./05-inference-deployment/README.md)。

- 推理引擎与运行时
- 推理性能优化
- 服务化与部署架构
- 本地、边缘与轻量化推理
- LLMOps、资源索引与工程实践
- 博客教程与工程实践

---

## 6. 模型评估 (LLM Evaluation)

没有度量就没有改进。

从评测原理综述到框架工具、公开基准、LLM-as-Judge、应用与安全评测、官方云评测服务，系统建立评测知识全景。详见 [`06-llm-evaluation/README.md`](./06-llm-evaluation/README.md)。

- 评测原理与综述
- 评测框架与工具
- 排行榜与公开基准
- LLM-as-Judge 与自动评测
- 应用与安全评测
- 官方平台与云评测服务
- 学习资源与社区导航

---

## 7. 安全与伦理 (Safety & Ethics)

负责任地构建与使用大模型。

本项目体量最大的章节之一，从 Awesome 清单到对齐、越狱攻防、护栏防护、应用安全、多模态安全、伦理与治理、厂商政策、学术跟踪到社区门户，13 个子方向全景覆盖。详见 [`07-safety-ethics/README.md`](./07-safety-ethics/README.md)。

- AI 安全综合资源汇总（Awesome 清单）
- 安全对齐与价值观（Alignment）
- 越狱攻防与红队测试（Jailbreak & Red Teaming）
- 安全护栏与防护工具（Guardrails & Defense）
- LLM 应用安全与威胁情报（OWASP / MITRE / LLMSecOps）
- 多模态安全（MLLM / LVLM Safety）
- 安全评估与基准、伦理与负责任 AI、厂商政策、学术论文、课程、机构与社区

---

## 8. 应用开发 (Applications)

把模型能力转化为真实产品。

本章按应用范式拆分为 6 个子主题，从提示词、RAG、Agent 到 AI 编程、深度研究与 MaaS，覆盖从交互层到服务层的完整应用栈。各子目录均配有独立 README。

### 8.1 提示词工程 (Prompt Engineering)

从 Prompt 延伸到 Context、Harness 与 Loop Engineering，覆盖提示设计、上下文管理、工具编排与循环优化的完整工程链。详见 [`08-applications/8.1-prompt/README.md`](./08-applications/8.1-prompt/README.md)。

- Prompt Engineer / Context Engineer / Harness Engineer / Loop Engineer

### 8.2 检索增强生成 (RAG)

从基础实践到高级方法、文档解析、知识库构建与生产级系统，含研究论文与资源导航。详见 [`08-applications/8.2-rag/README.md`](./08-applications/8.2-rag/README.md)。

- RAG 基础与入门实践 / 标准 RAG 应用开发 / 高级 RAG 方法（GraphRAG、CRAG 等）
- 文档解析与知识库构建 / 生产级 RAG 系统 / RAG 研究论文


### 8.3 Agent、Skill 与 MCP

本项目最大子章节，覆盖 Agent 范式与多智能体、Skill 技能体系与 MCP（模型上下文协议）工具生态。详见 [`08-applications/8.3-agents-skills-mcp/README.md`](./08-applications/8.3-agents-skills-mcp/README.md)。

- **Agent**：ReAct、Plan-and-Solve、Memory 机制、多智能体框架（AutoGen / CrewAI / MetaGPT 等）
- **Skill**：技能定义、封装与复用生态
- **MCP**：模型上下文协议、工具集成与市场

### 8.4 AI 编程 (AI Coding)

从需求规格、编码协作、Skill / 插件集成到代码理解与知识图谱，含学习路径索引。详见 [`08-applications/8.4-ai-coding/README.md`](./08-applications/8.4-ai-coding/README.md)。

- 需求、规格与规划 / 编码协作与代码交付 / Skill、插件与工具集成 / 代码理解、检索与知识图谱 / 学习路径与资源索引

### 8.5 Deep Research 深度研究

按技术架构梳理开源深度研究框架，含 LangGraph 状态机系、RAG 向量检索系、轻量复刻系与相邻方向。详见 [`08-applications/8.5-deepresearch/README.md`](./08-applications/8.5-deepresearch/README.md)。

- LangGraph 状态机系 / RAG + 向量检索系 / 轻量级实现 / 复刻系 / 泛 AI 应用 / 相邻方向

### 8.6 MaaS 模型即服务

聚焦 LLM 网关与模型聚合平台、企业级 AI 应用平台。详见 [`08-applications/8.6-Maas/README.md`](./08-applications/8.6-Maas/README.md)。（

- API 网关与模型聚合 / 企业级 AI 应用平台

---

## 9. 综合资源 (Resources)

跨章节的横向资源集合，含面试、论文、博客与同类项目四个清单，适合系统性补强与横向对照。

| 清单 | 说明 | 条目概览 |
|------|------|----------|
| [`llm-interview.md`](./09-resources/llm-interview.md) | LLM / AI 面试资源 | 90 条，按平台分 12 类（题库、Agent、课程、官方博客、中文社区等） |
| [`paper-list.md`](./09-resources/paper-list.md) | LLM 经典与前沿论文 | 按主题分 10 类（综述、Agent、推理、训练、RAG、高效系统、评测安全、多模态等） |
| [`blog-list.md`](./09-resources/blog-list.md) | 优质博客与站点 | 牛人博客、官方工程博客、中文社区、深度研究站点 4 章 |
| [`similar-projects.md`](./09-resources/similar-projects.md) | 同类 / 可参考开源项目 | 55 个独立项目，按形态分 9 类（Awesome 列表、课程、路线图、从零复现等） |

---


## 🛠 目录结构 (Project Structure)

```text
llm-learning-roadmap/
├── README.md                   # 总览与路线图（本文件）
├── CONTRIBUTING.md             # 贡献规范
├── 01-fundamentals/             # 基础理论与核心原理
├── 02-data-engineering/         # 数据工程
├── 03-pretraining/              # 预训练与基座模型
├── 04-alignment/                # 微调、对齐与强化学习
├── 05-inference-deployment/     # 推理加速与工程部署
├── 06-llm-evaluation/          # 模型评估
├── 07-safety-ethics/           # 安全与伦理
├── 08-applications/             # 应用开发
│   ├── 8.1-prompt/              #   提示词工程
│   ├── 8.2-rag/                 #   检索增强生成
│   ├── 8.3-agents-skills-mcp/   #   Agent、Skill 与 MCP
│   ├── 8.4-ai-coding/           #   AI 编程
│   ├── 8.5-deepresearch/        #   Deep Research 深度研究
│   └── 8.6-Maas/                #   MaaS 模型即服务
└── 09-resources/                # 综合资源（面试 / 论文 / 博客 / 相似项目）
```

> **学习路径建议**：可按目录编号 01→09 顺序系统推进；已有基础者可按需跳读。工程实践导向的同学建议重点研读 `02 数据工程` → `04 对齐` → `05 推理部署` → `08 应用`；研究导向的同学建议重点研读 `01 基础` → `03 预训练` → `06 评测` → `07 安全`。
---

## 🤝 贡献指南 (Contributing)

非常欢迎你为本项目贡献资源或修改建议！在提交 Pull Request 前，请参阅 [CONTRIBUTING.md](./CONTRIBUTING.md) 规范。

- 📌 推荐以 **增量文件（如 `incre.txt`）** 的形式提交新链接，由维护者统一分类落地，避免直接改动各章 README 造成冲突。
- 📝 每条资源请尽量提供：**项目 / 文章名称、链接、40–80 字简介**。
- ✅ GitHub 项目会自动配上 `shields.io` 星标徽章，格式见各章 README。

---

## 📄 开源协议 (License)

本项目采用 [MIT License](./LICENSE) 许可证开源。所收录的第三方资源版权归原作者所有，本仓库仅做索引与导航。
