# LLM 推理与部署资源索引

## 1. 推理引擎与运行时

- [tensorrt-llm-nvidia](https://developer.nvidia.com/tensorrt-llm)：NVIDIA 的 TensorRT-LLM 产品入口，概览针对 NVIDIA GPU 的编译、量化、批处理和多 GPU 推理能力，适合评估高性能部署方案。
- <img src="https://img.shields.io/github/stars/NVIDIA/TensorRT-LLM?style=social" height="17" align="texttop"/> [TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM): NVIDIA 的开源 LLM 推理库，基于 TensorRT 优化算子、量化和多 GPU 执行，面向 NVIDIA GPU 上的低延迟高吞吐服务。
- <img src="https://img.shields.io/github/stars/sgl-project/sglang?style=social" height="17" align="texttop"/> [sglang](https://github.com/sgl-project/sglang): 面向复杂 LLM/VLM 程序的开源服务框架，提供 RadixAttention 前缀缓存、约束解码和高效调度，适合 Agent 与结构化生成。
- [docs.sglang](https://docs.sglang.io)：SGLang 官方文档，介绍面向语言与视觉语言模型的服务运行时、RadixAttention、结构化生成和前端接口配置。
- [vllm_latest](https://docs.vllm.ai/en/latest)：vLLM 官方文档，覆盖安装、模型兼容性、PagedAttention、连续批处理与 OpenAI 兼容服务，是部署 vLLM 的主要参考。
- [vllm-project.github.io](https://vllm-project.github.io)：vLLM 项目主页，汇总文档、论文、生态集成和发布信息，适合跟踪引擎能力演进与查找官方入口。
- <img src="https://img.shields.io/github/stars/vllm-project/vllm?style=social" height="17" align="texttop"/> [vllm](https://github.com/vllm-project/vllm): 开源高吞吐推理与服务引擎，以 PagedAttention 和连续批处理提升 KV Cache 利用率，提供 OpenAI 兼容 API。
- <img src="https://img.shields.io/github/stars/huggingface/text-generation-inference?style=social" height="17" align="texttop"/> [text-generation-inference](https://github.com/huggingface/text-generation-inference): Hugging Face 的文本生成推理服务器，支持流式生成、张量并行、连续批处理和安全部署，适合托管 Hugging Face 模型。
- <img src="https://img.shields.io/github/stars/sihyeong/awesome-llm-inference-engine?style=social" height="17" align="texttop"/> [awesome-llm-inference-engine](https://github.com/sihyeong/awesome-llm-inference-engine): 推理引擎资源清单，集中列出 vLLM、SGLang、TGI、TensorRT-LLM 等项目与对比资料，适合快速完成运行时选型。

- [text-generation-inference](https://hugging-face.cn/docs/inference-endpoints/engines/tgi)：Hugging Face Inference Endpoints 的 TGI 引擎说明，介绍托管端点所用的文本生成服务及其模型与硬件选择。
- [text-generation-inference-index](https://huggingface.co/docs/text-generation-inference/index)：TGI 官方文档，说明启动服务器、张量并行、量化、流式响应和监控配置，适合自托管 Hugging Face 文本生成模型。
- [sglang-vs-vllm-vs-tensorrt-llm-benchmark-2](https://iotdigitaltwinplm.com/sglang-vs-vllm-vs-tensorrt-llm-benchmark-2026)：对比 SGLang、vLLM 和 TensorRT-LLM 的基准文章，关注吞吐、延迟、显存与适用硬件，适合初步进行引擎选型。
- [TensorRT-LLM-overview-github](https://nvidia.github.io/TensorRT-LLM/architecture/overview.html)：TensorRT-LLM 架构文档，解释构建器、运行时、批处理调度和多 GPU 组件关系，适合理解其底层执行链路。
- [TensorRT-LLM-overview-doc](https://nvidia.github.io/TensorRT-LLM/overview.html)：TensorRT-LLM 概览文档，汇总安装、支持模型、量化和服务入口，适合部署前快速确定版本与工作流。

- [fast-and-efficient-llm-inference-with-vllm](https://www.deeplearning.ai/courses/fast-and-efficient-llm-inference-with-vllm)：DeepLearning.AI 的 vLLM 课程，实践 PagedAttention、连续批处理、KV Cache 管理和服务部署，适合理解高效推理核心机制。
- [2026-03-14-llm-inference-optimization-vllm](https://www.youngju.dev/blog/llm/2026-03-14-llm-inference-optimization-vllm-tensorrt-speculative-decoding.en)：对比 vLLM、TensorRT-LLM 与投机解码的优化文章，讨论吞吐、延迟和部署策略，适合建立推理性能调优思路。

## 2. 推理性能优化

- [LLM Inference Unveiled: Survey and Roofline Model Insights](https://arxiv.org/pdf/2402.16363v5)：LLM 推理综述论文，结合 Roofline 模型分析推理阶段的计算与访存瓶颈，系统讨论性能度量和硬件优化空间。
- [A Survey on Efficient Inference for LargeLanguage Models](https://arxiv.org/pdf/2404.14294v3)：高效大语言模型推理综述，覆盖压缩、并行、KV Cache 管理和系统优化等路线，适合建立性能优化知识框架。
- [Taming the Titans: A Survey of Efficient LLM Inference Serving](https://arxiv.org/pdf/2504.19720)：面向 LLM 高效推理的近期研究论文，分析模型执行、硬件利用和系统优化方法，适合了解新兴推理研究方向。
- [A Survey of LLM Inference Systems](https://arxiv.org/pdf/2506.21901v1)：LLM 推理系统综述，梳理服务栈、调度、内存管理与硬件协同等设计问题，适合从系统视角理解平台演进。
- [从实验室到生产线：大模型部署必须跨越的5道工程鸿沟
](https://blog.csdn.net/AlgoFun/article/details/155886191)：中文推理优化实践文章，围绕批处理、缓存、量化和显存管理等常见问题给出工程视角，适合补充性能调优经验。
- <img src="https://img.shields.io/github/stars/huggingface/blog?style=social" height="17" align="texttop"/> [bloom-inference-optimization](https://github.com/huggingface/blog/blob/main/bloom-inference-optimization.md): Hugging Face 关于 BLOOM 推理优化的工程文章，介绍分布式推理、量化和硬件策略，适合理解超大模型服务实践。
- <img src="https://img.shields.io/github/stars/linhvuquach/ai-howto?style=social" height="17" align="texttop"/> [05-inference-optimization](https://github.com/linhvuquach/ai-howto/blob/master/docs/05-inference-optimization.md): AI HowTo 的推理优化笔记，梳理批处理、缓存、量化和服务框架等常用策略，适合快速建立性能调优清单。
- [llm_optims](https://huggingface.co/docs/transformers/main/en/llm_optims)：Transformers 官方推理优化指南，介绍注意力加速、量化和编译等功能，适合在 Transformers 栈中降低服务成本。

## 3. 服务化与部署架构

- [Serve LLMs with Anyscale services](https://docs.anyscale.com/llm/serving)：Anyscale 的 LLM Serving 文档，说明如何使用 Ray Serve 扩展副本、路由请求和弹性资源，适合集群化模型服务。
- [qwen3-vllm-inference](https://docs.cloud.google.com/ai-hypercomputer/docs/tutorials/gpu/qwen3-vllm-inference?hl=zh-cn)：Google AI Hypercomputer 教程，演示在 GPU 环境使用 vLLM 部署 Qwen3，涵盖镜像、模型准备和服务调用。
- [serve-gemma-gpu-tensortllm](https://docs.cloud.google.com/kubernetes-engine/docs/tutorials/serve-gemma-gpu-tensortllm?hl=zh-cn)：GKE 教程，展示利用 GPU、Kubernetes 与 TensorRT-LLM 部署 Gemma 服务，适合学习云原生推理编排。
- [online_serving-vllm-docs](https://docs.vllm.ai/en/latest/serving/online_serving)：vLLM 在线服务文档，讲解 OpenAI 兼容 API、启动参数、模型加载和请求模式，是自托管服务的操作手册。
- [vllm-anyscale-deployment-frameworks](https://docs.vllm.ai/en/stable/deployment/frameworks/anyscale)：vLLM 与 Anyscale 集成文档，说明将推理副本交由 Ray 平台调度和扩缩容，适合处理集群级服务需求。
- [llm-deployment-best-practices-2026](https://futureagi.com/blog/llm-deployment-best-practices-2026)：生产部署最佳实践文章，讨论模型选型、容量规划、监控、成本和安全等问题，适合上线前制定部署检查清单。
- <img src="https://img.shields.io/github/stars/datawhalechina/llm-deploy?style=social" height="17" align="texttop"/> [llm-deploy](https://github.com/datawhalechina/llm-deploy): Datawhale 中文部署教程，涵盖开源模型推理、量化、服务框架与资源管理，适合中文开发者实践 LLM 部署。
- [tensorrt-llm-setup-guide](https://localaimaster.com/blog/tensorrt-llm-setup-guide)：TensorRT-LLM 安装配置指南，说明 NVIDIA 环境准备、依赖、构建与运行步骤，适合搭建本地 GPU 推理环境。
- [optimizing-llm-inference-with-quantization-techniques-and-vllm-deployment-strategies](https://martinuke0.github.io/posts/2026-03-04-optimizing-llm-inference-with-quantization-techniques-and-vllm-deployment-strategies)：量化与 vLLM 部署策略文章，讨论精度、显存、吞吐之间的权衡，适合制定模型压缩与服务配置方案。
- [llm-deployment](https://portkey.ai/blog/llm-deployment)：LLM 部署文章，讨论模型托管、网关、可观测性、可靠性和成本治理，适合从应用平台角度规划生产服务。
- [vllm-kubernetes](https://scaleops.com/blog/vllm-kubernetes)：vLLM on Kubernetes 实践文章，聚焦 GPU 调度、自动扩缩容和集群资源利用，适合部署高并发推理工作负载。
- [tensorrt-llm-production-deployment-guide](https://www.spheron.network/blog/tensorrt-llm-production-deployment-guide)：TensorRT-LLM 生产部署指南，覆盖构建引擎、模型量化、服务配置和性能验证，适合 NVIDIA GPU 推理上线。

## 4. 本地、边缘与轻量化推理

- <img src="https://img.shields.io/github/stars/Enterprise-AI-Atlas/awesome-local-llms?style=social" height="17" align="texttop"/> [awesome-local-llms](https://github.com/Enterprise-AI-Atlas/awesome-local-llms): 本地 LLM 工具与模型资源清单，覆盖桌面运行时、模型下载、UI 和硬件指南，适合调研离线与私有化方案。
- <img src="https://img.shields.io/github/stars/ggml-org/llama.cpp?style=social" height="17" align="texttop"/> [llama.cpp](https://github.com/ggml-org/llama.cpp): 高性能 C/C++ LLM 运行时，支持 GGUF、CPU/GPU 混合推理和多平台编译，是消费级设备本地运行模型的核心项目。
- <img src="https://img.shields.io/github/stars/google-ai-edge/LiteRT-LM?style=social" height="17" align="texttop"/> [LiteRT-LM](https://github.com/google-ai-edge/LiteRT-LM): Google 面向端侧的 LiteRT-LM 项目，探索在移动和边缘硬件上高效运行语言模型，适合关注轻量推理与设备集成。
- <img src="https://img.shields.io/github/stars/ollama/ollama?style=social" height="17" align="texttop"/> [ollama](https://github.com/ollama/ollama): 本地运行与管理开源模型的工具，提供模型拉取、Modelfile、HTTP API 和跨平台安装，适合快速搭建个人推理服务。
- [ollama.com](https://ollama.com)：Ollama 官方网站，提供客户端下载、模型库、文档和 API 指南，适合查找本地模型运行与集成的权威入口。
- <img src="https://img.shields.io/github/stars/rafska/awesome-local-llm?style=social" height="17" align="texttop"/> [awesome-local-llm](https://github.com/rafska/awesome-local-llm): 本地运行 LLM 的全栈资源导航，覆盖推理平台、引擎、UI、模型、Agent、MCP 与 RAG 工具，适合调研离线与私有化部署方案。

## 5. LLMOps、资源索引与工程实践

- [LLM推理优化实战指南：量化压缩、KV Cache与内存带宽瓶颈破解
](https://bbs.csdn.net/weixin_34079177/article/details/100164809)：中文 LLM 运维与部署讨论文章，提供模型服务、资源配置或工程实践线索，适合补充国内社区的经验参考。
- <img src="https://img.shields.io/github/stars/aerlabsAI/ai-inference-resources?style=social" height="17" align="texttop"/> [ai-inference-resources](https://github.com/aerlabsAI/ai-inference-resources): AI 推理资源汇总，收集引擎、优化库、论文和部署工具，适合建立推理技术调研清单。
- <img src="https://img.shields.io/github/stars/av/awesome-llm-services?style=social" height="17" align="texttop"/> [awesome-llm-services](https://github.com/av/awesome-llm-services): LLM 服务平台清单，整理 API 提供商、托管平台和基础设施，适合比较模型调用、部署和服务采购方案。
- <img src="https://img.shields.io/github/stars/CalvinXKY/InfraTech?style=social" height="17" align="texttop"/> [InfraTech](https://github.com/CalvinXKY/InfraTech): AI 基础设施技术资源库，覆盖算力、训练、推理和部署组件，适合从系统层面梳理模型服务技术栈。
- <img src="https://img.shields.io/github/stars/ifLabX/Awesome-LLMOps?style=social" height="17" align="texttop"/> [Awesome-LLMOps](https://github.com/ifLabX/Awesome-LLMOps): LLMOps 资源清单，汇集部署、监控、评测、治理和成本工具，适合搭建模型生命周期管理能力。
- <img src="https://img.shields.io/github/stars/InftyAI/Awesome-LLMOps?style=social" height="17" align="texttop"/> [Awesome-LLMOps](https://github.com/InftyAI/Awesome-LLMOps): 以 LLM 应用上线为重点的资源索引，收集可观测性、提示管理、网关和运营工具，适合完善生产运维方案。
- <img src="https://img.shields.io/github/stars/sam-blackfly/awesome-llm-tools?style=social" height="17" align="texttop"/> [awesome-llm-tools](https://github.com/sam-blackfly/awesome-llm-tools): 大语言模型工具清单，覆盖开发、部署、评测和生产力软件，适合在推理项目中发现可组合的辅助组件。
- <img src="https://img.shields.io/github/stars/tensorchord/Awesome-LLMOps?style=social" height="17" align="texttop"/> [Awesome-LLMOps](https://github.com/tensorchord/Awesome-LLMOps): 聚焦 MLOps/LLMOps 的开源项目集合，包含实验、部署、监控和数据管理工具，适合进行平台能力选型。
- <img src="https://img.shields.io/github/stars/trieungoctam/ai-engineering-from-scratch?style=social" height="17" align="texttop"/> [ai-engineering-from-scratch](https://github.com/trieungoctam/ai-engineering-from-scratch): 从零构建 AI 工程系统的学习项目，涉及模型应用、检索、Agent 与服务实践，适合建立端到端工程视角。
- <img src="https://img.shields.io/github/stars/xlite-dev/Awesome-LLM-Inference?style=social" height="17" align="texttop"/> [Awesome-LLM-Inference](https://github.com/xlite-dev/Awesome-LLM-Inference): LLM 推理资源索引，集中整理引擎、量化、缓存、服务和论文资料，适合快速追踪推理技术生态。
- [lmsys/blog](https://www.lmsys.org/blog)：LMSYS 官方博客发布模型服务、Arena、开源模型与系统研究动态，适合跟踪大模型推理和评测领域的工程进展。
- [llmops-guide](https://zenocloud.io/blog/llmops-guide)：LLMOps 指南，梳理模型部署、监控、评测、版本与成本管理等关键环节，适合建立生产运维流程框架。
- <img src="https://img.shields.io/github/stars/zenrran4nlp/Awesome-LLM-Inference-Serving?style=social" height="17" align="texttop"/> [Awesome-LLM-Inference-Serving](https://github.com/zenrran4nlp/Awesome-LLM-Inference-Serving): 综述《Taming the Titans: A Survey of Efficient LLM Inference Serving》的配套文献索引，按单实例/集群/新兴场景分类覆盖模型并行、请求调度、KV Cache、PD 分离等，适合追踪推理服务研究全景。
- <img src="https://img.shields.io/github/stars/adongwanai/Awesome-Awesome-LLMs?style=social" height="17" align="texttop"/> [Awesome-Awesome-LLMs](https://github.com/adongwanai/Awesome-Awesome-LLMs): LLM 元导航仓库，收录 200+ 个 awesome list 并按 40+ 细分类与星级评级组织，适合在海量资源中快速定位所需方向。
- <img src="https://img.shields.io/github/stars/e-dupuis/awesome-llm-deployment?style=social" height="17" align="texttop"/> [awesome-llm-deployment](https://github.com/e-dupuis/awesome-llm-deployment): LLM 部署资源合集，面向受约束环境的模型上线，收录框架、工具与实践参考，适合部署方案调研。
- <img src="https://img.shields.io/github/stars/saucam/awesome-llm-prod?style=social" height="17" align="texttop"/> [awesome-llm-prod](https://github.com/saucam/awesome-llm-prod): 生产级开源 LLM 项目合集，按高性能、可扩展与跨行业场景筛选生产就绪方案，适合寻找可直接落地的开源实现。
- <img src="https://img.shields.io/github/stars/aws-samples/awsome-inference?style=social" height="17" align="texttop"/> [awsome-inference](https://github.com/aws-samples/awsome-inference): AWS 推理参考架构与测试用例库，覆盖 EKS、加速型 EC2 及 TensorRT-LLM、SGLang、Ray 等框架的端到端部署，适合 AWS 上线推理服务。

## 6. 博客教程与工程实践

### 6.1 Hugging Face 官方博客

- [llm-inference-at-scale-with-tgi](https://huggingface.co/blog/martinigoyanes/llm-inference-at-scale-with-tgi): Hugging Face 关于使用 TGI 进行大规模 LLM 推理的实践文章，介绍部署配置、批处理与吞吐优化，适合理解 TGI 生产化路径。
- [Kseniase/inference](https://huggingface.co/blog/Kseniase/inference): Hugging Face 关于 LLM 推理的入门概述博客，梳理推理基础概念与常见优化方向，适合建立推理知识框架。
- [introduction-to-nano-vllm](https://huggingface.co/blog/zamal/introduction-to-nano-vllm): 介绍 nano-vllm——纯 Python 极简实现的推理引擎，代码简洁可读，适合从源码层面学习 PagedAttention 等核心机制。
- [llm-compressor](https://huggingface.co/blog/rishiraj/llm-compressor): Hugging Face 关于 LLM Compressor 压缩库的介绍，覆盖 W4A16、AWQ、GPTQ 等量化方案与推理加速，适合制定模型压缩方案。
- [llm-performance-request-queueing](https://huggingface.co/blog/tngtech/llm-performance-request-queueing): Hugging Face 关于请求排队对 LLM 服务性能影响的分析文章，讨论队列策略与吞吐延迟权衡，适合服务化调优。

### 6.2 NVIDIA 开发者博客

- [optimizing-inference-on-llms-with-tensorrt-llm](https://developer.nvidia.com/blog/optimizing-inference-on-llms-with-tensorrt-llm-now-publicly-available/): NVIDIA 关于使用 TensorRT-LLM 优化 LLM 推理的官方博客，介绍算子融合、量化与批处理能力，适合理解 TRT-LLM 优化路径。
- [recurrent-drafting](https://developer.nvidia.com/blog/nvidia-tensorrt-llm-now-supports-recurrent-drafting-for-optimizing-llm-inference/): NVIDIA 介绍 TensorRT-LLM 支持 recurrent drafting（一种投机解码变体）的博客，讲解其降低首 Token 延迟的原理，适合了解投机解码前沿。
- [scaling-llms-with-triton-and-tensorrt-llm](https://developer.nvidia.com/blog/scaling-llms-with-nvidia-triton-and-nvidia-tensorrt-llm-using-kubernetes/): NVIDIA 关于使用 Triton Inference Server 与 TensorRT-LLM 在 Kubernetes 上扩展 LLM 服务的博客，适合学习云原生推理编排。

### 6.3 Anyscale 与 Modal 部署实战

- [deepseek-vllm-ray-google-kubernetes](https://www.anyscale.com/blog/deepseek-vllm-ray-google-kubernetes): Anyscale 关于使用 vLLM、Ray 与 Google Kubernetes Engine 部署 DeepSeek 模型的实践博客，适合学习大规模推理服务编排。
- [ray-serve-wide-ep-disaggregated-serving-vllm](https://www.anyscale.com/blog/ray-serve-llm-anyscale-apis-wide-ep-disaggregated-serving-vllm): Anyscale 关于基于 Ray Serve 与 wide expert parallelism 的解耦服务架构博客，讨论 Prefill/Decode 分离与 vLLM 集成，适合高并发服务设计。
- [ray-serve-faster-first-token-custom-routing](https://www.anyscale.com/blog/ray-serve-faster-first-token-custom-routing): Anyscale 关于优化首 Token 延迟（TTFT）与自定义请求路由的博客，适合降低交互式场景的响应延迟。
- [high-performance-distributed-inference-ray-serve-vllm-gke](https://www.anyscale.com/blog/high-performance-distributed-inference-ray-serve-llm-vllm-google-kubernetes-gke): Anyscale 关于 Ray Serve + vLLM + GKE 高性能分布式推理的博客，涵盖张量并行、资源调度与弹性扩缩容，适合集群级推理部署。
- [how-to-deploy-vllm](https://modal.com/blog/how-to-deploy-vllm): Modal 关于在 Modal 平台上部署 vLLM 的教程，演示容器化、GPU 配置与 OpenAI 兼容 API 暴露，适合快速上手 vLLM 上线。

### 6.4 推理框架选型对比（中文）

- [LLM 推理服务化架构深度对比](https://juejin.cn/post/7649934594186084392): 掘金文章，从 KV Cache 管理、调度器、前缀缓存与结构化输出四维度深度对比 vLLM、SGLang、TensorRT-LLM 与 TGI，并给出选型决策框架。
- [2026 大模型部署框架终极选型指南](https://juejin.cn/post/7626665836176195635): 掘金文章，按硬件与业务场景对决 vLLM、TensorRT-LLM、SGLang、LMDeploy、oMLX、Ollama、MLC LLM 七大框架，给出场景化最优解。
- [主流大模型推理部署框架一文讲清](https://juejin.cn/post/7592451049233776686): 掘金文章，系统梳理 vLLM、SGLang、TensorRT-LLM、Ollama、XInference、LightLLM 与国产适配框架的核心技术与适用场景。

### 6.5 LLM 应用工程模式与生产思考

- [Patterns for Building LLM-based Systems & Products](https://eugeneyan.com/writing/llm-patterns/): Eugene Yan 关于 LLM 系统与产品构建的七大模式总结（评估、RAG、微调、缓存、防护栏、防御性 UX、用户反馈），适合建立应用工程全景。
- [How to Match LLM Patterns to Problems](https://eugeneyan.com/writing/llm-problems/): Eugene Yan 的续篇，讨论如何将上述模式匹配到性能不足、约束、延迟、不可靠输出等具体 LLM 问题，适合做架构决策。
- [Building LLM applications for production](https://huyenchip.com/2023/04/11/llm-engineering.html): Chip Huyen 关于构建面向生产的 LLM 应用的经典文章，讨论自然语言歧义、成本延迟与提示规范化等核心挑战，适合理解 LLM 工程化难点。