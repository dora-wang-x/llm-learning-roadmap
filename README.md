# 🚀 llm-learning-roadmap

<p align="center">
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="PRs Welcome">
  <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" alt="License">
  <img src="https://img.shields.io/github/stars/dora-wang-x/llm-learning-roadmap-Path?style=flat-square" alt="Stars">
  <img src="https://img.shields.io/github/forks/dora-wang-x/llm-learning-roadmap-Path?style=flat-square" alt="Forks">
</p>

> 涵盖大语言模型（LLM）从底层原理、数据工程、训练微调到 RAG、Agent 及工程落地的全栈学习资源汇总。

---

## 📖 关于本项目 (About)

**Awesome-LLM-Learning-Path** 旨在建立一个符合 **“底层原理 ➔ 数据工程 ➔ 预训练 ➔ 微调/对齐 ➔ 能力扩展/Skill ➔ RAG ➔ Agent ➔ 推理/部署”** 工程落地逻辑的大模型知识图谱与资源索引库。

无论你是刚入行 AI 的开发者、高校研究者，还是寻求落地实践的企业架构师，都可以通过本项目建立系统的大模型知识体系。

---

## 📑 目录 (Table of Contents)

- [1. LLM 基础理论与核心原理 (Fundamentals)](#1-llm-基础理论与核心原理-fundamentals)
- [2. 数据工程 (Data Engineering)](#2-数据工程-data-engineering)
- [3. 预训练与基座模型 (Pre-training & Base Models)](#3-预训练与基座模型-pre-training--base-models)
- [4. 微调、对齐与强化学习 (Fine-tuning & Alignment)](#4-微调对齐与强化学习-fine-tuning--alignment)
- [5. 模型能力扩展与 Skill (Model Skills & Capabilities)](#5-模型能力扩展与-skill-model-skills--capabilities)
- [6. 检索增强生成 (RAG & Knowledge Integration)](#6-检索增强生成-rag--knowledge-integration)
- [7. LLM Agent & 应用开发 (Agents & Applications)](#7-llm-agent--应用开发-agents--applications)
- [8. 推理加速与工程部署 (Inference & Deployment)](#8-推理加速与工程部署-inference--deployment)
- [9. 模型评估、安全与红队测试 (Evaluation & Safety)](#9-模型评估安全与红队测试-evaluation--safety)
- [🛠 常用工具库推荐 (Awesome Tools)](#-常用工具库推荐-awesome-tools)
- [🤝 贡献指南 (Contributing)](#-贡献指南-contributing)
- [📄 开源协议 (License)](#-开源协议-license)

---

## 1. LLM 基础理论与核心原理 (Fundamentals)

*从经典 Transformer 到现代 LLM 架构演进的理论基石。*

### 核心论文 (Key Papers)
- **Attention Is All You Need** (Vaswani et al., 2017) [[Paper]](https://arxiv.org/abs/1706.03762)
- **RoFormer: Enhanced Transformer with Rotary Position Embedding** (Su et al., 2021) [[Paper]](https://arxiv.org/abs/2104.09864)
- **LLaMA: Open and Efficient Foundation Language Models** (Touvron et al., 2023) [[Paper]](https://arxiv.org/abs/2302.13971)
- **DeepSeek-V3 Technical Report** (DeepSeek, 2024) [[Paper]](https://github.com/deepseek-ai/DeepSeek-V3)

### 优质课程 (Courses & Tutorials)
- **Stanford CS224N**: NLP with Deep Learning [[Course]](https://web.stanford.edu/class/cs224n/)
- **Andrej Karpathy**: Neural Networks: Zero to Hero [[YouTube]](https://www.youtube.com/playlist?list=PLAqh184XbH8eK4hBUbf-5eddSkGLwah8I)

---

## 2. 数据工程 (Data Engineering)

*“Data is all you need” —— 决定模型上限的生命线。*

- **预训练数据处理**：去重（MinHash / Deduplication）、质量过滤、Tokenizer 训练（BPE, WordPiece）。
- **SFT 数据构造**：Self-Instruct、Evol-Instruct、多轮对话构建与过滤。
- **开源数据集**：
  - [FineWeb](https://huggingface.co/spaces/HuggingFaceFW/blogpost-fineweb) - 15T+ 高质量英文 Web 数据集
  - [UltraFeedback](https://huggingface.co/datasets/openbmb/UltraFeedback) - 大规模偏好对齐数据集

---

## 3. 预训练与基座模型 (Pre-training & Base Models)

- **分布式并行**：DP, TP, PP, EP, CP 三维并行机制。
- **经典框架**：
  - [Megatron-LM](https://github.com/NVIDIA/Megatron-LM) - NVIDIA 高性能大模型训练框架
  - [DeepSpeed](https://github.com/microsoft/DeepSpeed) - 微软分布式训练优化库

---

## 4. 微调、对齐与强化学习 (Fine-tuning & Alignment)

- **高效微调 (PEFT)**：LoRA, QLoRA, DoRA, Prefix-Tuning。
- **偏好对齐 (RLHF / Direct Alignment)**：PPO, DPO, ORPO, SimPO, KTO。
- **主流框架**：
  - [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory) - 统一的大模型高效微调框架
  - [verl](https://github.com/volcengine/verl) - 灵活、高效的大模型强化学习框架

---

## 5. 模型能力扩展与 Skill (Model Skills & Capabilities)

- **长文本 (Long Context)**：Needle-in-a-Haystack, RoPE 外推 (YaRN), Chunked Attention.
- **推理与思考链 (CoT & Reasoning)**：Chain-of-Thought, Tree-of-Thoughts, Self-Correction, DeepSeek-R1 式强化学习推理。
- **多模态扩展**：Vision-Language Models (LLaVA, Qwen-VL)。

---

## 6. 检索增强生成 (RAG & Knowledge Integration)

- ** Parsing & Chunking**：文档版面分析、语义 Chunking 策略。
- **Embedding & Reranking**：向量检索、Sparse+Dense 混合检索、Reciprocal Rank Fusion (RRF)。
- **Advanced RAG**：GraphRAG, Modular RAG, Corrective RAG (CRAG).
- **主流框架**：[LlamaIndex](https://github.com/run-llama/llama_index), [LangChain](https://github.com/langchain-ai/langchain).

---

## 7. LLM Agent & 应用开发 (Agents & Applications)

- **Agent 范式**：ReAct, Plan-and-Solve, Memory 机制（Short/Long-term）。
- **Tool-Use / Function Calling**：OpenAI Function Calling, OpenClaw, AutoGen, CrewAI.

---

## 8. 推理加速与工程部署 (Inference & Deployment)

- **推理引擎**：
  - [vLLM](https://github.com/vllm-project/vllm) - 高吞吐 PagedAttention 推理引擎
  - [SGLang](https://github.com/sgl-project/sglang) - 高效 LLM 结构化生成与推理框架
  - [llama.cpp](https://github.com/ggerganov/llama.cpp) - 极简 C/C++ 本地模型运行库
- **量化技术**：AWQ, GPTQ, GGUF, FP8/FP4 Quantization.

---

## 9. 模型评估、安全与红队测试 (Evaluation & Safety)

- **评估基准**：MMLU, GSM8K, HumanEval, LMSYS Chatbot Arena.
- **安全与防护**：Jailbreak 攻防, Prompt Injection 防范, [NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails).

---

## 🤝 贡献指南 (Contributing)

非常欢迎你为本项目贡献资源或修改建议！在提交 Pull Request 前，请参阅 [CONTRIBUTING.md](./CONTRIBUTING.md) 规范。

---

## 📄 开源协议 (License)

本项目采用 [MIT License](./LICENSE) 许可证开源。
