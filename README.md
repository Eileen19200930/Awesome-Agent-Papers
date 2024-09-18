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
  - [💬 Agent](#-Agent)
  - [🔥 ICL(In-context Learning)](#-ICL)
  - [🌟 COT (Chain-of-Thought Reasoning)](#-COT)
  - [💡 暂定](#-暂定)
  - [💪 数据集](#-数据集)
  - [🌈 评测指标](#-评测指标)
  - [📦 库函数](#-库函数)
  - [🔧 实践项目](#-实践项目)
  - [🔗 引用](#-引用)
  - [🤝 友情链接](#-友情链接)

## 👋 简介
- Awesome Agent Papers 是一个致力于收集和整理有关大型语言模型和智能代理的学术论文、项目、工具和资源的社区驱动项目。我们的目标是为研究人员和开发者提供一个集中的平台，以便于他们能够快速找到所需的资料。


## 💬 Agent
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

---

- (NeurIPS) **Reflexion: Language Agents with Verbal Reinforcement Learning** [paper](https://arxiv.org/pdf/2303.11366)   

  **摘要速览**  
  大型语言模型（LLMs）越来越多地被用作与外部环境（例如游戏、编译器、API）交互的目标驱动代理。然而，这些语言代理如何快速有效地从试错中学习仍然是一个挑战，因为传统的强化学习方法需要大量的训练样本和昂贵的模型微调。本文提出了一个名为Reflexion的框架，该框架通过语言反馈而非权重更新来强化语言代理。具体来说，Reflexion代理会口头反思任务反馈信号，然后将它们自己的反思文本保存在情景记忆缓冲区中，以在后续试验中做出更好的决策。Reflexion能够整合各种类型（标量值或自由形式语言）和来源（外部或内部模拟）的反馈信号，并在多样化的任务（顺序决策、编码、语言推理）上取得了显著的改进。例如，Reflexion在HumanEval编码基准测试中实现了91%的pass@1准确率，超过了之前达到80%准确率的最新技术GPT-4。此外，作者还进行了不同的反馈信号、反馈整合方法和代理类型的消融和分析研究，并提供了对它们如何影响性能的见解。所有代码、演示和数据集已在GitHub上发布。

  **主要贡献**  
  - 提出了Reflexion框架，通过语言反馈而非权重更新来强化语言代理。
  - 展示了Reflexion在多样化任务中的有效性，并在某些任务上超越了现有的最先进技术。
  - 通过消融和分析研究，提供了对不同反馈信号和方法如何影响代理性能的见解。
  
---

- (ACL2024) **Deciphering Digital Detectives: Understanding LLM Behaviors and Capabilities in Multi-Agent Mystery Games** [paper](https://arxiv.org/abs/2312.00746)   

  **摘要速览** 
  本研究探索了大型语言模型（LLMs）在中国侦探角色扮演游戏“剧本杀”中的应用，这是一个人工智能（AI）驱动游戏领域的新尝试。我们首次为“剧本杀”引入了包含角色剧本和游戏规则的数据集，以促进AI代理在这一复杂叙事环境中的发展。我们提出了一个独特的多代理交互框架，使用LLMs使AI代理能够自主参与游戏。为了评估这些AI代理的游戏表现，我们开发了新的方法来衡量它们对案例信息的掌握和推理技能。此外，我们还结合了最新的上下文学习进展，以提高代理在信息收集、凶手识别和逻辑推理方面的表现。实验结果验证了我们提出的方法的有效性。本研究旨在提供理解LLM能力的新颖视角，并为基于大型语言模型的代理评估建立新的基准。

  **主要贡献**  
  - 我们创建了一个中文数据集，提供角色剧本和预设的游戏规则，以启动“剧本杀”游戏。据我们所知，这是第一个专门为AI代理在“剧本杀”游戏设置中量身定制的数据集。
  - 我们设计了一个使用大型语言模型的多代理交互框架，允许多个基于LLM的代理在“剧本杀”游戏环境中自主交互，无需人工干预。
  - 为了定量和定性评估基于大型语言模型的代理在“剧本杀”游戏中的表现，我们设计了两个新任务：一个评估它们对案例信息的掌握，另一个评估它们利用收集到的信息进行推理的能力。
  - 利用上下文学习的最新进展，我们设计了模块来增强基于LLM的代理的性能。我们的评估表明，这种设计显著提高了基于LLM的代理在“剧本杀”游戏环境中的信息掌握、凶手识别和推理能力。
---
- **Agent Alignment in Evolving Social Norms** [paper](https://arxiv.org/abs/2401.04620v4)

  **摘要速览**
  随着基于大型语言模型（LLMs）的智能体越来越多地渗透到人类生产和生活的各个领域，将它们与人类价值观对齐变得尤为重要。目前对AI系统的对齐主要集中在通过人工干预被动地对齐LLMs。然而，智能体具有接收环境反馈和自我演化的特性，使得现有的LLM对齐方法不再充分。为此，我们提出了一个名为EvolutionaryAgent的智能体演化和对齐的演化框架，将智能体对齐转化为在适者生存原则下的演化和选择过程。在社会规范不断演化的环境中，更好地适应当前社会规范的智能体将有更高的概率生存和繁衍，而那些对齐不当的智能体则会随着时间的推移而减少。从多个角度评估智能体在与社会规范对齐方面的实验结果表明，EvolutionaryAgent能够随着时间的推移更好地与不断演化的社会规范对齐，同时保持其在一般任务上的熟练程度。在各种开源和闭源LLMs上进行的有效性测试也证明了我们方法的适用性。

  **主要贡献**

  - 我们介绍了EvolutionaryAgent，这是一种基于适者生存原则在动态环境中进行智能体演化和对齐的方法。
  - 我们设计了一个演化环境EvolvingSociety，以及一种在变化环境中评估智能体的方法。
  - 我们系统地定义了智能体对齐，并通过基于各种LLMs的实验证明了EvolutionaryAgent能够持续地产生与演化社会规范对齐的智能体。
## 🔥 ICL(In-context Learning)
- **A Survey on In-context Learning**

  **摘要速览**

  本文综述了大型语言模型（LLMs）的上下文学习（In-context Learning, ICL）的最新进展和挑战。随着模型和数据规模的增长，LLMs表现出了通过上下文中的少量示例进行学习的能力。文章首先给出了ICL的正式定义，并阐明了其与相关研究的关系。接着，文章组织并讨论了先进技术，包括训练策略、提示设计策略和相关分析。此外，文章探索了ICL在数据工程和知识更新等不同应用场景，并讨论了ICL面临的挑战和未来研究方向。

  **主要贡献**

  - 提供了ICL的正式定义，并明确了其与相关研究的联系。
  - 系统地组织和讨论了ICL的先进技术，包括训练策略和提示设计策略。
  - 探索了ICL在多个领域的应用，如数据工程和知识更新。
  - 讨论了ICL面临的挑战，并为未来的研究方向提出了建议。

- (ICLR2024) **Training Socially Aligned Language Models on Simulated Social Interactions** [paper](https://arxiv.org/pdf/2305.16960v3.pdf)

  **摘要速览**  
  这篇论文探讨了如何通过模拟社会互动来训练语言模型，使其在与社会价值观对齐方面表现更好。研究提出了一种新颖的训练方法，使语言模型能够从模拟的社会互动中学习，从而在不同的场景中表现更为稳定，能够更准确地反映社会规范与价值。研究结果表明，与现有的方法相比，这种新的训练范式在对齐基准测试和人类评估中表现更优异。

  **主要贡献**  
  - 提出了一种通过模拟社会互动进行语言模型训练的新范式，旨在提高模型在社会价值对齐方面的表现。
  - 该方法更具可扩展性和效率，避免了当前基于奖励建模方法中的不稳定性和奖励游戏问题。
  - 通过模拟社会互动收集细粒度的反馈数据，使得模型能够更好地反映社会规范和价值。

## 🌟 COT
- **Igniting Language Intelligence: The Hitchhiker’s Guide From Chain-of-Thought Reasoning to Language Agents paper**
[paper](https://arxiv.org/abs/2311.11797) 
  **摘要速览** 
  大型语言模型（LLMs）在语言智能领域的提升显著，其在复杂推理任务中的卓越表现得到了充分验证。此外，理论证明揭示了它们的涌现推理能力，展示了它们在语言上下文中的高级认知能力。LLMs在处理复杂推理任务中的显著有效性，关键在于它们利用链式推理（CoT）技术，要求模型在得出答案的过程中制定中间步骤。CoT推理方法不仅在提升推理表现方面表现出色，还增强了可解释性、可控性和灵活性。基于这些优点，近期研究将CoT推理方法扩展到了自主语言智能体的发展，使其能够遵循语言指令并在各种环境中执行动作。
  本文综述了多个重要研究维度，包括：（i）CoT技术的基础机制，重点阐明其有效性的条件和依据；（ii）CoT的范式转变；以及（iii）基于CoT方法的语言智能体的发展。未来的研究方向涵盖了泛化、效率、定制、扩展和安全性等方面。我们希望为读者提供对CoT推理和语言智能体等研究领域的全面理解，并阐明这些领域之间的相互联系。

  **主要贡献** 

  根据我们所知，这是首次系统地探讨链式推理（CoT）技术的基础机制、CoT的范式转变以及CoT与智能体之间的复杂互动。主要贡献包括：
  - CoT在两个主要条件下表现出有效性：首先，当使用的LLM参数至少为200亿时；其次，当LLM中的参数知识包含与任务相关且保持强相互关联的知识块时。
  - CoT通过帮助识别对推理至关重要的基本知识块，并通过形成中间推理步骤无缝连接这些组件来发挥作用。
  - CoT技术经历了显著的范式转变，涉及提示模式、推理格式和应用场景的变化。
  - CoT成为了推动LLM赋能智能体发展的催化剂，使其能够理解语言指令并在现实世界和模拟环境中执行动作，特别是在感知、记忆和推理能力上增强了智能体的能力。
  尽管LLM、CoT推理和语言智能体迅速发展，但仍然存在许多挑战，例如在未见领域的泛化、在冗余交互中的效率、语言智能体的定制、语言智能体的扩展以及确保语言智能体的安全性。

## 💡 暂定


## 💪 数据集


## 🌈 评测指标


## 📦 库函数


## 🔧 实践项目


## 🔗 引用


## 🤝 我的相关工作
- [AgentCourt](https://github.com/relic-yuexi/AgentCourt) [![GitHub stars](https://img.shields.io/github/stars/relic-yuexi/AgentCourt?style=social)](https://github.com/relic-yuexi/AgentCourt) - A project that simulates real courtroom proceedings with intelligent agents, exploring the application of AI in legal settings.


