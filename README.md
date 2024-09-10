# **Awesome-Agent-Papers**🚀🚀🚀


[![GitHub Repo stars](https://img.shields.io/github/stars/Eileen19200930/Awesome-Agent-Papers?style=social)](https://github.com/yourusername/Awesome-Agent-Papers/) 
[![GitHub Repo forks](https://img.shields.io/github/forks/Eileen19200930/Awesome-Agent-Papers?style=social)](https://github.com/yourusername/Awesome-Agent-Papers/) 
[![Awesome](https://img.shields.io/badge/Awesome-green.svg)](https://github.com/yourusername/Awesome-Agent-Papers/) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)  
![Last Commit](https://img.shields.io/github/last-commit/Eileen19200930/Awesome-Agent-Papers?color=green) 


[**English**](README.md) | **中文版**

这里收集了针对大型语言模型（LLMs）和智能代理（Agents）相关的精选论文和资源。

## 🌱 如何贡献
我们热烈欢迎大家的贡献，无论您是发现拼写错误、错误、有建议，还是想要分享与LLMs+Agents相关的资源。

## 📜 目录
- [**Awesome Agent Papers**🚀🚀🚀](#awesome-agent-papers)
  - [📜 目录](#-目录)
  - [👋 简介](#-简介)
  - [📖 综述](#-综述)
  - [💬 经典模型](#-经典模型)
  - [🔥 基础模型](#-基础模型)
  - [💡 暂定](#-暂定)
  - [💪 数据集](#-数据集)
  - [🌈 评测指标](#-评测指标)
  - [📦 库函数](#-库函数)
  - [🔧 实践项目](#-实践项目)
  - [🔗 引用](#-引用)
  - [🤝 友情链接](#-友情链接)

## 👋 简介
- Awesome Agent Papers 是一个致力于收集和整理有关大型语言模型和智能代理的学术论文、项目、工具和资源的社区驱动项目。我们的目标是为研究人员和开发者提供一个集中的平台，以便于他们能够快速找到所需的资料。

## 📖 综述


## 💬 Multi-Agent应用/模拟
- (ACL2024) **IBSEN: Director-Actor Agent Collaboration for Controllable and Interactive Drama Script Generation** [paper](https://arxiv.org/pdf/2407.01093.pdf)  

  **摘要速览**  
  大型语言模型已展示出在情节创造和角色扮演方面的能力。本文介绍了IBSEN，一个导演-演员协调代理框架，用于生成戏剧剧本并使代理执行的情节更加可控。导演代理编写情节大纲，指导演员代理进行角色扮演，并在人类玩家参与时重新安排情节，以确保情节朝着目标发展。我们创建了一个新颖的戏剧情节，涉及多个演员代理，并在导演代理的指令下检查它们之间的交互。评估结果表明，我们的框架能够仅从一个粗略的情节大纲生成完整、多样化的戏剧剧本，同时保持戏剧中角色的特点。

  **主要贡献**  
  - 提出IBSEN框架，通过导演和演员代理生成可控的戏剧剧本。
  - 允许人类玩家参与情节，并根据玩家的行动动态调整情节细节。
  - 对框架性能进行了初步的定量和定性分析，验证其在生成戏剧剧本方面的有效性。
  
---

- (ACL2024) **Collaborative Mechanisms for LLM Agents: A Social Psychology View** [paper](https://arxiv.org/abs/2310.02124)  

  **摘要速览**  
  随着自然语言处理（NLP）系统在复杂社会环境中的日益部署，出现了一个关键问题：这些NLP系统能否复制人类社会中观察到的协作智能，尤其是在由多种大型语言模型（LLMs）组成的多代理框架中？本文探讨了当代NLP系统之间的协作动态，结合了实证实验和理论见解。我们构建了四个独特的“社会”，由不同“特征”（随和或自信过度）的LLM代理组成，且通过不同的“思维模式”（辩论或反思）进行协作。我们对这些多代理社会在三个基准数据集上的评估显示，某些协作策略不仅超越了之前的最先进方法，同时还通过使用更少的API令牌提高了效率。此外，我们的研究结果表明，LLM代理展现出类似于人类的社会行为，如从众和达成共识，这与社会心理学的基础理论相一致。最后，我们整合了社会心理学的见解，以对LLM代理之间的协作进行背景化，激励对LLM协作机制的进一步探索。我们承诺分享我们的代码和数据集，希望能够促进该有前景领域的进一步研究。

  **主要贡献**  
  - 探讨了多种LLM代理在社会环境中的协作动态。
  - 通过实证实验和理论分析，展示了LLM代理的社会行为特征。
  - 提供了对LLM协作机制的背景化理解，促进未来的研究探索。

- (NeurIPS) **Reflexion: Language Agents with Verbal Reinforcement Learning** [paper](https://arxiv.org/pdf/2303.11366)   

  **摘要速览**  
  大型语言模型（LLMs）越来越多地被用作与外部环境（例如游戏、编译器、API）交互的目标驱动代理。然而，这些语言代理如何快速有效地从试错中学习仍然是一个挑战，因为传统的强化学习方法需要大量的训练样本和昂贵的模型微调。本文提出了一个名为Reflexion的框架，该框架通过语言反馈而非权重更新来强化语言代理。具体来说，Reflexion代理会口头反思任务反馈信号，然后将它们自己的反思文本保存在情景记忆缓冲区中，以在后续试验中做出更好的决策。Reflexion能够整合各种类型（标量值或自由形式语言）和来源（外部或内部模拟）的反馈信号，并在多样化的任务（顺序决策、编码、语言推理）上取得了显著的改进。例如，Reflexion在HumanEval编码基准测试中实现了91%的pass@1准确率，超过了之前达到80%准确率的最新技术GPT-4。此外，作者还进行了不同的反馈信号、反馈整合方法和代理类型的消融和分析研究，并提供了对它们如何影响性能的见解。所有代码、演示和数据集已在GitHub上发布。

  **主要贡献**  
  - 提出了Reflexion框架，通过语言反馈而非权重更新来强化语言代理。
  - 展示了Reflexion在多样化任务中的有效性，并在某些任务上超越了现有的最先进技术。
  - 通过消融和分析研究，提供了对不同反馈信号和方法如何影响代理性能的见解。
  
  **摘要速览** 
  本研究探索了大型语言模型（LLMs）在中国侦探角色扮演游戏“剧本杀”中的应用，这是一个人工智能（AI）驱动游戏领域的新尝试。我们首次为“剧本杀”引入了包含角色剧本和游戏规则的数据集，以促进AI代理在这一复杂叙事环境中的发展。我们提出了一个独特的多代理交互框架，使用LLMs使AI代理能够自主参与游戏。为了评估这些AI代理的游戏表现，我们开发了新的方法来衡量它们对案例信息的掌握和推理技能。此外，我们还结合了最新的上下文学习进展，以提高代理在信息收集、凶手识别和逻辑推理方面的表现。实验结果验证了我们提出的方法的有效性。本研究旨在提供理解LLM能力的新颖视角，并为基于大型语言模型的代理评估建立新的基准。
- (ACL2024) **Deciphering Digital Detectives: Understanding LLM Behaviors and Capabilities in Multi-Agent Mystery Games** [paper](https://arxiv.org/abs/2312.00746)   


  **主要贡献**  
  - 我们创建了一个中文数据集，提供角色剧本和预设的游戏规则，以启动“剧本杀”游戏。据我们所知，这是第一个专门为AI代理在“剧本杀”游戏设置中量身定制的数据集。
  - 我们设计了一个使用大型语言模型的多代理交互框架，允许多个基于LLM的代理在“剧本杀”游戏环境中自主交互，无需人工干预。
  - 为了定量和定性评估基于大型语言模型的代理在“剧本杀”游戏中的表现，我们设计了两个新任务：一个评估它们对案例信息的掌握，另一个评估它们利用收集到的信息进行推理的能力。
  - 利用上下文学习的最新进展，我们设计了模块来增强基于LLM的代理的性能。我们的评估表明，这种设计显著提高了基于LLM的代理在“剧本杀”游戏环境中的信息掌握、凶手识别和推理能力。
---

## 🔥 基础模型


## 💡 暂定


## 💪 数据集


## 🌈 评测指标


## 📦 库函数


## 🔧 实践项目


## 🔗 引用


## 🤝 友情链接
- [AgentCourt](https://github.com/relic-yuexi/AgentCourt) [![GitHub stars](https://img.shields.io/github/stars/relic-yuexi/AgentCourt?style=social)](https://github.com/relic-yuexi/AgentCourt) - A project that simulates real courtroom proceedings with intelligent agents, exploring the application of AI in legal settings.


