# 🤝 贡献指南 (Contribution Guidelines)

首先，感谢你对 **Awesome-LLM-Learning-Path** 项目的关注与支持！开源社区的力量离不开每一位贡献者的参与。

为了保持仓库内容的质量、一致性与可维护性，请在提交 Issue 或 Pull Request (PR) 前仔细阅读以下规范。

---

## 📋 贡献流程 (Workflow)

1. **Fork 本仓库** 到你自己的 GitHub 账号。
2. **Clone 到本地** 并创建你的特性分支：
   ```bash
   git clone https://github.com/YOUR-USERNAME/Awesome-LLM-Learning-Path.git
   cd Awesome-LLM-Learning-Path
   git checkout -b feature/add-new-resource
   ```
3. **修改内容**（请遵循下方的 [格式规范](#-格式规范)）。
4. **提交变更** 并撰写清晰的 Commit Message：
   ```bash
   git commit -m "feat(rag): add GraphRAG tutorial and paper links"
   ```
5. **Push 到你的远端分支**：
   ```bash
   git push origin feature/add-new-resource
   ```
6. **提交 Pull Request**，并在描述中说明本次更新/添加的具体内容及理由。

---

## 🎯 资源收录标准 (Inclusion Criteria)

我们收录的资源必须符合以下原则：

- **高质量与时效性**：优先收录业内认可度高、内容严谨、近 1-2 年内较新或经典的论文、开源库与教程。
- **逻辑清晰**：收录的资源应属于大模型生命周期或落地应用链条中的明确节点。
- **拒绝硬广/低质营销**：不接受纯商业推销、无干货的公众号文章或质量较差的入门复制粘贴教程。
- **链接有效**：提交前请确保链接均可正常访问（推荐提供 GitHub 链接、arXiv 链接或官方文档）。

---

## 📐 Markdown 格式规范 (Formatting Rules)

为了保持页面整洁统一，请遵循以下排版建议：

### 1. 资源条目命名规范
* **项目 / 框架**：`[名称](URL) - 简短一句话描述（注明语言/特点）。`
  > 示例：`- [vLLM](https://github.com/vllm-project/vllm) - 基于 PagedAttention 的高性能 LLM 推理与服务引擎。`
* **论文**：`**论文名称** (作者/机构, 年份) [[Paper](URL)] [[Code](URL)] - 简短说明。`
  > 示例：`- **DeepSeek-V3 Technical Report** (DeepSeek, 2024) [[Paper](https://arxiv.org/abs/xxx)] - 介绍 671B MoE 模型的架构与训练细节。`

### 2. 排版风格
- 中英文之间请保留一个**半角空格**（如：“LLM 基础原理” 而非 “LLM基础原理”）。
- 使用标准的 GitHub Markdown 语法，不要嵌套过深的无序列表（建议不超过 3 层）。
- 新新增的内容应放置在相应分类的合理位置（优先推荐按主题/时间排序）。

---

## 💬 Commit 提交规范

建议采用标准 Commit 规范：

- `feat`: 添加新的学习资源或章节
- `fix`: 修复失效链接、错别字或格式错误
- `docs`: 修改文档或说明说明
- `refactor`: 重构或调整大纲目录结构

示例：`feat(finetune): add verl framework link`

---

## ❓ 提交反馈与讨论

- 如果你发现了错别字、失效链接或格式问题，欢迎直接提交 PR 修正。
- 如果你有大的章节调整建议，或想讨论某些资源是否适合加入，请先在 [Issues](../../issues) 中发起 Discussion，以便大家交流讨论后再开 PR。

再次感谢你的贡献！让大模型学习之路更加清晰平坦！🌟
