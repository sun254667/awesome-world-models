<div align="center">

# 🎥 Awesome World Models

<p align="center">
  <img src="wm_banner.png" alt="Awesome World Models" width="100%">
</p>

<p align="center">
  <img src="wm_QRcode.png" alt="Awesome World Models" width="100%">
</p>
</div>

[![中文](https://img.shields.io/badge/语言-中文-red)](README.zh-CN.md)
[![English](https://img.shields.io/badge/Language-English-blue)](README.md)
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](LICENSE)

> A curated, learning-friendly list of world model research resources: papers, datasets, benchmarks, simulation platforms, code, models, and tutorials, covering both classic foundational works and cutting-edge advances, catering to research initiation and industrial deployment.

✅ **Inclusion Criteria**
- Prioritize high-quality works from top conferences and journals such as CVPR / ICCV / ECCV / NeurIPS / ICLR / ICML / RSS / AAAI / TPAMI
- Cover core cutting-edge directions: Language-Based World Models, Visual/Video World Models, 3D/4D World Modeling, Latent Space World Models, Object-Centric World Models, Symbolic & Neuro-Symbolic World Models, Interactive World Models, World Action Models (WAM), Vision-Language-Action (VLA), Model-Based RL, Robotics & Embodied AI, Autonomous Driving, GUI/Computer-Use Agents, Scientific Simulation

---

## Table of Contents
1. [Surveys & Overviews](#-surveys--overviews)
2. [Tutorials & Starter Resources](#-tutorials--starter-resources)
3. [Foundation Papers & Technical Reports](#-foundation-papers--technical-reports)
4. [Core World Model Paradigms](#-core-world-model-paradigms)
   - 4.1 [Language-Based World Models](#41-language-based-world-models)
   - 4.2 [Visual / Video World Models](#42-visual--video-world-models)
   - 4.3 [3D & 4D World Models (General Purpose)](#43-3d--4d-world-models-general-purpose)
   - 4.4 [Latent Space World Models](#44-latent-space-world-models)
   - 4.5 [Object-Centric World Models](#45-object-centric-world-models)
   - 4.6 [Symbolic & Neuro-Symbolic World Models](#46-symbolic--neuro-symbolic-world-models)
   - 4.7 [General Foundation World Models](#47-general-foundation-world-models)
5. [Interactive World Models](#-interactive-world-models)
   - 5.1 [General Interactive Frameworks](#51-general-interactive-frameworks)
   - 5.2 [Game & Open-World Exploration (Application)](#52-game--open-world-exploration-application)
6. [World Action Models (WAM) & VLA Integration](#-world-action-models-wam--vla-integration)
   - 6.1 [Cascaded WAM](#61-cascaded-wam)
   - 6.2 [Joint WAM & Unified VLA-World Models](#62-joint-wam--unified-vla-world-models)
   - 6.3 [World Models for VLA Training & Evaluation (Combining Paradigms)](#63-world-models-for-vla-training--evaluation-combining-paradigms)
7. [Model-Based RL World Models](#-model-based-rl-world-models)
   - 7.1 [Classic Series](#71-classic-series)
   - 7.2 [Continuous Control](#72-continuous-control)
   - 7.3 [Offline & Generalization](#73-offline--generalization)
8. [Application Domains](#-application-domains)
   - 8.1 [Robotics & Embodied AI](#81-robotics--embodied-ai)
     - 8.1.1 [Foundation Embodied World Models](#811-foundation-embodied-world-models)
     - 8.1.2 [Manipulation](#812-manipulation)
     - 8.1.3 [Navigation](#813-navigation)
     - 8.1.4 [Locomotion & Loco-Manipulation](#814-locomotion--loco-manipulation)
     - 8.1.5 [World Models x Policy Learning](#815-world-models-x-policy-learning)
     - 8.1.6 [Policy Evaluation with World Models](#816-policy-evaluation-with-world-models)
   - 8.2 [Autonomous Driving](#82-autonomous-driving)
   - 8.3 [GUI / Computer-Use Agents](#83-gui--computer-use-agents)
   - 8.4 [Scientific Discovery](#84-scientific-discovery)
   - 8.5 [Social & Economic Simulation](#85-social--economic-simulation)
9. [Datasets & Benchmarks](#-datasets--benchmarks)
   - 9.1 [General World Modeling](#91-general-world-modeling)
   - 9.2 [Physics & Causality](#92-physics--causality)
   - 9.3 [Domain-Specific Benchmarks](#93-domain-specific-benchmarks)
10. [Training & Inference Techniques](#-training--inference-techniques)
    - 10.1 [Memory Mechanisms](#101-memory-mechanisms)
    - 10.2 [Post-Training & Test-Time Scaling](#102-post-training--test-time-scaling)
    - 10.3 [Efficient & Real-Time Inference](#103-efficient--real-time-inference)
11. [Simulation Platforms & Physics Engines](#-simulation-platforms--physics-engines)
    - 11.1 [General Simulation Platforms](#111-general-simulation-platforms)
    - 11.2 [Differentiable Physics Engines & Neural Simulators](#112-differentiable-physics-engines--neural-simulators)
    - 11.3 [Interactive World Models & Game Engines](#113-interactive-world-models--game-engines)
    - 11.4 [Physics Simulation & Engine Integration](#114-physics-simulation--engine-integration)
    - 11.5 [Benchmarks for World Model Simulation](#115-benchmarks-for-world-model-simulation)
    - 11.6 [Code Agents & Simulation Construction](#116-code-agents--simulation-construction)
    - 11.7 [Surveys & Perspectives](#117-surveys--perspectives)
12. [Theory, Interpretability & Positions](#-theory-interpretability--positions)
    - 12.1 [Theory & Explainability](#121-theory--explainability)
    - 12.2 [Positions & Opinion Papers](#122-positions--opinion-papers)
13. [Related Awesome Lists](#-related-awesome-lists)
14. [Key Research Challenges](#-key-research-challenges)
15. [Contact](#-contact)
16. [License](#-license)

---

## 📚 Surveys & Overviews



- **A Definition and Roadmap for World Models**
  - Publication: arXiv 2026
  - Highlights: Provides a scientific definition of world models, discussions of their key technical aspects, and a staged roadmap for developing effective world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.06401)

- **World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications**
  - Publication: arXiv 2026
  - Highlights: Comprehensive survey covering architectures, methodologies, reasoning paradigms, and applications of world models; proposes a multi-axis taxonomy organized along four dimensions.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.00133)

- **A Comprehensive Survey on World Models for Embodied AI**
  - Publication: arXiv 2026
  - Highlights: Presents a unified framework for world models in embodied AI with a three-axis taxonomy encompassing Functionality, Decision-Coupled vs. General-Purpose, and Temporal Modeling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.16732)

- **Towards Interactive Video World Modeling: Frontiers, Challenges, Benchmarks, and Future Trends**
  - Publication: arXiv 2026
  - Highlights: Systematically reviews recent research trends, technical developments, evaluation benchmarks, and future directions in interactive world modeling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.01164)

- **World Action Models: A Survey**
  - Publication: arXiv 2026
  - Highlights: First systematic survey of World Action Models (WAMs), clarifying boundaries between world models, video generation models, action-grounded video world models, VLA policies, and WAMs.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.20781)

- **From World Models to World Action Models: A Concise Tutorial for Robotics**
  - Publication: arXiv 2026
  - Highlights: Defines world models as action-conditioned predictive models, summarizing four representative paradigms: imagine-then-execute, video-feature-conditioned action prediction, joint video-action modeling, and auxiliary video prediction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.00836)

- **World Models for Robotic Manipulation: A Survey**
  - Publication: arXiv 2026
  - Highlights: Surveys world models for robotic manipulation through three questions: what future representation to predict, how prediction connects to action, and when to use it in robot learning pipelines.
  - Paper Link: [arXiv](https://export.arxiv.org/abs/2606.00113)

- **A Tutorial on World Models and Physical AI**
  - Publication: arXiv 2026
  - Highlights: Presents a coherent framework unifying diverse world modeling approaches through shared predictive structure; connects world modeling techniques to physical AI applications such as robotics and autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.12783)

- **Safety, Security, and Cognitive Risks in World Models**
  - Publication: arXiv 2026
  - Highlights: Surveys world model architectures and their deployment contexts in safety-critical domains, characterizing the world model asset inventory and threat surface.
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.01346)

- **How Should World Models Be Evaluated for Embodied Decision-Making? A Decision-Making-Centric Position**
  - Publication: arXiv 2026
  - Highlights: Proposes an L0-L7 evaluation ladder spanning from visual plausibility to policy optimization utility, emphasizing intervention action fidelity and closed-loop rollout effectiveness.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.15032)

- **3D and 4D World Modeling: A Survey**
  - Publication: arXiv 2025 (v4 2026)
  - Highlights: First specialized survey on 3D and 4D world modeling and generation; establishes precise definitions and a structured taxonomy covering VideoGen, OccGen, and LiDARGen; systematically summarizes domain-specific datasets and evaluation metrics.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.07996)

- **A Survey of World Models for Autonomous Driving**
  - Publication: arXiv 2025
  - Highlights: Comprehensive survey of world models for autonomous driving, covering methods from video generation to 4D occupancy forecasting.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.11260)

- **World Model for Robot Learning: A Comprehensive Survey**
  - Publication: arXiv 2025
  - Highlights: Comprehensive survey of world models for robot learning, with a focus on policy learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.00080)

- **From Masks to Worlds: A Hitchhiker's Guide to World Models**
  - Publication: arXiv 2025
  - Highlights: A tutorial-style guide to world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.20668)

- **World Models in Artificial Intelligence: Sensing, Learning, and Reasoning Like a Child**
  - Publication: arXiv 2025
  - Highlights: Discusses world models from a cognitive perspective.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.15168)

- **Is Sora a World Simulator? A Comprehensive Survey on General World Models and Beyond**
  - Publication: arXiv 2024
  - Highlights: Comprehensive survey on general world models and their relation to video generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2405.03520)

- **Understanding World or Predicting Future? A Comprehensive Survey of World Models**
  - Publication: arXiv 2024
  - Highlights: Broad survey of world models with a focus on prediction and understanding.
  - Paper Link: [arXiv](https://arxiv.org/abs/2411.14499)

- **World Models: The Safety Perspective**
  - Publication: arXiv 2024
  - Highlights: Survey on safety challenges and risks of world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2411.07690)

---

## 🧪 Tutorials & Starter Resources


- **Nano World Models: A Minimalist Implementation of Future Video Prediction**
  - Publication: arXiv 2026
  - Highlights: A minimalist implementation of future video prediction with unified interface.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.23993) | [Website](https://simchowitzlabpublic.github.io/nano-world-model/) | [Code](https://github.com/simchowitzlabpublic/nano-world-model)

- **minWM: A Full-Stack Open-Source Framework for Real-Time Interactive Video World Models**
  - Publication: arXiv 2026
  - Highlights: Full-stack open-source framework for real-time interactive video world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.30263) | [Code](https://github.com/shengshu-ai/minWM)

- **StableWM: A Platform for Reproducible World Modeling Research and Evaluation**
  - Publication: arXiv 2026
  - Highlights: Platform for reproducible world modeling research and evaluation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.21800) | [Website](https://galilai-group.github.io/stable-worldmodel/) | [Code](https://github.com/galilai-group/stable-worldmodel)

---

## 📄 Foundation Papers & Technical Reports



- **Video generation models as world simulators** (OpenAI Sora, 2024)
  - [Technical Report](https://openai.com/research/video-generation-models-as-world-simulators)
  - Highlights: Demonstrates that large-scale video generation can act as a world simulator.

- **A Path Towards Autonomous Machine Intelligence** (Yann LeCun, 2022)
  - Paper: [OpenReview](https://openreview.net/pdf?id=BZ5a1r-kVsf)
  - Highlights: LeCun's vision of world models as a core component of autonomous intelligence.

- **World Models** (Ha & Schmidhuber, 2018)
  - Paper: [arXiv](https://arxiv.org/abs/1803.10122) | [Website](https://worldmodels.github.io/)
  - Highlights: The seminal work that introduced the concept of world models in deep learning.

---

## 🧠 Core World Model Paradigms

### 4.1 Language-Based World Models



- **Qwen-AgentWorld: Language World Models for General Agents**
  - Publication: arXiv 2026
  - Highlights: First native language world models (35B-A3B and 397B-A17B) simulating agentic environments across 7 domains via long CoT reasoning, trained on >10M interaction trajectories.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.24597)

- **WorldLLM: Improving LLMs' world modeling using curiosity-driven theory-making**
  - Publication: arXiv 2025
  - Highlights: Leverages curiosity-driven theory-making to improve LLMs' world modeling capabilities.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.06725)

- **Text2World: Benchmarking Large Language Models for Symbolic World Model Generation**
  - Publication: arXiv 2025
  - Highlights: First benchmark for evaluating LLMs' ability to generate symbolic world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.13092) | [Website](https://text-to-world.github.io/)

- **RAP: Reasoning with language model is planning with world model**
  - Publication: arXiv 2023
  - Highlights: Formalizes LLM reasoning as planning with a world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2305.14992)

- **LWM: World Model on Million-Length Video And Language With RingAttention**
  - Publication: arXiv 2024
  - Highlights: Million-length video and language world model based on RingAttention.
  - Paper Link: [arXiv](https://arxiv.org/abs/2402.08268) | [Code](https://github.com/LargeWorldModel/LWM)

- **Evaluating World Models with LLM for Decision Making**
  - Publication: arXiv 2024
  - Highlights: Evaluates world models using LLMs for decision-making tasks.
  - Paper Link: [arXiv](https://arxiv.org/abs/2411.08794)

- **LLMPhy: Complex Physical Reasoning Using Large Language Models and World Models**
  - Publication: arXiv 2024
  - Highlights: Combines LLMs and world models for complex physical reasoning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2411.08027)

- **LLMCWM: Language Agents Meet Causality – Bridging LLMs and Causal World Models**
  - Publication: arXiv 2024
  - Highlights: Bridges LLMs and causal world models for language agents with causal reasoning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.19923) | [Code](https://github.com/j0hngou/LLMCWM/)

- **Making Large Language Models into World Models with Precondition and Effect Knowledge**
  - Publication: arXiv 2024
  - Highlights: Transforms LLMs into world models using precondition and effect knowledge.
  - Paper Link: [arXiv](https://arxiv.org/abs/2409.12278)

- **CityBench: Evaluating the Capabilities of Large Language Model as World Model**
  - Publication: arXiv 2024
  - Highlights: Evaluates LLMs as city-level world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2406.13945) | [Code](https://github.com/tsinghua-fib-lab/CityBench)

### 4.2 Visual / Video World Models


- **Advancing Open-source World Models (LingBot-World)**
  - Publication: arXiv 2026
  - Highlights: Open-sourced world simulator stemming from video generation with high fidelity and robust dynamics.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.20540)

- **Infinite Worlds with Versatile Interactions (LingBot-World 2.0 / LingBot-World-Infinity)**
  - Publication: arXiv 2026
  - Highlights: Advanced iteration featuring unbounded interaction horizon, 60 fps 720p real-time rendering, diverse interactive elements, and agentic harness.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.07534) | WeChat: [link](https://mp.weixin.qq.com/s/c85iqjY_8EZQHPFdLaRIbw)

- **Next Forcing: Causal World Modeling with Multi-Chunk Prediction**
  - Publication: arXiv 2026
  - Highlights: Multi-chunk prediction framework enabling faster training, higher accuracy, and accelerated inference.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.11187)

- **Orca: The World is in Your Mind**
  - Publication: arXiv 2026
  - Highlights: BAAI's general world foundation model learning a unified latent space from multimodal signals; pre-trained on 125K hours of video and 160M event annotations.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.30534) | WeChat: [link](https://mp.weixin.qq.com/s/5G3Rc5o9yEThojhhECq2Lw)

- **Qwen-RobotWorld: Unifying Embodied World Modeling through Language-Conditioned Video Generation**
  - Publication: arXiv 2026
  - Highlights: Language-conditioned video world model predicting future visual trajectories across multiple robotic domains.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.17030) | WeChat: [link](https://mp.weixin.qq.com/s/EcOM534uHHJ8jwQ4sSK9og)

- **ABot-PhysWorld: Interactive World Foundation Model for Robotic Manipulation with Physics Alignment**
  - Publication: arXiv 2026
  - Highlights: 14B Diffusion Transformer generating visually realistic, physically plausible, and action-controllable videos.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.23376)

- **Nano World Models: A Minimalist Implementation of Future Video Prediction**
  - Publication: arXiv 2026
  - Highlights: Minimalist codebase centered around diffusion forcing with unified interface.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.23993)

- **A Mechanistic View on Video Generation as World Models: State and Dynamics**
  - Publication: arXiv 2026
  - Highlights: Taxonomy centered on State Construction and Dynamics Modeling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.17067)

- **Latent Video Prediction Learns Better World Models**
  - Publication: arXiv 2026
  - Highlights: First systematic study on robustness of latent-predictive video models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.15618)

- **PhyWorld: Physics-Faithful World Model for Video Generation**
  - Publication: arXiv 2026
  - Highlights: Two-stage post-training (flow matching + DPO physics preference alignment) for physically plausible scene continuations.
  - Paper Link: [arXiv](https://export.arxiv.org/abs/2605.19242)

- **Autonomous Video Generation with Counterfactual Controllability for Self-Evolving World Models**
  - Publication: arXiv 2026
  - Highlights: Achieves self-evolution of world models through counterfactual controllability.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.24152)

- **Directing the World: Fast Autoregressive Video Generation with Compositional Human-Camera Control**
  - Publication: arXiv 2026
  - Highlights: Fast autoregressive video generation via compositional human-camera control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.27964)

- **Causal Forcing: Autoregressive Diffusion Distillation for Real-Time Interactive Video Generation**
  - Publication: arXiv 2026
  - Highlights: Real-time interactive video generation via autoregressive diffusion distillation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.02214) | [Code](https://github.com/thu-ml/Causal-Forcing)

- **NeoVerse: Enhancing 4D World Model with in-the-wild Monocular Videos**
  - Publication: arXiv 2026
  - Highlights: Enhances 4D world models using in-the-wild monocular videos.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.00393) | [Website](https://neoverse-4d.github.io/)

- **Self-Forcing: Bridging the Train-Test Gap in Autoregressive Video Diffusion**
  - Publication: arXiv 2025
  - Highlights: Bridges the train-test gap in autoregressive video diffusion via self-forcing.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.08009) | [Code](https://github.com/guandeh17/Self-Forcing)

- **DFoT: History-Guided Video Diffusion**
  - Publication: arXiv 2025
  - Highlights: History-guided video diffusion model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.06764) | [Code](https://github.com/kwsong0113/diffusion-forcing-transformer)

- **SpaceTimePilot: Generative Rendering of Dynamic Scenes Across Space and Time**
  - Publication: arXiv 2025
  - Highlights: Generative rendering of dynamic scenes across space and time.
  - Paper Link: [arXiv](https://arxiv.org/abs/2512.25075) | [Code](https://github.com/ZheningHuang/spacetimepilot)

- **Diffusion Forcing: Next-token Prediction Meets Full-Sequence Diffusion**
  - Publication: arXiv 2024
  - Highlights: Unifies next-token prediction and full-sequence diffusion.
  - Paper Link: [arXiv](https://arxiv.org/abs/2407.01392) | [Website](https://boyuan.space/diffusion-forcing)

- **DisCo: World Models with Discrete Camera Motion Control**
  - Publication: arXiv 2026
  - Highlights: Discretizes continuous camera trajectories into action primitives for improved action separability; proposes the DisCoBench benchmark.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.07967)

- **Geometry-Aware Implicit Memory for Video World Models**
  - Publication: arXiv 2026
  - Highlights: Proposes a geometry-aware implicit memory framework that compresses variable-length histories into fixed-size memory tokens via a lightweight transformer.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.02436)

### 4.3 3D & 4D World Models (General Purpose)

*This section contains general-purpose 3D/4D generation and modeling paradigms. Application-specific models have been moved to Section 8.*



- **3D-Belief: Embodied Belief Inference via Generative 3D World Modeling**
  - Publication: arXiv 2026
  - Highlights: Redefines world modeling as embodied belief inference in 3D space.
  - Paper Link: [arXiv](https://export.arxiv.org/abs/2605.11367)

- **InSpatio-WorldFM: An Open-Source Real-Time Generative Frame Model**
  - Publication: arXiv 2026
  - Highlights: Real-time frame model with strong multi-view consistency, supports interactive exploration on consumer GPUs.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.11911)

- **InSpatio-World: A Real-Time 4D World Simulator via Spatiotemporal Autoregressive Modeling**
  - Publication: arXiv 2026
  - Highlights: Translates user interactions into camera trajectories for high-precision camera-controlled generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.07209)

- **HY-World 2.0: A Multi-Modal World Model for Reconstructing, Generating, and Simulating 3D Worlds**
  - Publication: arXiv 2026
  - Highlights: Multi-modal framework accommodating text, single/multi-view images, videos; outputs meshes / Gaussian Splattings.
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.14268)

- **DeepVerse: 4D Autoregressive Video Generation as a World Model**
  - Publication: arXiv 2025
  - Highlights: 4D autoregressive video generation as a world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.01103)

- **FantasyWorld: Geometry-Consistent World Modeling via Unified Video and 3D Prediction**
  - Publication: arXiv 2025
  - Highlights: Geometry-consistent world modeling via unified video and 3D prediction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.21657)

- **Aether: Geometric-Aware Unified World Modeling**
  - Publication: arXiv 2025
  - Highlights: Geometric-aware unified world modeling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.18945) | [Website](https://aether-world.github.io/)

- **WorldGrow: Generating Infinite 3D World**
  - Publication: arXiv 2025
  - Highlights: Generates infinite 3D worlds.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.21682) | [Code](https://github.com/world-grow/WorldGrow)

- **TRELLISWorld: Training-Free World Generation from Object Generators**
  - Publication: arXiv 2025
  - Highlights: Training-free world generation from object generators.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.23880)

- **Terra: Explorable Native 3D World Model with Point Latents**
  - Publication: arXiv 2025
  - Highlights: Explorable native 3D world model with point latents.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.14977) | [Website](https://huang-yh.github.io/terra/)

- **MorphoSim: Interactive, Controllable, Editable Language-guided 4D World Simulator**
  - Publication: arXiv 2025
  - Highlights: Interactive, controllable, editable language-guided 4D world simulator.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.04390) | [Code](https://github.com/eric-ai-lab/Morph4D)

- **EvoWorld: Evolving Panoramic World Generation with Explicit 3D Memory**
  - Publication: arXiv 2025
  - Highlights: Evolving panoramic world generation with explicit 3D memory.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.01183) | [Code](https://github.com/JiahaoPlus/EvoWorld)

- **HERO: Hierarchical Extrapolation and Refresh for Efficient World Models**
  - Publication: arXiv 2025
  - Highlights: Efficient world models via hierarchical extrapolation and refresh.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.17588)

- **UrbanWorld: An Urban World Model for 3D City Generation**
  - Publication: arXiv 2024
  - Highlights: Urban world model for 3D city generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2407.11965)

- **VGGT-World: Transforming VGGT into an Autoregressive Geometry World Model**
  - Publication: arXiv 2026
  - Highlights: Bypasses video generation to predict temporal evolution of frozen geometry foundation model features.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.12655)

- **3D Point World Models: Point Completion Enables More Accurate Dynamics Learning**
  - Publication: arXiv 2026
  - Highlights: Point cloud completion enables more accurate dynamics learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.00148)

- **Perceptual 3D Simulation With Physical World Modeling**
  - Publication: arXiv 2026
  - Highlights: Perceptual 3D simulation with physical world modeling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.27575)

- **PhysCoRe: Physics-Corrected Residual World Models for Material-Aware Deformable Dynamics**
  - Publication: arXiv 2026
  - Highlights: Physics-corrected residual world models for material-aware deformable dynamics.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.20653)

### 4.4 Latent Space World Models



- **Orca: The World is in Your Mind** (see also Visual section)
  - Highlights: Unified latent space from multimodal signals via unconscious and conscious learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.30534)

- **Looped World Models**
  - Publication: arXiv 2026
  - Highlights: First recurrent architecture iteratively refining latent states with shared transformer blocks, 100× parameter efficiency.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.18208)

- **EMERALD: Accurate and Efficient World Modeling with Masked Latent Transformers**
  - Publication: arXiv 2026
  - Highlights: Efficient world model with spatial latent states and MaskGIT prediction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.04075)

- **ThinkJEPA: Empowering Latent World Models with Large Vision-Language Reasoning Model**
  - Publication: arXiv 2026
  - Highlights: VLM-guided JEPA-style framework with dual temporal pathways.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.22281)

- **FF-JEPA: Long-Horizon Planning in World Models with Latent Planners**
  - Publication: arXiv 2026
  - Highlights: Forward-Forward JEPA unifying world models, prediction, and inverse dynamics.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.09311)

- **Kairos: A Native World Model Stack for Physical AI**
  - Publication: arXiv 2026
  - Highlights: Explicitly frameworks world models as systems learning physically meaningful predictive structures in abstract spaces.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.16533)

- **AdaJEPA: An Adaptive Latent World Model**
  - Publication: arXiv 2026
  - Highlights: Adaptive latent world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.32026) | [Website](https://agenticlearning.ai/adajepa/) | [Code](https://github.com/agentic-learning-ai-lab/adajepa)

- **EB-JEPA: Energy-Based Joint-Embedding Predictive Architectures**
  - Publication: arXiv 2026
  - Highlights: Energy-based joint-embedding predictive architectures.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.03604) | [Code](https://github.com/facebookresearch/eb_jepa)

- **V-JEPA 2.1: Unlocking Dense Features in Video Self-Supervised Learning**
  - Publication: arXiv 2026
  - Highlights: Unlocks dense features in video self-supervised learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.14482) | [Code](https://github.com/facebookresearch/vjepa2)

- **AWM: Learning Abstract World Models with a Group-Structured Latent Space**
  - Publication: arXiv 2025
  - Highlights: Learns abstract world models with a group-structured latent space.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.01529)

- **DINO-World: Back to the Features – DINO as a Foundation for Video World Models**
  - Publication: arXiv 2025
  - Highlights: Uses DINO features as a foundation for video world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.19468)

- **seq-JEPA: Autoregressive Predictive Learning of Invariant-Equivariant World Models**
  - Publication: arXiv 2025
  - Highlights: Autoregressive predictive learning of invariant-equivariant world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.03176)

- **V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning**
  - Publication: arXiv 2025
  - Highlights: Self-supervised video models enable understanding, prediction, and planning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.09985) | [Code](https://github.com/facebookresearch/vjepa2)

- **V-JEPA Learns Intuitive Physics**
  - Publication: arXiv 2025
  - Highlights: V-JEPA learns intuitive physics.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.11831) | [Code](https://github.com/facebookresearch/jepa-intuitive-physics)

- **DINO-WM: World Models on Pre-trained Visual Features enable Zero-shot Planning**
  - Publication: arXiv 2024
  - Highlights: World models on pre-trained visual features enable zero-shot planning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2411.04983) | [Website](https://dino-wm.github.io/)

- **DINO-Foresight: Looking into the Future with DINO**
  - Publication: arXiv 2024
  - Highlights: Looks into the future with DINO.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.11673) | [Code](https://github.com/Sta8is/DINO-Foresight)

- **I-JEPA: Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture**
  - Publication: arXiv 2023
  - Highlights: Self-supervised learning from images with a joint-embedding predictive architecture.
  - Paper Link: [arXiv](https://arxiv.org/abs/2301.08243)

- **IWM: Learning and Leveraging World Models in Visual Representation Learning**
  - Publication: arXiv 2024
  - Highlights: Learns and leverages world models in visual representation learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2403.00504)

- **V-JEPA: Video Joint Embedding Predictive Architecture** (Meta 2024)
  - Highlights: Meta's video joint embedding predictive architecture.
  - [Blog](https://ai.meta.com/blog/v-jepa-yann-lecun-ai-model-video-joint-embedding-predictive-architecture/) | [Code](https://github.com/facebookresearch/jepa)

- **MC-JEPA: Motion and Content Features via Joint-Embedding**
  - Publication: arXiv 2023
  - Highlights: Learns motion and content features via joint-embedding.
  - Paper Link: [arXiv](https://arxiv.org/abs/2307.12698)

### 4.5 Object-Centric World Models



- **Latent Particle World Models: Self-supervised Object-centric Stochastic Dynamics Modeling**
  - Publication: ICLR 2026 Oral
  - Highlights: Scales to real-world multi-object datasets for decision-making.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.04553)

- **OC-STORM: Objects matter – object-centric world models improve RL in visually complex environments**
  - Publication: arXiv 2025
  - Highlights: Object-centric world models improve RL in visually complex environments.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.16443)

- **Dyn-O: Building Structured World Models with Object-Centric Representations**
  - Publication: arXiv 2025
  - Highlights: Builds structured world models with object-centric representations.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.03298)

- **COMET: Compete and Compose – Learning Independent Mechanisms for Modular World Models**
  - Publication: arXiv 2024
  - Highlights: Learns independent mechanisms for modular world models via compete and compose.
  - Paper Link: [arXiv](https://arxiv.org/abs/2404.15109)

- **FPTT: Transformers and Slot Encoding for Sample Efficient Physical World Modelling**
  - Publication: arXiv 2024
  - Highlights: Transformers and slot encoding for sample-efficient physical world modeling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2405.20180) | [Code](https://github.com/torchipeppo/transformers-and-slot-encoding-for-wm)

- **Efficient Exploration and Discriminative World Model Learning with an Object-Centric Abstraction**
  - Publication: arXiv 2024
  - Highlights: Efficient exploration and discriminative world model learning with object-centric abstraction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2408.11816)

- **SlotFormer: Unsupervised Visual Dynamics Simulation with Object-Centric Models**
  - Publication: arXiv 2022
  - Highlights: Unsupervised visual dynamics simulation with object-centric models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2210.05861)

- **NPE: A Compositional Object-Based Approach to Learning Physical Dynamics**
  - Publication: arXiv 2016
  - Highlights: Compositional object-based approach to learning physical dynamics.
  - Paper Link: [arXiv](https://arxiv.org/abs/1612.00341)

### 4.6 Symbolic & Neuro-Symbolic World Models



- **OPINE-World: Programmatic World Modeling with Ontology-error-Prioritized Interactive Exploration**
  - Publication: arXiv 2026
  - Highlights: Programmatic world modeling with ontology-error-prioritized interactive exploration.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.01531)

- **Graph World Models: Concepts, Taxonomy, and Future Directions**
  - Publication: arXiv 2026
  - Highlights: Taxonomy based on relational inductive biases: spatial, physical, logical.
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.27895)

- **PoE-World: Compositional World Modeling with Products of Programmatic Experts**
  - Publication: arXiv 2025
  - Highlights: Compositional world modeling with products of programmatic experts.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.10819) | [Website](https://topwasu.github.io/poe-world)

- **One Life to Learn: Inferring Symbolic World Models for Stochastic Environments from Unguided Exploration**
  - Publication: arXiv 2025
  - Highlights: Infers symbolic world models for stochastic environments from unguided exploration.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.12088) | [Code](https://onelife-worldmodel.github.io/)

- **Finite Automata Extraction: Low-data World Model Learning as Programs from Gameplay Video**
  - Publication: arXiv 2025
  - Highlights: Low-data world model learning as programs from gameplay video.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.11836)

- **Synthesizing world models for bilevel planning**
  - Publication: arXiv 2025
  - Highlights: Synthesizes world models for bilevel planning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.20124)

- **Generating Symbolic World Models via Test-time Scaling of Large Language Models**
  - Publication: arXiv 2025
  - Highlights: Generates symbolic world models via test-time scaling of LLMs.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.04728) | [Website](https://vmlpddl.github.io/)

- **Neuro-Symbolic World Models for Adapting to Open World Novelty**
  - Publication: arXiv 2023
  - Highlights: Neuro-symbolic world models for adapting to open world novelty.
  - Paper Link: [arXiv](https://arxiv.org/abs/2301.06294)

### 4.7 General Foundation World Models



- **Cosmos 3: Omnimodal World Models for Physical AI**
  - Publication: arXiv 2026
  - Highlights: NVIDIA's omnimodal world models for Physical AI.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.02800) | [Code](https://github.com/nvidia/cosmos)

- **DreamX-World 1.0: A General-Purpose Interactive World Model**
  - Publication: arXiv 2026
  - Highlights: General-purpose interactive world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.16993) | [Code](https://github.com/AMAP-ML/DreamX-World)

- **DreamZero: World Action Models are Zero-shot Policies**
  - Publication: arXiv 2026
  - Highlights: World action models are zero-shot policies.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.15922) | [Code](https://github.com/dreamzero0/dreamzero)

- **SANA-WM: Efficient Minute-Scale World Modeling with Hybrid Linear Diffusion Transformer**
  - Publication: arXiv 2025
  - Highlights: Efficient minute-scale world modeling with hybrid linear diffusion transformer.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.15178) | [Website](https://nvlabs.github.io/Sana/WM/)

- **PAN: A World Model for General, Interactable, and Long-Horizon World Simulation**
  - Publication: arXiv 2025
  - Highlights: General, interactable, and long-horizon world simulation model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2511.09057) | [Website](https://panworld.ai/)

- **Cosmos World Foundation Model Platform for Physical AI**
  - Publication: arXiv 2025
  - Highlights: NVIDIA's Cosmos world foundation model platform for Physical AI.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.03575) | [Code](https://github.com/nvidia-cosmos)

- **Genie 3: A new frontier for world models**
  - Highlights: Google DeepMind's Genie 3, a new frontier for world models.
  - [Blog](https://deepmind.google/discover/blog/genie-3-a-new-frontier-for-world-models/)

- **Genie 2: A Large-Scale Foundation World Model**
  - Highlights: Google DeepMind's large-scale foundation world model.
  - [Blog](https://deepmind.google/discover/blog/genie-2-a-large-scale-foundation-world-model/)

- **Genie: Generative Interactive Environments**
  - Publication: arXiv 2024
  - Highlights: Google DeepMind's generative interactive environments.
  - Paper Link: [arXiv](https://arxiv.org/abs/2402.15391) | [Website](https://sites.google.com/view/genie-2024/home)

- **Emu3.5: Native Multimodal Models are World Learners**
  - Publication: arXiv 2025
  - Highlights: Native multimodal models are world learners.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.26583) | [Website](https://emu.world/pages/web/landingPage)

- **Emu3: Next-Token Prediction is All You Need**
  - Publication: arXiv 2024
  - Highlights: BAAI's Emu3, demonstrating next-token prediction unifies multimodal tasks.
  - Paper Link: [arXiv](https://arxiv.org/abs/2409.18869) | [Code](https://github.com/baaivision/Emu3)

- **Video models are zero-shot learners and reasoners**
  - Publication: arXiv 2025
  - Highlights: Veo-3 as zero-shot learners and reasoners.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.20328) | [Website](https://video-zero-shot.github.io/)

- **UniSim: Learning Interactive Real-World Simulators**
  - Publication: arXiv 2023
  - Highlights: Learns interactive real-world simulators.
  - Paper Link: [arXiv](https://arxiv.org/abs/2310.06114) | [Website](https://universal-simulator.github.io/unisim/)

- **Pandora: Towards General World Model with Natural Language Actions and Video States**
  - Publication: arXiv 2024
  - Highlights: General world model with natural language actions and video states.
  - Paper Link: [arXiv](https://arxiv.org/abs/2406.09455) | [Code](https://github.com/maitrix-org/Pandora)

- **RTFM: A Real-Time Frame Model** (World Labs)
  - Highlights: World Labs' real-time frame model.
  - [Blog](https://www.worldlabs.ai/blog/rtfm)

- **Marble: Generating Bigger and Better Worlds** (World Labs)
  - Highlights: World Labs' bigger and better worlds generation.
  - [Blog](https://www.worldlabs.ai/blog/bigger-better-worlds)

- **WorldGen: From Text to Traversable and Interactive 3D Worlds** (Meta)
  - Highlights: Meta's generation from text to traversable and interactive 3D worlds.
  - [Blog](https://www.meta.com/blog/worldgen-3d-world-generation-reality-labs-generative-ai-research) | [Paper](https://scontent-sea1-1.xx.fbcdn.net/v/t39.2365-6/586830145_834419405978070_3937417229378696315_n.pdf)

- **Generating Worlds** (World Labs)
  - Highlights: World Labs' world generation technology.
  - [Blog](https://www.worldlabs.ai/blog/generating-worlds)

- **Astra: General Interactive World Model with Autoregressive Denoising**
  - Publication: ICLR 2026
  - Highlights: General interactive world model with autoregressive denoising.
  - Paper Link: [arXiv](https://arxiv.org/abs/2512.08931)

---

## 🎮 Interactive World Models

### 5.1 General Interactive Frameworks



- **Qwen-AgentWorld: Language World Models for General Agents**
  - Publication: arXiv 2026
  - Highlights: First native language world models (35B-A3B and 397B-A17B) simulating agentic environments across 7 domains via long CoT reasoning, trained on >10M interaction trajectories.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.24597)

- **Advancing Open-source World Models (LingBot-World)**
  - Publication: arXiv 2026
  - Highlights: Open-sourced world simulator stemming from video generation with high fidelity and robust dynamics.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.20540)

- **Infinite Worlds with Versatile Interactions (LingBot-World 2.0 / LingBot-World-Infinity)**
  - Publication: arXiv 2026
  - Highlights: Advanced iteration featuring unbounded interaction horizon, 60 fps 720p real-time rendering, diverse interactive elements, and agentic harness.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.07534) | WeChat: [link](https://mp.weixin.qq.com/s/c85iqjY_8EZQHPFdLaRIbw)

- **ActWorld: From Explorable to Interactive World Model via Action-Aware Memory**
  - Publication: arXiv 2026
  - Highlights: Extends navigation-centric generators to support object interactions.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.17730)

- **MoWorld: A Flash World Model**
  - Publication: arXiv 2026
  - Highlights: First NPU-based real-time interactive world model achieving 50 FPS with 30%-50% inference cost.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.06216)

- **WorldDirector: Building Controllable World Simulators with Persistent Dynamic Memory**
  - Publication: arXiv 2026
  - Highlights: Decouples semantic motion orchestration from visual generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.02517)

- **Stateful Worlds, Stateless Elasticity: Exact-State Serving for Interactive World Models**
  - Publication: arXiv 2026
  - Highlights: WorldMove enables live session migration within 18.8ms.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.10389)

- **From Pixels to States: Rethinking Interactive World Models as Game Engines**
  - Publication: arXiv 2026
  - Highlights: Examines interactive game world modeling along four dimensions.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.14076)

- **Vid2World: Crafting Video Diffusion Models to Interactive World Models**
  - Publication: arXiv 2025
  - Highlights: Crafts video diffusion models into interactive world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.14357) | [Website](http://knightnemo.github.io/vid2world/)

- **AVID: Adapting Video Diffusion Models to World Models**
  - Publication: arXiv 2024
  - Highlights: Adapts video diffusion models to world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.12822) | [Code](https://github.com/microsoft/causica/tree/main/research_experiments/avid)

- **IRASim: A Fine-Grained World Model for Robot Manipulation**
  - Publication: arXiv 2024
  - Highlights: Fine-grained world model for robot manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2406.14540) | [Website](https://gen-irasim.github.io/)

- **DWS: Pre-Trained Video Generative Models as World Simulators**
  - Publication: arXiv 2025
  - Highlights: Pre-trained video generative models as world simulators.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.07825)

- **Video Adapter: Probabilistic Adaptation of Black-Box Text-to-Video Models**
  - Highlights: Probabilistic adaptation of black-box text-to-video models.
  - [OpenReview](https://openreview.net/forum?id=pjtIEgscE3) | [Website](https://video-adapter.github.io/video-adapter/)

- **VideoAgent: Self-Improving Video Generation**
  - Publication: arXiv 2024
  - Highlights: Self-improving video generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.10076) | [Website](https://video-as-agent.github.io/)

- **WISA: World Simulator Assistant for Physics-Aware Text-to-Video Generation**
  - Publication: arXiv 2025
  - Highlights: World simulator assistant for physics-aware text-to-video generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.08153) | [Code](https://github.com/360CVGroup/WISA)

- **Force Prompting: Video Generation Models Can Learn and Generalize Physics-based Control Signals**
  - Publication: arXiv 2025
  - Highlights: Video generation models can learn and generalize physics-based control signals.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.19386) | [Code](https://github.com/brown-palm/force-prompting)

- **Infinite-World: Scaling Interactive World Models to 1000-Frame Horizons via Pose-Free Hierarchical Memory**
  - Publication: arXiv 2026
  - Highlights: Scales interactive world models to 1000-frame horizons via pose-free hierarchical memory.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.02393)

### 5.2 Game & Open-World Exploration (Application)

*This section merges the original 5.2 and the removed 8.6, serving as the dedicated application subsection for interactive world models in gaming.*



- **What if? Emulative Simulation with World Models for Situated Reasoning (WanderDream)**
  - Publication: arXiv 2026
  - Highlights: First large-scale dataset for emulative simulation of mental exploration.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.06445)

- **MIRA: Multiplayer Interactive World Models with Representation Autoencoders**
  - Publication: arXiv 2026
  - Highlights: Multiplayer interactive world models with representation autoencoders.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.05352) | [Website](https://mira-wm.com/) | [Code](https://github.com/mira-wm/mira)

- **Solaris: Building a Multiplayer Video World Model in Minecraft**
  - Publication: arXiv 2026
  - Highlights: Builds a multiplayer video world model in Minecraft.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.22208) | [Website](https://solaris-wm.github.io/) | [Code](https://github.com/solaris-wm/solaris)

- **Matrix-Game 3.0: Real-Time and Streaming Interactive World Model with Long-Horizon Memory**
  - Publication: arXiv 2026
  - Highlights: Real-time and streaming interactive world model with long-horizon memory.
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.08995) | [Website](https://matrix-game-v3.github.io/) | [Code](https://github.com/SkyworkAI/Matrix-Game/tree/main/Matrix-Game-3)

- **SCOPE: Simulating Cross-game Operations in Playable Environments for FPS World Models**
  - Publication: arXiv 2025
  - Highlights: Simulates cross-game operations in playable environments for FPS world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.23345) | [Website](https://z2tong.github.io/SCOPE/) | [Code](https://github.com/z2tong/SCOPE)

- **Matrix-Game 2.0: An Open-Source, Real-Time, and Streaming Interactive World Model**
  - Publication: arXiv 2025
  - Highlights: Open-source, real-time, and streaming interactive world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.13009) | [Website](https://matrix-game-v2.github.io/)

- **Matrix-Game: Interactive World Foundation Model**
  - Publication: arXiv 2025
  - Highlights: Interactive world foundation model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.18701) | [Code](https://github.com/SkyworkAI/Matrix-Game)

- **RealPlay: From Virtual Games to Real-World Play**
  - Publication: arXiv 2025
  - Highlights: From virtual games to real-world play.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.18901) | [Website](https://wenqsun.github.io/RealPlay/) | [Code](https://github.com/wenqsun/Real-Play)

- **GameFactory: Creating New Games with Generative Interactive Videos**
  - Publication: arXiv 2025
  - Highlights: Creates new games with generative interactive videos.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.08325) | [Website](https://yujiwen.github.io/gamefactory/) | [Code](https://github.com/KwaiVGI/GameFactory)

- **WORLDMEM: Long-term Consistent World Simulation with Memory**
  - Publication: arXiv 2025
  - Highlights: Long-term consistent world simulation with memory.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.12369) | [Website](https://xizaoqu.github.io/worldmem/) | [Code](https://github.com/xizaoqu/WorldMem)

- **MineWorld: a Real-Time and Open-Source Interactive World Model on Minecraft**
  - Publication: arXiv 2025
  - Highlights: Real-time and open-source interactive world model on Minecraft.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.08388) | [Website](https://aka.ms/mineworld)

- **AnimeGamer: Infinite Anime Life Simulation with Next Game State Prediction**
  - Publication: arXiv 2025
  - Highlights: Infinite anime life simulation with next game state prediction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.01014) | [Website](https://howe125.github.io/AnimeGamer.github.io/)

- **HunyuanWorld 1.0: Generating Immersive, Explorable, and Interactive 3D Worlds from Words or Pixels**
  - Publication: arXiv 2025
  - Highlights: Generates immersive, explorable, and interactive 3D worlds from words or pixels.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.21809) | [Website](https://3d-models.hunyuan.tencent.com/world/) | [Code](https://github.com/Tencent-Hunyuan/HunyuanWorld-1.0)

- **Matrix-3D: Omnidirectional Explorable 3D World Generation**
  - Publication: arXiv 2025
  - Highlights: Omnidirectional explorable 3D world generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.08086) | [Website](https://matrix-3d.github.io)

- **Waypoint-1: The Path to Real-Time Worlds and Why It Matters**
  - Highlights: The path to real-time worlds.
  - [Blog](https://over.world/blog/the-path-to-real-time-worlds-and-why-it-matters)

- **GameNGen: Diffusion Models Are Real-Time Game Engines**
  - Publication: arXiv 2024
  - Highlights: Diffusion models are real-time game engines.
  - Paper Link: [arXiv](https://arxiv.org/abs/2408.14837)

- **DIAMOND: Diffusion for World Modeling: Visual Details Matter in Atari**
  - Publication: arXiv 2024
  - Highlights: Visual details matter in Atari for diffusion world modeling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2405.12399) | [Code](https://github.com/eloialonso/diamond)

---

## 🤖 World Action Models (WAM) & VLA Integration

### 6.1 Cascaded WAM



- **Flash-WAM: Modality-Aware Distillation for World Action Models**
  - Publication: arXiv 2026
  - Highlights: Compresses WAM inference to a single step per modality, 348× speedup on RoboTwin 2.0.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.05254)

### 6.2 Joint WAM & Unified VLA-World Models

*This section merges the original 6.2 Joint WAM and the "Unifying" sub-section from the original 8.1.5. It focuses on paradigms that jointly model video generation, world state prediction, and action decision-making within a single architecture.*



- **Native Video-Action Pretraining for Generalizable Robot Control (LingBot-VA 2.0)**
  - Publication: arXiv 2026
  - Highlights: Video-action foundation model with semantic visual-action tokenizer, causal pretraining, sparse MoE.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.08639) | WeChat: [link](https://mp.weixin.qq.com/s/YI7j20M11WanZSlartWPwA)

- **DiM-WAM: World Action Modeling with Diverse Historical Event Memory**
  - Publication: arXiv 2026
  - Highlights: Augments WAM with Diverse Historical Event Memory (DHEM).
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.27677)

- **WorldBagel: Uncovering the Power of Unified Multimodal Models for Vision-Language-Action-World Modeling**
  - Publication: arXiv 2026
  - Highlights: Unified VLAW framework outperforming task-specific alternatives.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.03461)

- **GigaWorld-Policy-0.5: A Faster and Stronger WAM Empowered by AutoResearch**
  - Publication: arXiv 2026
  - Highlights: Faster and stronger WAM with a mixture-of-experts transformer architecture, achieving 85ms inference latency on RTX 4090.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.13960) | [Website](https://open-gigaai.github.io/giga-world-policy/) | [Code](https://github.com/open-gigaai/giga-world-policy)

- **EgoWAM: World Action Models Beyond Pixels with In-the-Wild Egocentric Human Data**
  - Publication: arXiv 2026
  - Highlights: World action models beyond pixels using in-the-wild egocentric human data.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.08436) | [Website](https://gatech-rl2.github.io/egowam.github.io/)

- **WAM-TTT: Steering World-Action Models by Watching Human Play at Test Time**
  - Publication: arXiv 2026
  - Highlights: Steers world-action models by watching human play at test time.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.06988)

- **FlowWAM: Optical Flow as a Unified Action Representation for World Action Models**
  - Publication: arXiv 2026
  - Highlights: Optical flow as a unified action representation for WAMs.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.13017) | [Website](https://flow-wam.github.io/) | [Code](https://github.com/YixiangChen515/FlowWAM)

- **ABot-M0.5: Unified Mobility-and-Manipulation World Action Model**
  - Publication: arXiv 2026
  - Highlights: Unified mobility-and-manipulation WAM aligning time granularity, action space, and train-test consistency.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.00678) | [Code](https://github.com/amap-cvlab/ABot-Manipulation)

- **LDA-1B: Scaling Latent Dynamics Action Model via Universal Embodied Data Ingestion**
  - Publication: arXiv 2026
  - Highlights: Scales latent dynamics action model via universal embodied data ingestion.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.12215) | [Website](https://pku-epic.github.io/LDA/) | [Code](https://github.com/jiangranlv/latent-dynamics-action)

- **LingBot-VA: Causal video-action world model for generalist robot control**
  - Publication: arXiv 2026
  - Highlights: Causal video-action world model for generalist robot control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.21998) | [Website](https://technology.robbyant.com/lingbot-va) | [Code](https://github.com/Robbyant/lingbot-va)

- **UWM: Unified World Models – Coupling Video and Action Diffusion for Pretraining on Large Robotic Datasets**
  - Publication: arXiv 2025
  - Highlights: Couples video and action diffusion for pretraining on large robotic datasets.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.02792) | [Website](https://weirdlabuw.github.io/uwm/)

- **UVA: Unified Video Action Model**
  - Publication: arXiv 2025
  - Highlights: Unified video action model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.00200) | [Website](https://unified-video-action-model.github.io/) | [Code](https://github.com/ShuangLI59/unified_video_action)

- **DiWA: Diffusion Policy Adaptation with World Models**
  - Publication: arXiv 2025
  - Highlights: Diffusion policy adaptation with world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.03645) | [Code](https://diwa.cs.uni-freiburg.de)

- **Learning Latent Action World Models In The Wild**
  - Publication: arXiv 2026
  - Highlights: Learns latent action world models in the wild.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.05230)

- **InternVLA-A1.5: Unifying Understanding, Latent Foresight, and Action for Compositional Generalization**
  - Publication: arXiv 2026
  - Highlights: Unifies understanding, latent foresight, and action for compositional generalization.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.04988) | [Website](https://internrobotics.github.io/internvla-a15.github.io/) | [Code](https://github.com/InternRobotics/InternVLA-A-series)

- **VLA-JEPA: Enhancing Vision-Language-Action Model with Latent World Model**
  - Publication: arXiv 2026
  - Highlights: Enhances VLA with a latent world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.10098) | [Website](https://ginwind.github.io/VLA-JEPA/) | [Code](https://github.com/ginwind/VLA-JEPA)

- **WorldVLA: Towards Autoregressive Action World Model**
  - Publication: arXiv 2025
  - Highlights: Towards autoregressive action world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.21539) | [Code](https://github.com/alibaba-damo-academy/WorldVLA)

- **MinD: Unified Visual Imagination and Control via Hierarchical World Models**
  - Publication: arXiv 2025
  - Highlights: Unified visual imagination and control via hierarchical world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.18897) | [Website](https://manipulate-in-dream.github.io/)

- **DreamVLA: A Vision-Language-Action Model Dreamed with Comprehensive World Knowledge**
  - Publication: arXiv 2025
  - Highlights: VLA dreamed with comprehensive world knowledge.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.04447) | [Code](https://github.com/Zhangwenyao1/DreamVLA) | [Website](https://zhangwenyao1.github.io/DreamVLA/)

- **VPP: Video Prediction Policy – A Generalist Robot Policy with Predictive Visual Representations**
  - Publication: arXiv 2024
  - Highlights: Generalist robot policy with predictive visual representations.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.14803) | [Website](https://video-prediction-policy.github.io)

- **UP-VLA: A Unified Understanding and Prediction Model for Embodied Agent**
  - Publication: arXiv 2025
  - Highlights: Unified understanding and prediction model for embodied agents.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.18867) | [Code](https://github.com/CladernyJorn/UP-VLA)

- **CoT-VLA: Visual Chain-of-Thought Reasoning for Vision-Language-Action Models**
  - Publication: arXiv 2025
  - Highlights: Visual chain-of-thought reasoning for VLAs.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.22020) | [Website](https://cot-vla.github.io/)

- **3D-VLA: A 3D Vision-Language-Action Generative World Model**
  - Publication: arXiv 2024
  - Highlights: 3D vision-language-action generative world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2403.09631)

- **LAWM: Latent Action Pretraining Through World Modeling**
  - Publication: arXiv 2025
  - Highlights: Latent action pretraining through world modeling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.18428) | [Code](https://github.com/baheytharwat/lawm)

- **UniVLA: Unified Vision-Language-Action Model**
  - Publication: arXiv 2025
  - Highlights: Unified vision-language-action model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.19850) | [Code](https://robertwyq.github.io/univla.github.)

- **dVLA: Diffusion Vision-Language-Action Model with Multimodal Chain-of-Thought**
  - Publication: arXiv 2025
  - Highlights: Diffusion VLA with multimodal chain-of-thought.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.25681)

- **UD-VLA: Unified Diffusion VLA via Joint Discrete Denoising Diffusion Process**
  - Publication: arXiv 2025
  - Highlights: Unified diffusion VLA via joint discrete denoising diffusion process.
  - Paper Link: [arXiv](https://arxiv.org/abs/2511.01718) | [Code](https://github.com/OpenHelix-Team/UD-VLA) | [Website](https://irpn-eai.github.io/UD-VLA.github.io/)

- **Goal-VLA: Image-Generative VLMs as Object-Centric World Models Empowering Zero-shot Robot Manipulation**
  - Publication: arXiv 2025
  - Highlights: Image-generative VLMs as object-centric world models empowering zero-shot manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.23919) | [Website](https://nus-lins-lab.github.io/goalvlaweb/)

- **Vidarc: Embodied Video Diffusion Model for Closed-loop Control**
  - Publication: arXiv 2025
  - Highlights: Embodied video diffusion model for closed-loop control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2512.17661)

- **VideoVLA: Video Generators Can Be Generalizable Robot Manipulators**
  - Publication: arXiv 2025
  - Highlights: Video generators as generalizable robot manipulators.
  - Paper Link: [arXiv](https://arxiv.org/abs/2512.06963) | [Website](https://videovla-nips2025.github.io)

- **Motus: A Unified Latent Action World Model**
  - Publication: arXiv 2025
  - Highlights: Unified latent action world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2512.13030) | [Website](https://motus-robotics.github.io/motus)

- **mimic-video: Video-Action Models for Generalizable Robot Control Beyond VLAs**
  - Publication: arXiv 2025
  - Highlights: Video-action models for generalizable robot control beyond VLAs.
  - Paper Link: [arXiv](https://arxiv.org/abs/2512.15692) | [Website](https://mimic-video.github.io)

### 6.3 World Models for VLA Training & Evaluation (Combining Paradigms)

*This section merges the original 6.3 and the "Combining" sub-section from the original 8.1.5. It focuses on using world models as environments/simulators to assist in training, fine-tuning, or evaluating VLA policies (i.e., "world model as environment" rather than "world model as policy").*



- **WEAVER: Better, Faster, Longer: An Effective World Model for Robotic Manipulation**
  - Publication: arXiv 2026
  - Highlights: Multi-view WM with flow-matching loss, SOTA on robotic manipulation, satisfying fidelity, consistency, and efficiency.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.13672)

- **PAIWorld: A 3D-Consistent World Foundation Model for Robotic Manipulation**
  - Publication: arXiv 2026
  - Highlights: DiT-based foundation model, ranked 1st on WorldArena and 2nd on AgiBot-Challenge2026.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.18375)

- **WAM-RL: World-Action Model Reinforcement Learning with Reconstruction Rewards and Online Video SFT**
  - Publication: arXiv 2026
  - Highlights: First RL in World-Action paradigm jointly optimizing world and action models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.17906)

- **Reinforcing VLAs in Task-Agnostic World Models (RAW-Dream)**
  - Publication: arXiv 2026
  - Highlights: Completely decouples world model learning from downstream task dependencies.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.12334)

- **RoboDream: Compositional World Models for Scalable Robot Data Synthesis**
  - Publication: arXiv 2026
  - Highlights: Generalizable embodiment-centric world model for scalable data generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.02577)

- **Hi-WM: Human-in-the-World-Model for Scalable Robot Post-Training**
  - Publication: arXiv 2026
  - Highlights: Post-training framework using learned world model as corrective substrate.
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.21741)

- **Ctrl-World: A Controllable Generative World Model for Robot Manipulation**
  - Publication: arXiv 2025
  - Highlights: Controllable generative world model for robot manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.10125) | [Website](https://ctrl-world.github.io/) | [Code](https://github.com/Robert-gyj/Ctrl-World)

- **VLA-RFT: Vision-Language-Action Reinforcement Fine-tuning with Verified Rewards in World Simulators**
  - Publication: arXiv 2025
  - Highlights: VLA reinforcement fine-tuning with verified rewards in world simulators.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.00406)

- **World-Env: Leveraging World Model as a Virtual Environment for VLA Post-Training**
  - Publication: arXiv 2025
  - Highlights: Leveraging world models as virtual environments for VLA post-training.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.24948)

- **Self-Improving Embodied Foundation Models**
  - Publication: arXiv 2025
  - Highlights: Self-improving embodied foundation models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.15155)

- **GigaBrain-0.5M\*: a VLA That Learns From World Model-Based Reinforcement Learning**
  - Publication: arXiv 2026
  - Highlights: VLA that learns from world model-based RL.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.12099) | [Website](https://gigabrain05m.github.io/) | [Code](https://github.com/open-gigaai/giga-brain-0)

- **RISE: Self-Improving Robot Policy with Compositional World Model**
  - Publication: arXiv 2026
  - Highlights: Self-improving robot policy with compositional world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.11075) | [Website](https://opendrivelab.com/kai0-rl/)

- **GigaBrain-0: A World Model-Powered Vision-Language-Action Model**
  - Publication: arXiv 2025
  - Highlights: World model-powered VLA.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.19430) | [Website](https://gigabrain0.github.io/)

- **WMPO: World Model-based Policy Optimization for Vision-Language-Action Models**
  - Publication: arXiv 2025
  - Highlights: World model-based policy optimization for VLAs.
  - Paper Link: [arXiv](https://arxiv.org/abs/2511.09515) | [Website](https://wm-po.github.io)

---

## 🧪 Model-Based RL World Models

### 7.1 Classic Series



- **DreamerV4: Training Agents Inside of Scalable World Models**
  - Publication: arXiv 2025
  - Highlights: Trains agents inside of scalable world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.24527) | [Website](https://danijar.com/project/dreamer4/)

- **DreamerV3: Mastering Diverse Domains through World Models**
  - Publication: arXiv 2023
  - Highlights: Masters diverse domains through world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2301.04104) | [Code](https://github.com/danijar/dreamerv3) | [Website](https://danijar.com/project/dreamerv3/)

- **TD-MPC2: Scalable, Robust World Models for Continuous Control**
  - Publication: arXiv 2023
  - Highlights: Scalable, robust world models for continuous control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2310.16828) | [Torch Code](https://github.com/nicklashansen/tdmpc2)

- **DreamerV2: Mastering Atari with Discrete World Models**
  - Publication: arXiv 2020
  - Highlights: Masters Atari with discrete world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2010.02193) | [Code](https://github.com/danijar/dreamerv2) | [Website](https://danijar.com/project/dreamerv2/)

- **Dreamer: Dream to Control: Learning Behaviors by Latent Imagination**
  - Publication: arXiv 2019
  - Highlights: Learns behaviors by latent imagination.
  - Paper Link: [arXiv](https://arxiv.org/abs/1912.01603) | [Code](https://github.com/danijar/dreamer) | [Website](https://danijar.com/project/dreamer/)

### 7.2 Continuous Control



- **Scaling World-Model Reinforcement Learning Through Diffusion Policy Optimization**
  - Publication: arXiv 2026
  - Highlights: Unifies search and policy optimization via diffusion policy representation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.26282)

- **JEDI: Joint Embedding Diffusion World Model for Online Model-Based Reinforcement Learning**
  - Publication: arXiv 2026
  - Highlights: Joint embedding diffusion world model for online MBRL.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2605.13013)

- **ACID: Action Consistency via Inverse Dynamics for Planning with World Models**
  - Publication: arXiv 2026
  - Highlights: Action consistency via inverse dynamics for planning with world models.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2607.02403)

- **DyMoDreamer: World Modeling with Dynamic Modulation**
  - Publication: arXiv 2025
  - Highlights: World modeling with dynamic modulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.24804) | [Code](https://github.com/Ultraman-Tiga1/DyMoDreamer)

- **MoSim: Neural Motion Simulator Pushing the Limit of World Models in RL**
  - Publication: arXiv 2025
  - Highlights: Neural motion simulator pushing the limit of world models in RL.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.07095)

- **HarmonyDream: Task Harmonization Inside World Models**
  - Publication: arXiv 2023
  - Highlights: Task harmonization inside world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2310.00344) | [Code](https://github.com/thuml/HarmonyDream)

- **Δ-IRIS: Efficient World Models with Context-Aware Tokenization**
  - Publication: arXiv 2024
  - Highlights: Efficient world models with context-aware tokenization.
  - Paper Link: [arXiv](https://arxiv.org/abs/2406.19320) | [Code](https://github.com/vmicheli/delta-iris)

- **AD3: Implicit Action is the Key for World Models to Distinguish the Diverse Visual Distractors**
  - Publication: arXiv 2024
  - Highlights: Implicit action is the key for world models to distinguish diverse visual distractors.
  - Paper Link: [arXiv](https://arxiv.org/abs/2403.09976)

- **R2I: Mastering Memory Tasks with World Models**
  - Publication: arXiv 2024
  - Highlights: Masters memory tasks with world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2403.04253) | [Website](https://recall2imagine.github.io/) | [Code](https://github.com/chandar-lab/Recall2Imagine)

- **REM: Improving Token-Based World Models with Parallel Observation Prediction**
  - Publication: arXiv 2024
  - Highlights: Improves token-based world models with parallel observation prediction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2402.05643) | [Code](https://github.com/leor-c/REM)

- **AWM: Do Transformer World Models Give Better Policy Gradients?**
  - Publication: arXiv 2024
  - Highlights: Investigates whether transformer world models give better policy gradients.
  - Paper Link: [arXiv](https://arxiv.org/abs/2402.05290)

- **Hieros: Hierarchical Imagination on Structured State Space Sequence World Models**
  - Publication: arXiv 2023
  - Highlights: Hierarchical imagination on structured state space sequence world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2310.05167)

- **DreamSmooth: Improving Model-based Reinforcement Learning via Reward Smoothing**
  - Publication: arXiv 2023
  - Highlights: Improves MBRL via reward smoothing.
  - Paper Link: [arXiv](https://arxiv.org/abs/2311.01450)

### 7.3 Offline & Generalization



- **CoMap: Co-Evolving World Models and Agent Policies for LLM Agents**
  - Publication: arXiv 2026
  - Highlights: Co-evolves textual world models and agent policies through closed-loop interaction.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2606.02372)

- **Policy and World Modeling Co-Training for Language Agents (PaW)**
  - Publication: arXiv 2026
  - Highlights: Adds auxiliary WM supervision to policy during RL without changing inference.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.02388)

- **ROMBRL: Policy-Driven World Model Adaptation for Robust Offline Model-based RL**
  - Publication: arXiv 2025
  - Highlights: Policy-driven world model adaptation for robust offline MBRL.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.13709)

- **SENSEI: Semantic Exploration Guided by Foundation Models to Learn Versatile World Models**
  - Publication: arXiv 2025
  - Highlights: Semantic exploration guided by foundation models to learn versatile world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.01584) | [Website](https://sites.google.com/view/sensei-paper)

- **Spiking World Model: Implementing Spiking World Model with Multi-Compartment Neurons for MBRL**
  - Publication: arXiv 2025
  - Highlights: Implements spiking world models with multi-compartment neurons for MBRL.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.00713)

- **DCWM: Discrete Codebook World Models for Continuous Control**
  - Publication: arXiv 2025
  - Highlights: Discrete codebook world models for continuous control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.00653)

- **Multimodal Dreaming: A Global Workspace Approach to World Model-Based RL**
  - Publication: arXiv 2025
  - Highlights: Global workspace approach to world model-based RL.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.21142)

- **Learning To Explore With Predictive World Model Via Self-Supervised Learning**
  - Publication: arXiv 2025
  - Highlights: Learns to explore with predictive world models via self-supervised learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.13200)

- **Simulus: Combining Improvements in Sample-Efficient World Model Agents**
  - Publication: arXiv 2025
  - Highlights: Uncovers untapped potential in sample-efficient world model agents.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2502.11537)

- **DMWM: Dual-Mind World Model with Long-Term Imagination**
  - Publication: arXiv 2025
  - Highlights: Dual-mind world model with long-term imagination.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.07591)

- **EvolvingAgent: Curriculum Self-evolving Agent with Continual World Model for Long-Horizon Tasks**
  - Publication: arXiv 2025
  - Highlights: Agent autonomous evolution with continual world model for long-horizon tasks.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.05907)

- **CoWorld: Making Offline RL Online: Collaborative World Models for Offline Visual RL**
  - Publication: arXiv 2023
  - Highlights: Collaborative world models for offline visual RL.
  - Paper Link: [arXiv](https://arxiv.org/abs/2305.15260)

- **Dreaming of Many Worlds: Learning Contextual World Models Aids Zero-Shot Generalization**
  - Publication: arXiv 2024
  - Highlights: Learning contextual world models aids zero-shot generalization.
  - Paper Link: [arXiv](https://arxiv.org/abs/2403.10967) | [Code](https://github.com/sai-prasanna/dreaming_of_many_worlds)

- **PWM: Policy Learning with Multi-Task World Models**
  - Publication: arXiv 2024
  - Highlights: Policy learning with large world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2407.02466) | [Code](https://www.imgeorgiev.com/pwm/)

- **GenRL: Multimodal foundation world models for generalist embodied agents**
  - Publication: arXiv 2024
  - Highlights: Multimodal foundation world models for generalist embodied agents.
  - Paper Link: [arXiv](https://arxiv.org/abs/2406.18043) | [Code](https://github.com/mazpie/genrl)

- **Adaptive World Models: Learning Behaviors by Latent Imagination Under Non-Stationarity**
  - Publication: arXiv 2024
  - Highlights: Learns behaviors by latent imagination under non-stationarity.
  - Paper Link: [arXiv](https://arxiv.org/abs/2411.01342)

- **Reward-free World Models for Online Imitation Learning**
  - Publication: arXiv 2024
  - Highlights: Reward-free world models for online imitation learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.14081)

- **MoReFree: Reset-free Reinforcement Learning with World Models**
  - Publication: arXiv 2024
  - Highlights: World models increase autonomy in RL.
  - Paper Link: [arXiv](https://arxiv.org/abs/2408.09807) | [Website](https://sites.google.com/view/morefree)

- **Grounded Answers for Multi-agent Decision-making Problem through Generative World Model**
  - Publication: arXiv 2024
  - Highlights: Grounds LLMs in embodied environments with imperfect world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.02664)

- **Energy-based Transition Models: Offline Transition Modeling via Contrastive Energy Learning**
  - Highlights: Offline transition modeling via contrastive energy learning.
  - [OpenReview](https://openreview.net/forum?id=dqpg8jdA2w) | [Code](https://github.com/Ruifeng-Chen/Energy-Transition-Models)

- **PCM: Policy-conditioned Environment Models are More Generalizable**
  - Highlights: Policy-conditioned environment models are more generalizable.
  - [OpenReview](https://openreview.net/forum?id=g9mYBdooPA) | [Website](https://policy-conditioned-model.github.io/) | [Code](https://github.com/xionghuichen/policy-conditioned-model)

- **JOWA: Scaling Offline Model-Based RL via Jointly-Optimized World-Action Model Pretraining**
  - Highlights: Scales offline MBRL via jointly-optimized world-action model pretraining.
  - [OpenReview](https://openreview.net/forum?id=T1OvCSFaum) | [Code](https://github.com/CJReinforce/JOWA)

- **LS-Imagine: Open-World RL over Long Short-Term Imagination**
  - Highlights: Open-world RL over long short-term imagination.
  - [OpenReview](https://openreview.net/forum?id=vzItLaEoDa)

- **TWISTER: Learning Transformer-based World Models with Contrastive Predictive Coding**
  - Highlights: Learns transformer-based world models with contrastive predictive coding.
  - [OpenReview](https://openreview.net/forum?id=YK9G4Htdew) | [Website](https://github.com/burchim/TWISTER)

- **WAKER: Reward-Free Curricula for Training Robust World Models**
  - Highlights: Reward-free curricula for training robust world models.
  - [OpenReview](https://openreview.net/forum?id=eCGpNGDeNu)

- **THICK: Learning Hierarchical World Models with Adaptive Temporal Abstractions**
  - Highlights: Learns hierarchical world models with adaptive temporal abstractions.
  - [OpenReview](https://openreview.net/forum?id=TjCDNssXKU) | [Code](https://github.com/CognitiveModeling/THICK)

---

## 🎯 Application Domains

### 8.1 Robotics & Embodied AI

#### 8.1.1 Foundation Embodied World Models



- **Xiaomi-Robotics-U0: Unified Embodied Synthesis with World Foundation Model**
  - Publication: arXiv 2026
  - Highlights: Xiaomi's unified embodied synthesis with a world foundation model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.11643) | [Website](https://robotics.xiaomi.com/xiaomi-robotics-u0.html) | [Code](https://github.com/XiaomiRobotics/Xiaomi-Robotics-U0)

- **ABot-3DWorld 0: A Universal World Model to Explore Any 3D Space** *(Moved from 4.3)*
  - Publication: arXiv 2026
  - Highlights: A universal world model for exploring any 3D space.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.11673) | [Website](https://abot-world.amap.com/plaza)

- **WoW: Towards a World omniscient World model Through Embodied Interaction**
  - Publication: arXiv 2025
  - Highlights: Towards a world-omniscient world model through embodied interaction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.22642) | [Website](https://wow-world-model.github.io) | [Code](https://github.com/wow-world-model/wow-world-model)

- **Genie Envisioner: A Unified World Foundation Platform for Robotic Manipulation**
  - Publication: arXiv 2025
  - Highlights: Unified world foundation platform for robotic manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.05635) | [Website](https://genie-envisioner.github.io/) | [Code](https://github.com/AgibotTech/Genie-Envisioner)

- **iVideoGPT: Interactive VideoGPTs are Scalable World Models**
  - Publication: arXiv 2024
  - Highlights: Interactive VideoGPTs are scalable world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2405.15223) | [Website](https://thuml.github.io/iVideoGPT/) | [Code](https://github.com/thuml/iVideoGPT)

- **ViPRA: Video Prediction for Robot Actions**
  - Publication: arXiv 2025
  - Highlights: Video prediction for robot actions.
  - Paper Link: [arXiv](https://arxiv.org/abs/2511.07732) | [Website](https://vipra-project.github.io) | [Code](https://github.com/sroutray/vipra)


#### 8.1.2 Manipulation



- **DriftWorld: Fast World Modeling through Drifting**
  - Publication: arXiv 2026
  - Highlights: Fast world modeling through a drifting generative model, generating future frames at 30+ fps in a single forward pass, 17x faster than diffusion baselines.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.15065) | [Website](https://susie-lu.github.io/driftworld/)

- **RynnWorld-4D: 4D Embodied World Models for Robotic Manipulation**
  - Publication: arXiv 2026
  - Highlights: 4D embodied world models for robotic manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.06559) | [Website](https://alibaba-damo-academy.github.io/RynnWorld-4D.github.io/) | [Code](https://github.com/alibaba-damo-academy/RynnWorld-4D)

- **RynnWorld-Teleop: An Action-Conditioned World Model for Digital Teleoperation**
  - Publication: arXiv 2026
  - Highlights: Action-conditioned world model for digital teleoperation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.06558) | [Website](https://alibaba-damo-academy.github.io/RynnWorld-Teleop.github.io) | [Code](https://github.com/alibaba-damo-academy/RynnWorld-Teleop)

- **PhysisForcing: Physics Reinforced World Simulator for Robotic Manipulation**
  - Publication: arXiv 2026
  - Highlights: Physics-reinforced world simulator for robotic manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.28128) | [Website](https://dagroup-pku.github.io/PhysisForcing.github.io/) | [Code](https://github.com/dagroup-pku/PhysisForcing)

- **Hierarchical World Model: H-WM – Robotic Task and Motion Planning Guided by Hierarchical World Model**
  - Publication: arXiv 2026
  - Highlights: Robotic task and motion planning guided by a hierarchical world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.11291)

- **Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning**
  - Publication: arXiv 2026
  - Highlights: Fine-tunes video models for visuomotor control and planning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.16163) | [Website](https://research.nvidia.com/labs/dir/cosmos-policy/)

- **DiT4DiT: Jointly Modeling Video Dynamics and Actions for Generalizable Robot Control**
  - Publication: arXiv 2026
  - Highlights: Jointly models video dynamics and actions for generalizable robot control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.10448) | [Website](https://dit4dit.github.io/)

- **PointWorld**
  - Publication: arXiv 2026
  - Highlights: NVIDIA's large-scale pre-trained 3D world model unifying state and action as 3D point flows.
  - Paper Link: [arXiv](https://www.arxiv.org/abs/2601.03782) | [Website](https://point-world.github.io)

- **GEM-4D: Geometry-Enhanced Video World Models for Robot Manipulation**
  - Publication: arXiv 2025
  - Highlights: Geometry-enhanced video world models for robot manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.22882) | [Website](https://anonymous-submission-20.github.io/gem.github.io/)

- **GaussianDream: A Feed-Forward 3D Gaussian World Model for Robotic Manipulation**
  - Publication: arXiv 2025
  - Highlights: Feed-forward 3D Gaussian world model for robotic manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.20752)

- **Demo-JEPA: Joint-Embedding Predictive Architecture for One-shot Cross-Embodiment Imitation**
  - Publication: arXiv 2025
  - Highlights: Joint-embedding predictive architecture for one-shot cross-embodiment imitation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.20811)

- **Action-State Consistency: Is the Future Compatible? Diagnosing Dynamic Consistency in World Action Models**
  - Publication: arXiv 2025
  - Highlights: Diagnoses dynamic consistency in world action models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.07514)

- **Dex-WM**
  - Publication: arXiv 2025
  - Highlights: Dexterous world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2512.13644) | [Website](https://raktimgg.github.io/dexwm/)

- **FLARE: Robot Learning with Implicit World Modeling**
  - Publication: arXiv 2025
  - Highlights: Robot learning with implicit world modeling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.15659) | [Website](https://research.nvidia.com/labs/gear/flare/)

- **EnerVerse: Envisioning Embodied Future Space for Robotics Manipulation**
  - Publication: arXiv 2025
  - Highlights: Envisions embodied future space for robotics manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.01895) | [Website](https://sites.google.com/view/enerverse)

- **AgiBot-World Colosseo: A Large-scale Manipulation Platform for Scalable and Intelligent Embodied Systems**
  - Publication: arXiv 2025
  - Highlights: Large-scale manipulation platform for scalable and intelligent embodied systems.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.06669) | [Website](https://agibot-world.com/) | [Code](https://github.com/OpenDriveLab/AgiBot-World)

- **DyWA: Dynamics-adaptive World Action Model for Generalizable Non-prehensile Manipulation**
  - Publication: arXiv 2025
  - Highlights: Dynamics-adaptive world action model for generalizable non-prehensile manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.16806) | [Website](https://pku-epic.github.io/DyWA/) | [Code](https://github.com/jiangranlv/DyWA)

- **TesserAct: Learning 4D Embodied World Models**
  - Publication: arXiv 2025
  - Highlights: Learns 4D embodied world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.20995) | [Website](https://tesseractworld.github.io/) | [Code](https://github.com/UMass-Embodied-AGI/TesserAct)

- **DreamGen: Unlocking Generalization in Robot Learning through Video World Models**
  - Publication: arXiv 2025
  - Highlights: Unlocks generalization in robot learning through video world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.12705) | [Website](https://research.nvidia.com/labs/gear/dreamgen/) | [Code](https://github.com/nvidia/GR00T-dreams)

- **HiP: Compositional Foundation Models for Hierarchical Planning**
  - Publication: arXiv 2023
  - Highlights: Compositional foundation models for hierarchical planning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2309.08587) | [Website](https://hierarchical-planning-foundation-model.github.io/) | [Code](https://github.com/anuragajay/hip/tree/main)

- **PAR: Physical Autoregressive Model for Robotic Manipulation without Action Pretraining**
  - Publication: arXiv 2025
  - Highlights: Physical autoregressive model for robotic manipulation without action pretraining.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.09822) | [Website](https://hcplab-sysu.github.io/PhysicalAutoregressiveModel/) | [Code](https://github.com/HCPLab-SYSU/PhysicalAutoregressiveModel)

- **WristWorld: Generating Wrist-Views via 4D World Models for Robotic Manipulation**
  - Publication: arXiv 2025
  - Highlights: Generates wrist-views via 4D world models for robotic manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.07313) | [Website](https://wrist-world.github.io) | [Code](https://github.com/XuWuLingYu/WristWorld)

- **EMMA: Generalizing Real-World Robot Manipulation via Generative Visual Transfer**
  - Publication: arXiv 2025
  - Highlights: Generalizes real-world robot manipulation via generative visual transfer.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.22407) | [Website](https://emma-gigaai.github.io)

- **PhysTwin: Physics-Informed Reconstruction and Simulation of Deformable Objects from Videos**
  - Publication: arXiv 2025
  - Highlights: Physics-informed reconstruction and simulation of deformable objects from videos.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.17973) | [Website](https://jianghanxiao.github.io/phystwin-web/) | [Code](https://github.com/Jianghanxiao/PhysTwin)

- **KeyWorld: Key Frame Reasoning Enables Effective and Efficient World Models**
  - Publication: arXiv 2025
  - Highlights: Key frame reasoning enables effective and efficient world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.21027)

- **World4RL: Diffusion World Models for Policy Refinement with RL for Robotic Manipulation**
  - Publication: arXiv 2025
  - Highlights: Diffusion world models for policy refinement with RL.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.19080) | [Website](https://world4rl.github.io)

- **SAMPO: Scale-wise Autoregression with Motion PrOmpt for generative world models**
  - Publication: arXiv 2025
  - Highlights: Scale-wise autoregression with motion prompt for generative world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.15536)

- **PhysicalAgent: Towards General Cognitive Robotics with Foundation World Models**
  - Publication: arXiv 2025
  - Highlights: Towards general cognitive robotics with foundation world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.13903)

- **Learning Primitive Embodied World Models: Towards Scalable Robotic Learning**
  - Publication: arXiv 2025
  - Highlights: Towards scalable robotic learning with primitive embodied world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.20840) | [Website](https://qiaosun22.github.io/PrimitiveWorld/)

- **GWM: Towards Scalable Gaussian World Models for Robotic Manipulation**
  - Publication: arXiv 2025
  - Highlights: Towards scalable Gaussian world models for robotic manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.17600) | [Website](https://gaussian-world-model.github.io/) | [Code](https://github.com/Gaussian-World-Model/gaussianwm)

- **Flow-as-Action: Latent Policy Steering with Embodiment-Agnostic Pretrained World Models**
  - Publication: arXiv 2025
  - Highlights: Latent policy steering with embodiment-agnostic pretrained world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.13340)

- **EmbodieDreamer: Advancing Real2Sim2Real Transfer for Policy Training via Embodied World Modeling**
  - Publication: arXiv 2025
  - Highlights: Advancing real2sim2real transfer via embodied world modeling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.05198) | [Website](https://embodiedreamer.github.io/) | [Code](https://github.com/GigaAI-research/EmbodieDreamer)

- **RoboScape: Physics-informed Embodied World Model**
  - Publication: arXiv 2025
  - Highlights: Physics-informed embodied world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.23135) | [Code](https://github.com/tsinghua-fib-lab/RoboScape)

- **FWM: Factored World Models for Zero-Shot Generalization in Robotic Manipulation**
  - Publication: arXiv 2022
  - Highlights: Factored world models for zero-shot generalization.
  - Paper Link: [arXiv](https://arxiv.org/abs/2202.05333)

- **ParticleFormer: A 3D Point Cloud World Model for Multi-Object, Multi-Material Robotic Manipulation**
  - Publication: arXiv 2025
  - Highlights: 3D point cloud world model for multi-object, multi-material robotic manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.23126) | [Website](https://suninghuang19.github.io/particleformer_page/)

- **ManiGaussian++: General Robotic Bimanual Manipulation with Hierarchical Gaussian World Model**
  - Publication: arXiv 2025
  - Highlights: General robotic bimanual manipulation with hierarchical Gaussian world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.19842) | [Code](https://github.com/April-Yz/ManiGaussian_Bimanual)

- **ReOI: Reimagination with Test-time Observation Interventions for Distractor-Robust World Model Predictions**
  - Publication: arXiv 2025
  - Highlights: Reimagination with test-time observation interventions for distractor-robust world model predictions.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.16565)

- **GAF: Gaussian Action Field as a Dynamic World Model for Robotic Manipulation**
  - Publication: arXiv 2025
  - Highlights: Gaussian action field as a dynamic world model for robotic manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.14135) | [Website](http://chaiying1.github.io/GAF.github.io/project_page/)

- **Prompting with the Future: Open-World MPC with Interactive Digital Twins**
  - Publication: arXiv 2025
  - Highlights: Open-world MPC with interactive digital twins.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.13761) | [Website](https://prompting-with-the-future.github.io/) | [Code](https://github.com/TritiumR/Prompting-with-the-Future)

- **Time-Aware World Model for Adaptive Prediction and Control**
  - Publication: arXiv 2025
  - Highlights: Time-aware world model for adaptive prediction and control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.08441) | [Website](https://anh-nn01.github.io/time-aware-world-models/) | [Code](https://github.com/anh-nn01/Time-Aware-World-Model/tree/main?tab=readme-ov-file)

- **3DFlowAction: Learning Cross-Embodiment Manipulation from 3D Flow World Model**
  - Publication: arXiv 2025
  - Highlights: Learns cross-embodiment manipulation from 3D flow world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.06199) | [Code](https://github.com/Hoyyyaard/3DFlowAction/)

- **ORV: 4D Occupancy-centric Robot Video Generation**
  - Publication: arXiv 2025
  - Highlights: 4D occupancy-centric robot video generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.03079) | [Code](https://github.com/OrangeSodahub/ORV) | [Website](https://orangesodahub.github.io/ORV/)

- **WoMAP: World Models For Embodied Open-Vocabulary Object Localization**
  - Publication: arXiv 2025
  - Highlights: World models for embodied open-vocabulary object localization.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.01600) | [Website](https://robot-womap.github.io)

- **OSVI-WM: One-Shot Visual Imitation for Unseen Tasks using World-Model-Guided Trajectory Generation**
  - Publication: arXiv 2025
  - Highlights: One-shot visual imitation for unseen tasks using world-model-guided trajectory generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.20425)

- **LaDi-WM: A Latent Diffusion-based World Model for Predictive Manipulation**
  - Publication: arXiv 2025
  - Highlights: Latent diffusion-based world model for predictive manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.11528) | [Website](https://guhuangai.github.io/LaDiWM.github.io/) | [Code](https://github.com/GuHuangAI/LaDiWM)

- **FlowDreamer: A RGB-D World Model with Flow-based Motion Representations for Robot Manipulation**
  - Publication: arXiv 2025
  - Highlights: RGB-D world model with flow-based motion representations for robot manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.10075) | [Website](https://sharinka0715.github.io/FlowDreamer/) | [Code](https://github.com/sharinka0715/FlowDreamer/)

- **PIN-WM: Learning Physics-INformed World Models for Non-Prehensile Manipulation**
  - Publication: arXiv 2025
  - Highlights: Learning physics-informed world models for non-prehensile manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.16693) | [Website](https://pinwm.github.io) | [Code](https://github.com/XuAdventurer/PIN-WM)

- **RoboMaster: Learning Video Generation for Robotic Manipulation with Collaborative Trajectory Control**
  - Publication: arXiv 2025
  - Highlights: Learning video generation for robotic manipulation with collaborative trajectory control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.01943) | [Website](https://fuxiao0719.github.io/projects/robomaster/) | [Code](https://github.com/KwaiVGI/RoboMaster)

- **ManipDreamer: Boosting Robotic Manipulation World Model with Action Tree and Visual Guidance**
  - Publication: arXiv 2025
  - Highlights: Boosts robotic manipulation world models with action tree and visual guidance.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.16464) | [Website](https://myendless1.github.io/ManipDreamer/)

- **AdaWorld: Learning Adaptable World Models with Latent Actions**
  - Publication: arXiv 2025
  - Highlights: Learns adaptable world models with latent actions.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.18938) | [Website](https://adaptable-world-model.github.io/) | [Code](https://github.com/Little-Podi/AdaWorld)

- **Towards Suturing World Models: Learning Predictive Models for Robotic Surgical Tasks**
  - Publication: arXiv 2025
  - Highlights: Learning predictive models for robotic surgical tasks.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.12531) | [Website](https://mkturkcan.github.io/suturingmodels/)

- **EVA: An Embodied World Model for Future Video Anticipation**
  - Publication: arXiv 2024
  - Highlights: Embodied world model for future video anticipation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.15461) | [Website](https://sites.google.com/view/eva-publi) | [Code](https://github.com/litwellchi/EmbodiedVideoAnticipator?tab=readme-ov-file)

- **DexSim2Real$^2$: Building Explicit World Model for Precise Articulated Object Dexterous Manipulation**
  - Publication: arXiv 2024
  - Highlights: Builds explicit world models for precise articulated object dexterous manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2409.08750) | [Code](https://github.com/jiangtaoran/DexSim2Real2?tab=readme-ov-file)

- **Physically Embodied Gaussian Splatting: A Realtime Correctable World Model for Robotics**
  - Publication: arXiv 2024
  - Highlights: Realtime correctable world model for robotics.
  - Paper Link: [arXiv](https://arxiv.org/abs/2406.10788) | [Website](https://embodied-gaussians.github.io/) | [Code](https://github.com/bdaiinstitute/embodied_gaussians)

- **LUMOS: Language-Conditioned Imitation Learning with World Models**
  - Publication: arXiv 2025
  - Highlights: Language-conditioned imitation learning with world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.10370) | [Website](http://lumos.cs.uni-freiburg.de/) | [Code](https://github.com/nematoli/lumos)

- **Object-Centric World Model for Language-Guided Manipulation**
  - Publication: arXiv 2025
  - Highlights: Object-centric world model for language-guided manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.06170)

- **DEMO^3: Multi-Stage Manipulation with Demonstration-Augmented Reward, Policy, and World Model Learning**
  - Publication: arXiv 2025
  - Highlights: Multi-stage manipulation with demonstration-augmented reward, policy, and world model learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.01837) | [Website](https://adrialopezescoriza.github.io/demo3/) | [Code](https://github.com/adrialopezescoriza/demo3)

- **Strengthening Generative Robot Policies through Predictive World Modeling**
  - Publication: arXiv 2025
  - Highlights: Strengthens generative robot policies through predictive world modeling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.00622) | [Website](https://computationalrobotics.seas.harvard.edu/GPC)

- **RoboHorizon: An LLM-Assisted Multi-View World Model for Long-Horizon Robotic Manipulation**
  - Publication: arXiv 2025
  - Highlights: LLM-assisted multi-view world model for long-horizon robotic manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.06605)

- **Dream to Manipulate: Compositional World Models Empowering Robot Imitation Learning with Imagination**
  - Publication: arXiv 2024
  - Highlights: Compositional world models empowering robot imitation learning with imagination.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.14957) | [Website](https://leobarcellona.github.io/DreamToManipulate/)

- **RoboDreamer: Learning Compositional World Models for Robot Imagination**
  - Publication: arXiv 2024
  - Highlights: Learns compositional world models for robot imagination.
  - Paper Link: [arXiv](https://arxiv.org/abs/2404.12377) | [Code](https://github.com/rainbow979/robodreamer) | [Website](https://robovideo.github.io)

- **Vidar: Embodied Video Diffusion Model for Generalist Manipulation**
  - Publication: arXiv 2025
  - Highlights: Embodied video diffusion model for generalist manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.12898)

- **ManiGaussian: Dynamic Gaussian Splatting for Multi-task Robotic Manipulation**
  - Publication: arXiv 2024
  - Highlights: Dynamic Gaussian splatting for multi-task robotic manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2403.08321) | [Code](https://github.com/GuanxingLu/ManiGaussian) | [Website](https://guanxinglu.github.io/ManiGaussian/)

- **WHALE: Towards Generalizable and Scalable World Models for Embodied Decision-making**
  - Publication: arXiv 2024
  - Highlights: Towards generalizable and scalable world models for embodied decision-making.
  - Paper Link: [arXiv](https://arxiv.org/abs/2411.05619)

- **VisualPredicator: Learning Abstract World Models with Neuro-Symbolic Predicates for Robot Planning**
  - Publication: arXiv 2024
  - Highlights: Learns abstract world models with neuro-symbolic predicates for robot planning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.23156)

- **Multi-Task Interactive Robot Fleet Learning with Visual World Models**
  - Publication: arXiv 2024
  - Highlights: Multi-task interactive robot fleet learning with visual world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.22689) | [Code](https://github.com/UT-Austin-RPL/sirius-fleet/) | [Website](https://ut-austin-rpl.github.io/sirius-fleet/)

- **PIVOT-R: Primitive-Driven Waypoint-Aware World Model for Robotic Manipulation**
  - Publication: arXiv 2024
  - Highlights: Primitive-driven waypoint-aware world model for robotic manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.10394) | [Website](https://abliao.github.io/PIVOT-R/) | [Code](https://github.com/abliao/PIVOT-R)

- **Video2Action: Grounding Video Models to Actions through Goal Conditioned Exploration**
  - Publication: arXiv 2024
  - Highlights: Grounds video models to actions through goal-conditioned exploration.
  - Paper Link: [arXiv](https://arxiv.org/abs/2411.07223) | [Website](https://video-to-action.github.io/) | [Code](https://github.com/video-to-action/video-to-action-release)

- **FRAPPE: Infusing World Modeling into Generalist Policies via Multiple Future Representation Alignment**
  - Publication: arXiv 2026
  - Highlights: Infuses world modeling into generalist policies via multiple future representation alignment.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.17259)

- **PhysMani: Physics-principled 3D World Model for Dynamic Object Manipulation**
  - Publication: arXiv 2026 (ECCV 2026)
  - Highlights: Couples a physics-principled 3D Gaussian world model with a future-aware action policy model; proposes PhysMani-Bench with 16 tasks.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.01938)

#### 8.1.3 Navigation



- **EfficientNWM: An Efficient and Multi-Modal Navigation System with One-Step World Model**
  - Publication: arXiv 2026
  - Highlights: Efficient and multi-modal navigation system with a one-step world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.12277) | [Website](https://robotnav-bot.github.io/nav-onestepwm/) | [Code](https://github.com/robotnav-bot/NOW)

- **NavMorph: A Self-Evolving World Model for Vision-and-Language Navigation in Continuous Environments**
  - Publication: arXiv 2025
  - Highlights: Self-evolving world model for vision-and-language navigation in continuous environments.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.23468) | [Code](https://github.com/Feliciaxyao/NavMorph)

- **MindJourney: Test-Time Scaling with World Models for Spatial Reasoning**
  - Publication: arXiv 2025
  - Highlights: Test-time scaling with world models for spatial reasoning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.12508) | [Website](https://umass-embodied-agi.github.io/MindJourney)

- **Unified World Models: Memory-Augmented Planning and Foresight for Visual Navigation**
  - Publication: arXiv 2025
  - Highlights: Memory-augmented planning and foresight for visual navigation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.08713) | [Code](https://github.com/F1y1113/UniWM)

- **NaVi-WM: Deductive Chain-of-Thought Augmented Socially-aware Robot Navigation World Model**
  - Publication: arXiv 2025
  - Highlights: Deductive chain-of-thought augmented socially-aware robot navigation world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.23509) | [Website](https://sites.google.com/view/NaviWM)

- **AIF: Deep Active Inference with Diffusion Policy and Multiple Timescale World Model for Real-World Exploration and Navigation**
  - Publication: arXiv 2025
  - Highlights: Deep active inference with diffusion policy and multiple timescale world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.23258)

- **Kinodynamic Motion Planning for Mobile Robot Navigation across Inconsistent World Models**
  - Publication: arXiv 2025
  - Highlights: Kinodynamic motion planning across inconsistent world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.26339)

- **World Model Implanting for Test-time Adaptation of Embodied Agents**
  - Publication: arXiv 2025
  - Highlights: World model implanting for test-time adaptation of embodied agents.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.03956)

- **Imaginative World Modeling with Scene Graphs for Embodied Agent Navigation**
  - Publication: arXiv 2025
  - Highlights: Imaginative world modeling with scene graphs for embodied agent navigation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.06990)

- **Persistent Embodied World Models: Learning 3D Persistent Embodied World Models**
  - Publication: arXiv 2025
  - Highlights: Learning 3D persistent embodied world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.05495)

- **Perspective-Shifted Neuro-Symbolic World Models: A Framework for Socially-Aware Robot Navigation**
  - Publication: arXiv 2025
  - Highlights: Neuro-symbolic world models for socially-aware robot navigation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.20425)

- **WMNav: Integrating Vision-Language Models into World Models for Object Goal Navigation**
  - Publication: arXiv 2025
  - Highlights: Integrates VLMs into world models for object goal navigation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.02247) | [Website](https://b0b8k1ng.github.io/WMNav/)

- **NWM: Navigation World Models**
  - Publication: arXiv 2024
  - Highlights: Navigation world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.03572) | [Website](https://www.amirbar.net/nwm/)

- **X-MOBILITY: End-To-End Generalizable Navigation via World Modeling**
  - Publication: arXiv 2024
  - Highlights: End-to-end generalizable navigation via world modeling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.17491)

- **MWM: Masked World Models for Visual Control**
  - Publication: arXiv 2022
  - Highlights: Masked world models for visual control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2206.14244) | [Website](https://sites.google.com/view/mwm-rl) | [Code](https://github.com/younggyoseo/MWM)

#### 8.1.4 Locomotion & Loco-Manipulation



- **Ego-VCP: Ego-Vision World Model for Humanoid Contact Planning**
  - Publication: arXiv 2025
  - Highlights: Ego-vision world model for humanoid contact planning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.11682) | [Website](https://ego-vcp.github.io/) | [Code](https://github.com/HybridRobotics/Ego-VCP)

- **ProTerrain: Probabilistic Physics-Informed Rough Terrain World Modeling**
  - Publication: arXiv 2025
  - Highlights: Probabilistic physics-informed rough terrain world modeling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.19364)

- **RWM-O: Offline Robotic World Model – Learning Robotic Policies without a Physics Simulator**
  - Publication: arXiv 2025
  - Highlights: Learning robotic policies without a physics simulator.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.16680)

- **Humanoid World Models: Open World Foundation Models for Humanoid Robotics**
  - Publication: arXiv 2025
  - Highlights: Open world foundation models for humanoid robotics.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.01182)

- **DWL: Advancing Humanoid Locomotion: Mastering Challenging Terrains with Denoising World Model Learning**
  - Publication: arXiv 2024
  - Highlights: Mastering challenging terrains with denoising world model learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2408.14472)

- **HRSSM: Learning Latent Dynamic Robust Representations for World Models**
  - Publication: arXiv 2024
  - Highlights: Learning latent dynamic robust representations for world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2405.06263) | [Code](https://github.com/bit1029public/HRSSM)

- **WMP: World Model-based Perception for Visual Legged Locomotion**
  - Publication: arXiv 2024
  - Highlights: World model-based perception for visual legged locomotion.
  - Paper Link: [arXiv](https://arxiv.org/abs/2409.16784) | [Website](https://wmp-loco.github.io/)

- **TrajWorld: Trajectory World Models for Heterogeneous Environments**
  - Publication: arXiv 2025
  - Highlights: Trajectory world models for heterogeneous environments.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.01366) | [Code](https://github.com/thuml/TrajWorld)

- **Puppeteer: Hierarchical World Models as Visual Whole-Body Humanoid Controllers**
  - Publication: arXiv 2024
  - Highlights: Hierarchical world models as visual whole-body humanoid controllers.
  - Paper Link: [arXiv](https://arxiv.org/abs/2405.18418) | [Code](https://nicklashansen.com/rlpuppeteer)

- **Occupancy World Model for Robots**
  - Publication: arXiv 2025
  - Highlights: Occupancy world model for robots.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.05512)

- **Accelerating Model-Based RL with State-Space World Models**
  - Publication: arXiv 2025
  - Highlights: Accelerating MBRL with state-space world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.20168)

- **Learning Humanoid Locomotion with World Model Reconstruction**
  - Publication: arXiv 2025
  - Highlights: Learning humanoid locomotion with world model reconstruction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.16230)

- **Robotic World Model: A Neural Network Simulator for Robust Policy Optimization in Robotics**
  - Publication: arXiv 2025
  - Highlights: Neural network simulator for robust policy optimization in robotics.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.10100)

- **D^2PO: World Modeling Makes a Better Planner – Dual Preference Optimization for Embodied Task Planning**
  - Publication: arXiv 2025
  - Highlights: Dual preference optimization for embodied task planning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.10480)

- **COMBO: Compositional World Models for Embodied Multi-Agent Cooperation**
  - Publication: arXiv 2024
  - Highlights: Compositional world models for embodied multi-agent cooperation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2404.10775) | [Website](https://vis-www.cs.umass.edu/combo/) | [Code](https://github.com/UMass-Foundation-Model/COMBO)


#### 8.1.5 World Models x Policy Learning

*This section focuses on using world models for policy search, optimization, and policy representation learning (without joint VLA architectures).*

- **LingBot-VA: Causal video-action world model for generalist robot control**
  - Publication: arXiv 2026
  - Highlights: Causal video-action world model for generalist robot control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.21998) | [Website](https://technology.robbyant.com/lingbot-va) | [Code](https://github.com/Robbyant/lingbot-va)

- **Native Video-Action Pretraining for Generalizable Robot Control (LingBot-VA 2.0)**
  - Publication: arXiv 2026
  - Highlights: Video-action foundation model with semantic visual-action tokenizer, causal pretraining, sparse MoE.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.08639) | WeChat: [link](https://mp.weixin.qq.com/s/YI7j20M11WanZSlartWPwA)

- **UWM: Unified World Models – Coupling Video and Action Diffusion for Pretraining on Large Robotic Datasets**
  - Publication: arXiv 2025
  - Highlights: Couples video and action diffusion for pretraining on large robotic datasets.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.02792) | [Website](https://weirdlabuw.github.io/uwm/)

- **UVA: Unified Video Action Model**
  - Publication: arXiv 2025
  - Highlights: Unified video action model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.00200) | [Website](https://unified-video-action-model.github.io/) | [Code](https://github.com/ShuangLI59/unified_video_action)

- **DiWA: Diffusion Policy Adaptation with World Models**
  - Publication: arXiv 2025
  - Highlights: Diffusion policy adaptation with world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.03645) | [Code](https://diwa.cs.uni-freiburg.de)

- **DreamerV4: Training Agents Inside of Scalable World Models**
  - Publication: arXiv 2025
  - Highlights: Trains agents inside of scalable world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.24527) | [Website](https://danijar.com/project/dreamer4/)

- **LVP: Large Video Planner Enables Generalizable Robot Control**
  - Publication: arXiv 2025
  - Highlights: Large video planner enables generalizable robot control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2512.15840) | [Website](https://www.boyuan.space/large-video-planner/)

- **LDA-1B: Scaling Latent Dynamics Action Model via Universal Embodied Data Ingestion**
  - Publication: arXiv 2026
  - Highlights: Scales latent dynamics action model via universal embodied data ingestion.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.12215) | [Website](https://pku-epic.github.io/LDA/) | [Code](https://github.com/jiangranlv/latent-dynamics-action)

- **ABot-M0.5: Unified Mobility-and-Manipulation World Action Model**
  - Publication: arXiv 2026
  - Highlights: Unified mobility-and-manipulation WAM aligning time granularity, action space, and train-test consistency.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.00678) | [Code](https://github.com/amap-cvlab/ABot-Manipulation)

- **EgoWAM: World Action Models Beyond Pixels with In-the-Wild Egocentric Human Data**
  - Publication: arXiv 2026
  - Highlights: World action models beyond pixels using in-the-wild egocentric human data.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.08436) | [Website](https://gatech-rl2.github.io/egowam.github.io/)

- **WAM-TTT: Steering World-Action Models by Watching Human Play at Test Time**
  - Publication: arXiv 2026
  - Highlights: Steers world-action models by watching human play at test time.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.06988)

- **FlowWAM: Optical Flow as a Unified Action Representation for World Action Models**
  - Publication: arXiv 2026
  - Highlights: Optical flow as a unified action representation for WAMs.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.13017) | [Website](https://flow-wam.github.io/) | [Code](https://github.com/YixiangChen515/FlowWAM)

- **GigaWorld-Policy-0.5: A Faster and Stronger WAM Empowered by AutoResearch**
  - Publication: arXiv 2026
  - Highlights: Faster and stronger WAM with a mixture-of-experts transformer architecture, achieving 85ms inference latency on RTX 4090.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.13960) | [Website](https://open-gigaai.github.io/giga-world-policy/) | [Code](https://github.com/open-gigaai/giga-world-policy)

- **Robotic World Model: A Neural Network Simulator for Robust Policy Optimization in Robotics**
  - Publication: arXiv 2025
  - Highlights: Neural network simulator for robust policy optimization in robotics.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.10100)


#### 8.1.6 Policy Evaluation with World Models

*This section focuses on using world models as evaluators/simulators to test policy robustness and performance.*



- **SC3-Eval: Evaluating Robot Foundation Models via Self-Consistent Video Generation**
  - Publication: arXiv 2026
  - Highlights: Evaluates robot foundation models via self-consistent video generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.18610) | [Website](https://weichengtseng.github.io/sc3-eval/)

- **GigaWorld-1: A Roadmap to Build World Models for Robot Policy Evaluation**
  - Publication: arXiv 2026
  - Highlights: A roadmap to build world models for robot policy evaluation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.02642) | [Website](https://open-gigaai.github.io/giga-world-1/)

- **StressDream: Steering Video World Models for Robust Policy Evaluation and Improvement**
  - Publication: arXiv 2026
  - Highlights: Steers video world models for robust policy evaluation and improvement.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.00267) | [Website](https://junwon.me/StressDream/) | [Code](https://github.com/CMU-IntentLab/StressDream)

- **WorldGym: Evaluating Robot Policies in a World Model**
  - Publication: arXiv 2025
  - Highlights: Evaluates robot policies in a world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.00613) | [Website](https://world-model-eval.github.io)

- **WorldEval: World Model as Real-World Robot Policies Evaluator**
  - Publication: arXiv 2025
  - Highlights: World model as real-world robot policy evaluator.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.19017) | [Website](https://worldeval.github.io)

- **WoW!: World Models in a Closed-Loop World**
  - Highlights: World models in a closed-loop world.
  - [OpenReview](https://openreview.net/abs/e6aed49462d9e080633e727436cc95a0a8d61c57.pdf) | [Website](https://wow202509.github.io/WOW_project_page/)

- **Cosmos-Surg-dVRK: World Foundation Model-based Automated Online Evaluation of Surgical Robot Policy Learning**
  - Publication: arXiv 2025
  - Highlights: World foundation model-based automated online evaluation of surgical robot policy learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.16240)

---

### 8.2 Autonomous Driving

- **DriveVA: Video Action Models are Zero-Shot Drivers**
  - Publication: ECCV 2026
  - Highlights: Jointly predicts future video latents and driving actions, with zero-shot transfer to nuScenes and Bench2Drive.
  - Paper Link: [Paper](https://link.springer.com/chapter/10.1007/978-3-032-37718-0_19) | [Code](https://github.com/xiaomi-mlab/DriveVA)



- **M⁴World: A Multi-view Multimodal Driving World Model for Interactive Object Manipulation and Minute-long Streaming**
  - Publication: arXiv 2026
  - Highlights: Multi-view multimodal generative driving world model synthesizing surround-view video and LiDAR scans.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.14005)

- **Xiaomi Auto World Model: A Joint World Model Integrating Reconstruction and Generation**
  - Publication: arXiv 2026
  - Highlights: Xiaomi's joint world model integrating reconstruction and generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.12701)

- **ResWorld: Temporal Residual World Model for End-to-End Autonomous Driving**
  - Publication: arXiv 2026
  - Highlights: Temporal residual world model for end-to-end autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.08261)

- **CausalDrive: Real-time Causal World Models for Autonomous Driving**
  - Publication: arXiv 2026
  - Highlights: Real-time causal world models for autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.15341)

- **LWDrive: Layer-Wise World-Model-Guided Vision-Language Model Planning for Autonomous Driving**
  - Publication: arXiv 2026
  - Highlights: Layer-wise world-model-guided VLM planning, achieving 92.0 on the NAVSIM benchmark.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.29879)

- **Toward Physically Consistent Driving Video World Models under Challenging Trajectories (PhyGenesis)**
  - Publication: arXiv 2026
  - Highlights: Physically consistent driving video world models under challenging trajectories.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.24506)

- **AutoWorld: Scaling Multi-Agent Traffic Simulation with Self-Supervised World Models**
  - Publication: arXiv 2026
  - Highlights: Scales multi-agent traffic simulation with self-supervised world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.28963)

- **Reason--Imagine--Act: Closed-Loop LLM Decision Making with World Models for Autonomous Driving**
  - Publication: arXiv 2026
  - Highlights: Closed-loop LLM decision making with world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.14723)

- **OmniDreams: NVIDIA OmniDreams – Real-Time Generative World Model for Closed-Loop AV Simulation**
  - Publication: arXiv 2026
  - Highlights: NVIDIA's real-time generative world model for closed-loop AV simulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.03159) | [Website](https://research.nvidia.com/labs/sil/projects/omnidreams-blog/) | [Code](https://github.com/nv-tlabs/omni-dreams)

- **Cosmos-Drive-Dreams: Scalable Synthetic Driving Data Generation with World Foundation Models**
  - Publication: arXiv 2025
  - Highlights: Scalable synthetic driving data generation with world foundation models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.09042) | [Website](https://research.nvidia.com/labs/toronto-ai/cosmos_drive_dreams)

- **GAIA-2: A Controllable Multi-View Generative World Model for Autonomous Driving**
  - Publication: arXiv 2025
  - Highlights: Controllable multi-view generative world model for autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.20523) | [Website](https://wayve.ai/thinking/gaia-2)

- **GAIA-1: A Cutting-Edge Generative AI Model for Autonomy**
  - Publication: arXiv 2023
  - Highlights: Cutting-edge generative AI model for autonomy.
  - Paper Link: [arXiv](https://arxiv.org/abs/2309.17080) | [Blog](https://wayve.ai/thinking/introducing-gaia1/)

- **WorldLens: Full-Spectrum Evaluations of Driving World Models in Real World**
  - Publication: arXiv 2025
  - Highlights: Full-spectrum evaluations of driving world models in the real world.
  - Paper Link: [arXiv](https://arxiv.org/abs/2512.10958) | [Website](https://worldbench.github.io/worldlens)

- **Copilot4D: Learning Unsupervised World Models for Autonomous Driving via Discrete Diffusion**
  - Publication: arXiv 2023
  - Highlights: Learns unsupervised world models for autonomous driving via discrete diffusion.
  - Paper Link: [arXiv](https://arxiv.org/abs/2311.01017)

- **OmniNWM: Omniscient Driving Navigation World Models**
  - Publication: arXiv 2025
  - Highlights: Omniscient driving navigation world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.18313) | [Website](https://arlo0o.github.io/OmniNWM/)

- **PWM: From Forecasting to Planning – Policy World Model for Collaborative State-Action Prediction**
  - Publication: arXiv 2025
  - Highlights: Policy world model for collaborative state-action prediction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.19654) | [Code](https://github.com/6550Zhao/Policy-World-Model)

- **Dream4Drive: Rethinking Driving World Model as Synthetic Data Generator for Perception Tasks**
  - Publication: arXiv 2025
  - Highlights: Rethinking driving world models as synthetic data generators.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.19195) | [Website](https://wm-research.github.io/Dream4Drive/)

- **SparseWorld: A Flexible, Adaptive, and Efficient 4D Occupancy World Model**
  - Publication: arXiv 2025
  - Highlights: Flexible, adaptive, and efficient 4D occupancy world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.17482) | [Code](https://github.com/MSunDYY/SparseWorld)

- **DriveVLA-W0: World Models Amplify Data Scaling Law in Autonomous Driving**
  - Publication: arXiv 2025
  - Highlights: World models amplify data scaling laws in autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.12796) | [Code](https://github.com/BraveGroup/DriveVLA-W0)

- **IRL-VLA: Training an Vision-Language-Action Policy via Reward World Model**
  - Publication: arXiv 2025
  - Highlights: Training a VLA policy via reward world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.06571) | [Website](https://lidarcrafter.github.io) | [Code](https://github.com/lidarcrafter/toolkit)

- **LiDARCrafter: Dynamic 4D World Modeling from LiDAR Sequences**
  - Publication: arXiv 2025
  - Highlights: Dynamic 4D world modeling from LiDAR sequences.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.03692) | [Website](https://lidarcrafter.github.io) | [Code](https://github.com/lidarcrafter/toolkit)

- **FASTopoWM: Fast-Slow Lane Segment Topology Reasoning with Latent World Models**
  - Publication: arXiv 2025
  - Highlights: Fast-slow lane segment topology reasoning with latent world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.23325) | [Code](https://github.com/YimingYang23/FASTopoWM)

- **Orbis: Overcoming Challenges of Long-Horizon Prediction in Driving World Models**
  - Publication: arXiv 2025
  - Highlights: Overcomes challenges of long-horizon prediction in driving world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.13162) | [Code](https://lmb-freiburg.github.io/orbis.github.io/)

- **World Model-Based End-to-End Scene Generation for Accident Anticipation**
  - Publication: arXiv 2025
  - Highlights: End-to-end scene generation for accident anticipation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.12762)

- **NRSeg: Noise-Resilient Learning for BEV Semantic Segmentation via Driving World Models**
  - Publication: arXiv 2025
  - Highlights: Noise-resilient learning for BEV semantic segmentation via driving world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.04002) | [Code](https://github.com/lynn-yu/NRSeg)

- **World4Drive: End-to-End Autonomous Driving via Intention-aware Physical Latent World Model**
  - Publication: arXiv 2025
  - Highlights: End-to-end autonomous driving via intention-aware physical latent world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.00603) | [Code](https://github.com/ucaszyp/World4Drive)

- **Epona: Autoregressive Diffusion World Model for Autonomous Driving**
  - Publication: arXiv 2025
  - Highlights: Autoregressive diffusion world model for autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.24113) | [Code](https://kevin-thu.github.io/Epona/)

- **SceneDiffuser++: City-Scale Traffic Simulation via a Generative World Model**
  - Publication: arXiv 2025
  - Highlights: City-scale traffic simulation via a generative world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.21976)

- **COME: Adding Scene-Centric Forecasting Control to Occupancy World Model**
  - Publication: arXiv 2025
  - Highlights: Adds scene-centric forecasting control to occupancy world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.13260) | [Code](https://github.com/synsin0/COME)

- **STAGE: A Stream-Centric Generative World Model for Long-Horizon Driving-Scene Simulation**
  - Publication: arXiv 2025
  - Highlights: Stream-centric generative world model for long-horizon driving-scene simulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.13138)

- **ReSim: Reliable World Simulation for Autonomous Driving**
  - Publication: arXiv 2025
  - Highlights: Reliable world simulation for autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.09981) | [Code](https://github.com/OpenDriveLab/ReSim) | [Website](https://opendrivelab.com/ReSim)

- **V2XCrafter: Learning to Generate Driving Scene Across Agents**
  - Publication: arXiv 2025
  - Highlights: Learns to generate driving scenes across agents.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.29471)

- **Dreamland: Controllable World Creation with Simulator and Generative Models**
  - Publication: arXiv 2025
  - Highlights: Controllable world creation with simulator and generative models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.08006) | [Website](https://metadriverse.github.io/dreamland/)

- **LongDWM: Cross-Granularity Distillation for Building a Long-Term Driving World Model**
  - Publication: arXiv 2025
  - Highlights: Cross-granularity distillation for building long-term driving world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.01546) | [Website](https://wang-xiaodong1899.github.io/longdwm/)

- **GeoDrive: 3D Geometry-Informed Driving World Model with Precise Action Control**
  - Publication: arXiv 2025
  - Highlights: 3D geometry-informed driving world model with precise action control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.22421) | [Code](https://github.com/antonioo-c/GeoDrive)

- **FutureSightDrive: Thinking Visually with Spatio-Temporal CoT for Autonomous Driving**
  - Publication: arXiv 2025
  - Highlights: Thinking visually with spatio-temporal CoT for autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.17685) | [Code](https://github.com/MIV-XJTU/FSDrive)

- **Raw2Drive: RL with Aligned World Models for End-to-End Autonomous Driving (in CARLA v2)**
  - Publication: arXiv 2025
  - Highlights: RL with aligned world models for end-to-end autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.16394)

- **VL-SAFE: Vision-Language Guided Safety-Aware RL with World Models for Autonomous Driving**
  - Publication: arXiv 2025
  - Highlights: Vision-language guided safety-aware RL with world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.16377) | [Website](https://ys-qu.github.io/vlsafe-website/)

- **PosePilot: Steering Camera Pose for Generative World Models with Self-supervised Depth**
  - Publication: arXiv 2025
  - Highlights: Steering camera pose for generative world models with self-supervised depth.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.01729)

- **Learning to Drive from a World Model**
  - Publication: arXiv 2025
  - Highlights: Learning to drive from a world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.19077)

- **DriVerse: Navigation World Model for Driving Simulation via Multimodal Trajectory Prompting**
  - Publication: arXiv 2025
  - Highlights: Navigation world model for driving simulation via multimodal trajectory prompting.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.18576)

- **End-to-End Driving with Online Trajectory Evaluation via BEV World Model**
  - Publication: arXiv 2025
  - Highlights: End-to-end driving with online trajectory evaluation via BEV world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.01941) | [Code](https://github.com/liyingyanUCAS/WoTE)

- **Knowledge Graphs as World Models for Semantic Material-Aware Obstacle Handling in AVs**
  - Publication: arXiv 2025
  - Highlights: Knowledge graphs as world models for semantic material-aware obstacle handling.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.21232)

- **MiLA: Multi-view Intensive-fidelity Long-term Video Generation World Model for Autonomous Driving**
  - Publication: arXiv 2025
  - Highlights: Multi-view intensive-fidelity long-term video generation world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.15875) | [Website](https://github.com/xiaomi-mlab/mila.github.io)

- **UniFuture: A Unified Driving World Model for Future Generation and Perception**
  - Publication: arXiv 2025
  - Highlights: Unified driving world model for future generation and perception.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.13587) | [Website](https://github.com/dk-liang/UniFuture)

- **EOT-WM: Other Vehicle Trajectories Are Also Needed – Unifies Ego-Other trajectories in Latent Space**
  - Publication: arXiv 2025
  - Highlights: Unifies ego-other trajectories in latent space.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.09215)

- **Temporal Triplane Transformers as Occupancy World Models**
  - Publication: arXiv 2025
  - Highlights: Temporal triplane transformers as occupancy world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.07338)

- **InDRiVE: Intrinsic Disagreement based RL for Vehicle Exploration through Curiosity Driven Generalized World Model**
  - Publication: arXiv 2025
  - Highlights: Intrinsic disagreement-based RL for vehicle exploration via curiosity-driven generalized world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.05573)

- **MaskGWM: A Generalizable Driving World Model with Video Mask Reconstruction**
  - Publication: arXiv 2025
  - Highlights: Generalizable driving world model with video mask reconstruction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.11663)

- **Dream to Drive: Model-Based Vehicle Control Using Analytic World Models**
  - Publication: arXiv 2025
  - Highlights: Model-based vehicle control using analytic world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.10012)

- **Semi-Supervised Vision-Centric 3D Occupancy World Model for Autonomous Driving**
  - Publication: arXiv 2025
  - Highlights: Semi-supervised vision-centric 3D occupancy world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.07309)

- **Dream to Drive with Predictive Individual World Model**
  - Publication: arXiv 2025
  - Highlights: Predictive individual world model for driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.16733) | [Code](https://github.com/gaoyinfeng/PIWM)

- **HERMES: A Unified Self-Driving World Model for Simultaneous 3D Scene Understanding and Generation**
  - Publication: arXiv 2025
  - Highlights: Unified self-driving world model for simultaneous 3D scene understanding and generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.14729)

- **AdaWM: Adaptive World Model based Planning for Autonomous Driving**
  - Publication: arXiv 2025
  - Highlights: Adaptive world model-based planning for autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.13072)

- **AD-L-JEPA: Self-Supervised Spatial World Models with JEPA for Autonomous Driving with LiDAR**
  - Publication: arXiv 2025
  - Highlights: Self-supervised spatial world models with JEPA for LiDAR-based autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.04969)

- **DrivingWorld: Constructing World Model for Autonomous Driving via Video GPT**
  - Publication: arXiv 2024
  - Highlights: Constructs world models for autonomous driving via Video GPT.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.19505) | [Code](https://github.com/YvanYin/DrivingWorld) | [Website](https://huxiaotaostasy.github.io/DrivingWorld/index.html)

- **DrivingGPT: Unifying Driving World Modeling and Planning with Multi-modal Autoregressive Transformers**
  - Publication: arXiv 2024
  - Highlights: Unifies driving world modeling and planning with multi-modal autoregressive transformers.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.18607) | [Website](https://rogerchern.github.io/DrivingGPT/)

- **An Efficient Occupancy World Model via Decoupled Dynamic Flow and Image-assisted Training**
  - Publication: arXiv 2024
  - Highlights: Efficient occupancy world model via decoupled dynamic flow and image-assisted training.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.13772)

- **GEM: A Generalizable Ego-Vision Multimodal World Model for Fine-Grained Control**
  - Publication: arXiv 2024
  - Highlights: Generalizable ego-vision multimodal world model for fine-grained control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.11198) | [Website](https://vita-epfl.github.io/GEM.github.io/)

- **GaussianWorld: Gaussian World Model for Streaming 3D Occupancy Prediction**
  - Publication: arXiv 2024
  - Highlights: Gaussian world model for streaming 3D occupancy prediction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.04380) | [Code](https://github.com/zuosc19/GaussianWorld)

- **Doe-1: Closed-Loop Autonomous Driving with Large World Model**
  - Publication: arXiv 2024
  - Highlights: Closed-loop autonomous driving with large world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.09627) | [Website](https://wzzheng.net/Doe/) | [Code](https://github.com/wzzheng/Doe)

- **Physical Informed Driving World Model**
  - Publication: arXiv 2024
  - Highlights: Physical informed driving world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.08410) | [Website](https://metadrivescape.github.io/papers_project/DrivePhysica/page.html)

- **InfiniCube: Unbounded and Controllable Dynamic 3D Driving Scene Generation with World-Guided Video Models**
  - Publication: arXiv 2024
  - Highlights: Unbounded and controllable dynamic 3D driving scene generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.03934) | [Website](https://research.nvidia.com/labs/toronto-ai/infinicube/)

- **InfinityDrive: Breaking Time Limits in Driving World Models**
  - Publication: arXiv 2024
  - Highlights: Breaks time limits in driving world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.01522) | [Website](https://metadrivescape.github.io/papers_project/InfinityDrive/page.html)

- **ReconDreamer: Crafting World Models for Driving Scene Reconstruction via Online Restoration**
  - Publication: arXiv 2024
  - Highlights: Crafts world models for driving scene reconstruction via online restoration.
  - Paper Link: [arXiv](https://arxiv.org/abs/2411.19548) | [Website](https://recondreamer.github.io/)

- **Imagine-2-Drive: High-Fidelity World Modeling in CARLA for Autonomous Vehicles**
  - Publication: arXiv 2024
  - Highlights: High-fidelity world modeling in CARLA for autonomous vehicles.
  - Paper Link: [arXiv](https://arxiv.org/abs/2411.10171) | [Website](https://anantagrg.github.io/Imagine-2-Drive.github.io/)

- **DynamicCity: Large-Scale 4D Occupancy Generation from Dynamic Scenes**
  - Publication: arXiv 2024
  - Highlights: Large-scale 4D occupancy generation from dynamic scenes.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.18084) | [Website](https://dynamic-city.github.io) | [Code](https://github.com/3DTopia/DynamicCity)

- **DriveDreamer4D: World Models Are Effective Data Machines for 4D Driving Scene Representation**
  - Publication: arXiv 2024
  - Highlights: World models as effective data machines for 4D driving scene representation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.13571) | [Website](https://drivedreamer4d.github.io/)

- **DOME: Taming Diffusion Model into High-Fidelity Controllable Occupancy World Model**
  - Publication: arXiv 2024
  - Highlights: Tames diffusion models into high-fidelity controllable occupancy world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.10429) | [Website](https://gusongen.github.io/DOME)


- **Mitigating Covariate Shift in Imitation Learning for AVs Using Latent Space Generative World Models**
  - Publication: arXiv 2024
  - Highlights: Mitigates covariate shift in imitation learning for AVs using latent space generative world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2409.16663)

- **LatentDriver: Learning Multiple Probabilistic Decisions from Latent World Model in Autonomous Driving**
  - Publication: arXiv 2024
  - Highlights: Learns multiple probabilistic decisions from latent world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2409.15730) | [Code](https://github.com/Sephirex-X/LatentDriver)

- **RenderWorld: World Model with Self-Supervised 3D Label**
  - Publication: arXiv 2024
  - Highlights: World model with self-supervised 3D labels.
  - Paper Link: [arXiv](https://arxiv.org/abs/2409.11356)

- **OccLLaMA: An Occupancy-Language-Action Generative World Model for Autonomous Driving**
  - Publication: arXiv 2024
  - Highlights: Occupancy-language-action generative world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2409.03272)

- **DriveGenVLM: Real-world Video Generation for VLM based Autonomous Driving**
  - Publication: arXiv 2024
  - Highlights: Real-world video generation for VLM-based autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2408.16647)

- **Drive-OccWorld: Driving in the Occupancy World – Vision-Centric 4D Occupancy Forecasting and Planning**
  - Publication: arXiv 2024
  - Highlights: Vision-centric 4D occupancy forecasting and planning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2408.14197)

- **BEVWorld: A Multimodal World Model for Autonomous Driving via Unified BEV Latent Space**
  - Publication: arXiv 2024
  - Highlights: Multimodal world model via unified BEV latent space.
  - Paper Link: [arXiv](https://arxiv.org/abs/2407.05679) | [Code](https://github.com/zympsyche/BevWorld)

- **AdaptiveDriver: Planning with Adaptive World Models for Autonomous Driving**
  - Publication: arXiv 2024
  - Highlights: Planning with adaptive world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2406.10714) | [Code](https://arunbalajeev.github.io/world_models_planning/world_model_paper.html)

- **UnO: Unsupervised Occupancy Fields for Perception and Forecasting**
  - Publication: arXiv 2024
  - Highlights: Unsupervised occupancy fields for perception and forecasting.
  - Paper Link: [arXiv](https://arxiv.org/abs/2406.08691) | [Code](https://waabi.ai/research/uno)

- **LAW: Enhancing End-to-End Autonomous Driving with Latent World Model**
  - Publication: arXiv 2024
  - Highlights: Enhances end-to-end autonomous driving with latent world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2406.08481) | [Code](https://github.com/BraveGroup/LAW)

- **Delphi: Unleashing Generalization of End-to-End Autonomous Driving with Controllable Long Video Generation**
  - Publication: arXiv 2024
  - Highlights: Unleashes generalization of end-to-end autonomous driving with controllable long video generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2406.01349) | [Code](https://github.com/westlake-autolab/Delphi)

- **OccSora: 4D Occupancy Generation Models as World Simulators for Autonomous Driving**
  - Publication: arXiv 2024
  - Highlights: 4D occupancy generation models as world simulators.
  - Paper Link: [arXiv](https://arxiv.org/abs/2405.20337) | [Code](https://github.com/wzzheng/OccSora)

- **Vista: A Generalizable Driving World Model with High Fidelity and Versatile Controllability**
  - Publication: arXiv 2024
  - Highlights: Generalizable driving world model with high fidelity and versatile controllability.
  - Paper Link: [arXiv](https://arxiv.org/abs/2405.17398) | [Code](https://github.com/OpenDriveLab/Vista)

- **CarDreamer: Open-Source Learning Platform for World Model based Autonomous Driving**
  - Publication: arXiv 2024
  - Highlights: Open-source learning platform for world model-based autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2405.09111) | [Code](https://github.com/ucd-dare/CarDreamer)

- **DriveSim: Probing Multimodal LLMs as World Models for Driving**
  - Publication: arXiv 2024
  - Highlights: Probes multimodal LLMs as world models for driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2405.05956) | [Code](https://github.com/sreeramsa/DriveSim)

- **DriveWorld: 4D Pre-trained Scene Understanding via World Models for Autonomous Driving**
  - Publication: arXiv 2024
  - Highlights: 4D pre-trained scene understanding via world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2405.04390)

- **DriveDreamer-2: LLM-Enhanced World Models for Diverse Driving Video Generation**
  - Publication: arXiv 2024
  - Highlights: LLM-enhanced world models for diverse driving video generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2403.06845) | [Code](https://drivedreamer2.github.io/)

- **Think2Drive: Efficient RL by Thinking in Latent World Model for Quasi-Realistic Autonomous Driving**
  - Publication: arXiv 2024
  - Highlights: Efficient RL by thinking in latent world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2402.16720)

- **MARL-CCE: Modelling Competitive Behaviors in Autonomous Driving Under Generative World Model**
  - Publication: ECCV 2024
  - Highlights: Models competitive behaviors under generative world models.
  - Paper Link: [Paper](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/05085.pdf) | [Code](https://github.com/qiaoguanren/MARL-CCE)

- **GenAD: Generalized Predictive Model for Autonomous Driving**
  - Publication: arXiv 2024
  - Highlights: Generalized predictive model for autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2403.09630) | [Website](https://github.com/OpenDriveLab/DriveAGI?tab=readme-ov-file#genad-dataset-opendv-youtube)

- **GenAD: Generative End-to-End Autonomous Driving**
  - Publication: arXiv 2024
  - Highlights: Generative end-to-end autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2402.11502) | [Code](https://github.com/wzzheng/GenAD)

- **NeMo: Neural Volumetric World Models for Autonomous Driving**
  - Publication: ECCV 2024
  - Highlights: Neural volumetric world models.
  - Paper Link: [Paper](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/02571.pdf)

- **ViDAR: Visual Point Cloud Forecasting enables Scalable Autonomous Driving**
  - Publication: arXiv 2023
  - Highlights: Visual point cloud forecasting enables scalable autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2312.17655) | [Code](https://github.com/OpenDriveLab/ViDAR)

- **Drive-WM: Driving into the Future – Multiview Visual Forecasting and Planning with World Model**
  - Publication: arXiv 2023
  - Highlights: Multiview visual forecasting and planning with world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2311.17918) | [Code](https://github.com/BraveGroup/Drive-WM)

- **Cam4DOCC: Benchmark for Camera-Only 4D Occupancy Forecasting in Autonomous Driving**
  - Publication: arXiv 2023
  - Highlights: Benchmark for camera-only 4D occupancy forecasting.
  - Paper Link: [arXiv](https://arxiv.org/abs/2311.17663) | [Code](https://github.com/haomo-ai/Cam4DOcc)

- **OccWorld: Learning a 3D Occupancy World Model for Autonomous Driving**
  - Publication: arXiv 2023
  - Highlights: Learns a 3D occupancy world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2311.16038) | [Code](https://github.com/wzzheng/OccWorld)

- **SafeDreamer: Safe Reinforcement Learning with World Models**
  - Publication: ICLR 2024
  - Highlights: Safe RL with world models.
  - Paper Link: [OpenReview](https://openreview.net/forum?id=tsE5HLYtYg) | [Code](https://github.com/PKU-Alignment/SafeDreamer)

- **DriveDreamer: Towards Real-world-driven World Models for Autonomous Driving**
  - Publication: arXiv 2023
  - Highlights: Towards real-world-driven world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2309.09777) | [Code](https://github.com/JeffWang987/DriveDreamer)

- **SEM2: Enhance Sample Efficiency and Robustness of End-to-End Urban Autonomous Driving via Semantic Masked World Model**
  - Publication: IEEE Trans. 2024
  - Highlights: Enhances sample efficiency and robustness via semantic masked world models.
  - Paper Link: [IEEE](https://ieeexplore.ieee.org/abstract/document/10538211/)

- **Latent-WAM: Latent World Action Modeling for End-to-End Autonomous Driving**
  - Publication: arXiv 2026
  - Highlights: Latent world action modeling for trajectory planning via spatial-aware and dynamic-aware latent representations.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.24581)

- **Geographic Diversity Beats Data Volume for Cross-Domain Generalization in Zero-Label JEPA Driving World Models**
  - Publication: arXiv 2026
  - Highlights: Geographic diversity outperforms data volume for cross-domain generalization; 63K geographically diverse scenes outperform 200K single-geography scenes.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.04500)

- **GeoWorldAD: Geometry World Action Model for Autonomous Driving**
  - Publication: arXiv 2026
  - Highlights: Geometry world action model for autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.17521)

- **GraphWorld: Long-Horizon Planning with World Models for End-to-End Autonomous Driving**
  - Publication: arXiv 2026
  - Highlights: Long-horizon planning with graph world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.16274)

- **Orbis 2: A Hierarchical World Model for Driving**
  - Publication: arXiv 2026
  - Highlights: Hierarchical world model for driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.15898)

- **EponaV2: Driving World Model with Comprehensive Future Reasoning**
  - Publication: arXiv 2026
  - Highlights: Driving world model with comprehensive future reasoning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.14696)

---

### 8.3 GUI / Computer-Use Agents



- **WebWorld: A Large-Scale World Model for Web Agent Training**
  - Publication: arXiv 2026
  - Highlights: Built from over one million real web interactions; outperforms GPT-5 as a world model for inference-time search.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.14721)

- **Qwen-AgentWorld: Language World Models for General Agents**
  - Publication: arXiv 2026
  - Highlights: First native language world models (35B-A3B and 397B-A17B) simulating agentic environments across 7 domains via long CoT reasoning, trained on >10M interaction trajectories.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.24597)

- **From Tokens to States: LLMs as a Special Case of World Models and the Continuous Path Beyond**
  - Publication: arXiv 2026
  - Highlights: Formalizes LLMs as a special case of world models and proposes a continuous path beyond.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.28127)

- **Computer-Using World Model (CUWM)**
  - Publication: arXiv 2026
  - Highlights: Predicts next UI state given current state and candidate actions.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.15003)

- **Code2World: A GUI World Model via Renderable Code Generation**
  - Publication: arXiv 2026
  - Highlights: Models GUI dynamics by generating renderable code rather than pixels.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.07131)

- **MobileDreamer: Generative Sketch World Model for GUI Agent**
  - Publication: arXiv 2026
  - Highlights: Lightweight world model predicting task-relevant text sketches rather than full screenshots.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.04035)

- **ViMo: A Generative Visual GUI World Model for App Agent**
  - Publication: arXiv 2025
  - Highlights: Generative visual GUI world model for app agents.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.13936)

- **How Mobile World Model Guides GUI Agents?**
  - Publication: arXiv 2026
  - Highlights: Investigates how mobile world models guide GUI agents.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.10347)

- **Neural-OS: Towards Simulating Operating Systems via Neural Generative Models**
  - Publication: arXiv 2025
  - Highlights: Towards simulating operating systems via neural generative models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.08800) | [Website](https://neural-os.com/) | [Code](https://github.com/yuntian-group/neural-os)

- **R-WoM: Retrieval-augmented World Model For Computer-use Agents**
  - Publication: arXiv 2025
  - Highlights: Retrieval-augmented world model for computer-use agents.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.11892)

- **SimuRA: Towards General Goal-Oriented Agent via Simulative Reasoning Architecture with LLM-Based World Model**
  - Publication: arXiv 2025
  - Highlights: Simulative reasoning architecture with LLM-based world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.23773)

- **WebSynthesis: World-Model-Guided MCTS for Efficient WebUI-Trajectory Synthesis**
  - Publication: arXiv 2025
  - Highlights: World-model-guided MCTS for efficient WebUI trajectory synthesis.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.04370)

- **WKM: Agent Planning with World Knowledge Model**
  - Publication: arXiv 2024
  - Highlights: Agent planning with world knowledge models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2405.14205) | [Code](https://github.com/zjunlp/WKM)

- **WebDreamer: Is Your LLM Secretly a World Model of the Internet? Model-Based Planning for Web Agents**
  - Publication: arXiv 2024
  - Highlights: Model-based planning for web agents.
  - Paper Link: [arXiv](https://arxiv.org/abs/2411.06559) | [Code](https://github.com/OSU-NLP-Group/WebDreamer)

- **Web Agents with World Models: Learning and Leveraging Environment Dynamics in Web Navigation**
  - Publication: arXiv 2024
  - Highlights: Learning and leveraging environment dynamics in web navigation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.13232)

- **WebEvolver: Enhancing Web Agent Self-Improvement with Coevolving World Model**
  - Publication: arXiv 2025
  - Highlights: Enhancing web agent self-improvement with coevolving world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.21024)

- **WALL-E 2.0: World Alignment by NeuroSymbolic Learning improves World Model-based LLM Agents**
  - Publication: arXiv 2025
  - Highlights: World alignment by neuro-symbolic learning improves world model-based LLM agents.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.15785) | [Code](https://github.com/elated-sawyer/WALL-E)

- **Dyna-Think: Synergizing Reasoning, Acting, and World Model Simulation in AI Agents**
  - Publication: arXiv 2025
  - Highlights: Synergizes reasoning, acting, and world model simulation in AI agents.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.00320)

- **FPWC: Unlocking Smarter Device Control – Foresighted Planning with a World Model-Driven Code Execution Approach**
  - Publication: arXiv 2025
  - Highlights: Foresighted planning with a world model-driven code execution approach.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.16422)

---

### 8.4 Scientific Discovery



- **MicroVerse: A Preliminary Exploration Toward a Micro-World Simulation**
  - Publication: arXiv 2026
  - Highlights: Preliminary exploration of micro-world simulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.00585) | [Code](https://github.com/FreedomIntelligence/MicroVerse)

- **Earth-o1: A Grid-free Observation-native Atmospheric World Model**
  - Publication: arXiv 2026
  - Highlights: Grid-free, observation-native atmospheric world model matching the fidelity of established physical frameworks.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.06337)

- **CheXWorld: Exploring Image World Modeling for Radiograph Representation Learning**
  - Publication: arXiv 2025
  - Highlights: Explores image world modeling for radiograph representation learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.13820) | [Code](https://github.com/LeapLabTHU/CheXWorld)

- **EchoWorld: Learning Motion-Aware World Models for Echocardiography Probe Guidance**
  - Publication: arXiv 2025
  - Highlights: Learning motion-aware world models for echocardiography probe guidance.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.13065) | [Code](https://github.com/LeapLabTHU/EchoWorld)

- **ODesign: A World Model for Biomolecular Interaction Design**
  - Publication: arXiv 2025
  - Highlights: World model for biomolecular interaction design.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.22304) | [Website](https://odesign.lglab.ac.cn)

- **SFP: Spatiotemporal Forecasting as Planning – A Model-Based RL Approach with Generative World Models**
  - Publication: arXiv 2025
  - Highlights: Spatiotemporal forecasting as planning with generative world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.04020)

- **Xray2Xray: World Model from Chest X-rays with Volumetric Context**
  - Publication: arXiv 2025
  - Highlights: World model from chest X-rays with volumetric context.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.19055)

- **Medical World Model: Generative Simulation of Tumor Evolution for Treatment Planning**
  - Publication: arXiv 2025
  - Highlights: Generative simulation of tumor evolution for treatment planning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.02327)

- **Surgical Vision World Model**
  - Publication: arXiv 2025
  - Highlights: Surgical vision world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.02904)


---

### 8.5 Social & Economic Simulation



- **Social World Models**
  - Publication: arXiv 2025
  - Highlights: Social world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.00559)

- **Social World Model-Augmented Mechanism Design Policy Learning**
  - Publication: arXiv 2025
  - Highlights: Social world model-augmented mechanism design policy learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.19270)

- **SocioVerse: A World Model for Social Simulation Powered by LLM Agents and A Pool of 10 Million Real-World Users**
  - Publication: arXiv 2025
  - Highlights: World model for social simulation powered by LLM agents and 10 million real-world users.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.10157) | [Code](https://github.com/FudanDISC/SocioVerse)


---

## 📊 Datasets & Benchmarks

### 9.1 General World Modeling



| Dataset/Benchmark Name | Year | Scale | Core Tasks | Link |
|---|---|---|---|---|
| **Omni-WorldBench** | 2026 | 18 representative world models | Comprehensive interaction-centric evaluation for 4D world models | [arXiv](https://arxiv.org/abs/2603.22212) |
| **AgentWorldBench** | 2026 | 5 frontier models, 9 benchmarks | Comprehensive benchmark for language world models | [arXiv](https://arxiv.org/abs/2606.24597) |
| **iWorld-Bench** | 2026 | 330k video clips, 4.9k test samples | Interactive world model evaluation | [arXiv](https://arxiv.org/abs/2605.03941) |
| **MemoBench** | 2026 | 360 ground-truth videos | "Disappear-reappear" world modeling evaluation | [arXiv](https://arxiv.org/abs/2606.27537) |
| **Chess-World-Model** | 2026 | 10.1 million chess games | Precise state tracking benchmark | [arXiv](https://arxiv.org/abs/2605.30100) |
| **WorldModelBench** | 2025 | Video generation models | World model evaluation | [arXiv](https://arxiv.org/abs/2502.20694) |
| **WorldArena** | 2025 | Embodied world models | Perception & functional utility | [arXiv](https://arxiv.org/pdf/2602.08971) |
| **WorldArena 2.0** | 2026 | Embodied world models | Extended benchmarking on modality, functionality, and platform | [arXiv](https://arxiv.org/abs/2605.17912) |
| **WorldScore** | 2025 | — | Unified evaluation benchmark for world generation | [arXiv](https://arxiv.org/abs/2504.00983) |
| **CRONOS** | 2025 | — | Counterfactual physical consistency in video models | [arXiv](https://arxiv.org/abs/2605.23699) |
| **WBench** | 2025 | — | Multi-turn interactive video world model evaluation | [arXiv](https://arxiv.org/abs/2605.25874) |
| **OmniWorld** | 2025 | — | Multi-domain multi-modal dataset for 4D world modeling | [arXiv](https://arxiv.org/abs/2509.12201) |
| **World-in-World** | 2025 | — | Closed-loop world model evaluation | [arXiv](https://arxiv.org/abs/2510.18135) |
| **EWMBench** | 2025 | — | Embodied world model quality evaluation | [arXiv](https://arxiv.org/abs/2505.09694) |
| **WorldSimBench** | 2024 | — | Video generation models as world simulators | [arXiv](https://arxiv.org/abs/2410.18072) |
| **World Reasoning Arena (WR-Arena)** | 2026 | — | Comprehensive benchmark evaluating world models along three fundamental dimensions | [arXiv](https://arxiv.org/abs/2603.25887) |
| **MBench** | 2026 | — | Comprehensive benchmark on memory capability for video world models | [arXiv](https://arxiv.org/abs/2606.00793) |

### 9.2 Physics & Causality



| Dataset/Benchmark Name | Year | Scale | Core Tasks | Link |
|---|---|---|---|---|
| **A Physics-Grounded Benchmark for Multi-Agent Dynamics in World Models** | 2026 | Multi-agent dynamics | Physics-grounded multi-agent dynamics benchmark | [arXiv](https://arxiv.org/abs/2606.28757) |
| **CausalARC** | 2026 | Causal reasoning tasks | Abstract reasoning with causal world models | [arXiv](https://arxiv.org/pdf/2509.03636) |


### 9.3 Domain-Specific Benchmarks



#### Robotics

| Dataset/Benchmark Name | Year | Scale | Core Tasks | Link |
|---|---|---|---|---|
| **ContactWorld** | 2026 | 12 contact-rich tasks | Vision-tactile world models for contact-rich manipulation | [arXiv](https://arxiv.org/abs/2606.13877) |
| **RoboWM-Bench** | 2026 | Robotic manipulation | Embodied evaluation for video world models | [Semantic Scholar](https://www.semanticscholar.org) |
| **AgiBot-World** | 2025 | Large-scale manipulation | Manipulation benchmark | [Website](https://agibot-world.com/) |
| **PhysMani-Bench** | 2026 | 16 tasks | Physics-principled dynamic object manipulation | [arXiv](https://arxiv.org/abs/2607.01938) |

#### Autonomous Driving

| Dataset/Benchmark Name | Year | Scale | Core Tasks | Link |
|---|---|---|---|---|
| **ReactSim-Bench** | 2026 | 2,636 test scenarios | Reactive behavior world model simulation in autonomous driving | [arXiv](https://arxiv.org/abs/2606.14058) |
| **SimWorld** | 2025 | — | Simulator-conditioned scene generation | [arXiv](https://arxiv.org/abs/2503.13952) |
| **ACT-Bench** | 2024 | — | Action controllable world models for autonomous driving | [arXiv](https://arxiv.org/abs/2412.05337) |
| **DrivingWorld** | 2024 | 40+ sec video | Autonomous driving world model | [arXiv](https://arxiv.org/abs/2412.19505) |
| **InfinityDrive** | 2024 | Minute-scale | Driving world model | [arXiv](https://arxiv.org/abs/2412.01234) |
| **DisCoBench** | 2026 | — | Comprehensive benchmark for discrete camera motion control in world models | [arXiv](https://arxiv.org/abs/2606.07967) |

#### Web/GUI Agents

| Dataset/Benchmark Name | Year | Scale | Core Tasks | Link |
|---|---|---|---|---|
| **WebWorld** | 2026 | 1M+ web interactions | Large-scale world model for web agent training | [arXiv](https://arxiv.org/abs/2602.14721) |

---

## ⚙️ Training & Inference Techniques

### 10.1 Memory Mechanisms



- **DiM-WAM: Diverse Historical Event Memory** (see WAM section)
- **Current World Models Lack a Persistent State Core**
  - Publication: arXiv 2026
  - Highlights: Argues that generators must maintain a continuously evolving world state rather than rendering plausible frames only at observation time.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.20545)

- **Latent Spatial Memory for Video World Models (Mirage)**
  - Publication: arXiv 2026
  - Highlights: Stores persistent 3D scene content directly as latent tokens, avoiding repeated RGB rendering, and updates caches during generation.
  - Paper Link: [GitHub](https://github.com/microsoft/LatentSpatialMemory)

- **MemLearner: Learning to Query Context Memory for Video World Models**
  - Publication: arXiv 2026
  - Highlights: Learns to query context memory for video world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.31734) | [Website](https://yujiwen.github.io/memlearner/)

- **Context as Memory: Scene-Consistent Interactive Long Video Generation with Memory Retrieval**
  - Publication: arXiv 2025
  - Highlights: Scene-consistent interactive long video generation with memory retrieval.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.03141) | [Website](https://context-as-memory.github.io/)

- **VMem: Consistent Interactive Video Scene Generation with Surfel-Indexed View Memory**
  - Publication: arXiv 2025
  - Highlights: Consistent interactive video scene generation with surfel-indexed view memory.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.18903) | [Website](https://v-mem.github.io/) | [Code](https://github.com/runjiali-rl/vmem)

- **WonderWorld: Interactive 3D Scene Generation from a Single Image**
  - Publication: arXiv 2024
  - Highlights: Interactive 3D scene generation from a single image.
  - Paper Link: [arXiv](https://arxiv.org/abs/2406.09394) | [Website](https://kovenyu.com/wonderworld/)

- **Spatial Memory: Video World Models with Long-term Spatial Memory**
  - Publication: arXiv 2025
  - Highlights: Video world models with long-term spatial memory.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.05284) | [Website](https://spmem.github.io)

- **Mem-World: Memory-Augmented Action-Conditioned World Models for Persistent Robot Manipulation**
  - Publication: arXiv 2026
  - Highlights: Memory-augmented multi-view action-conditioned world models; proposes W-VMem, a 4D wrist-centric surfel-indexed memory.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.18960)

- **Echo-Memory: A Controlled Study of Memory in Action World Models**
  - Publication: arXiv 2026
  - Highlights: Controlled study of memory mechanisms in action-conditioned world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.09803)

### 10.2 Post-Training & Test-Time Scaling



- **RLVR-World: Training World Models with Reinforcement Learning**
  - Publication: arXiv 2025
  - Highlights: Trains world models with reinforcement learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2505.13934) | [Website](https://thuml.github.io/RLVR-World/) | [Code](https://github.com/thuml/RLVR-World)

- **RLIR: Reinforcement Learning with Inverse Rewards for World Model Post-training**
  - Publication: arXiv 2025
  - Highlights: Uses inverse rewards for world model post-training.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.23958)

- **ChronoEdit: Towards Temporal Reasoning for Image Editing and World Simulation**
  - Publication: arXiv 2025
  - Highlights: Temporal reasoning for image editing and world simulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.04290) | [Website](https://research.nvidia.com/labs/toronto-ai/chronoedit/) | [Code](https://github.com/nv-tlabs/ChronoEdit)

- **SWIFT: Can Test-Time Scaling Improve World Foundation Model?**
  - Publication: arXiv 2025
  - Highlights: Investigates whether test-time scaling improves world foundation models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.24320) | [Code](https://github.com/Mia-Cong/SWIFT.git)

### 10.3 Efficient & Real-Time Inference



- **Flash-WAM: Modality-Aware Distillation for World Action Models** (see WAM)
- **WorldCache: Accelerating World Models for Free via Heterogeneous Token Caching**
  - Publication: arXiv 2026 (ICML 2026)
  - Highlights: Delivers up to 3.7× end-to-end speedups while maintaining 98% rollout quality. Accepted by ICML 2026.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.06331)

- **DISK: Dynamic Inference SKipping for World Models**
  - Publication: arXiv 2026
  - Highlights: Training-free adaptive inference for autoregressive world models.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2602.00440)

- **Planning in 8 Tokens: A Compact Discrete Tokenizer for Latent World Model (CompACT)**
  - Publication: arXiv 2026
  - Highlights: Compresses each observation to only 8 tokens.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2603.05438)

---

## 🧩 Simulation Platforms & Physics Engines


### 11.1 General Simulation Platforms

- **Isaac Lab: A GPU-Accelerated Simulation Framework for Multi-Modal Robot Learning**
  - Publication: arXiv 2025
  - Highlights: An open‑source GPU‑accelerated physics simulation engine jointly developed by NVIDIA, Google DeepMind, and Disney Research, specifically designed for robotics and simulation research. Built on NVIDIA Warp, it aims to provide a robust, scalable, and extensible platform for Physical AI.
  - Paper Link: [arXiv](https://arxiv.org/abs/2511.04831)

- **Cosmos World Foundation Model Platform for Physical AI**
  - Publication: arXiv 2025 (v3)
  - Highlights: NVIDIA's world foundation model platform for Physical AI, including video curation pipelines, pre‑trained world foundation models, post‑training examples, and video tokenizers to help developers build custom world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.03575)

- **HY-World 2.0: A Multi-Modal World Model for Reconstructing, Generating, and Simulating 3D Worlds**
  - Publication: arXiv 2026
  - Highlights: Tencent Hunyuan's multi‑modal world model framework that accepts text, single‑/multi‑view images, and videos as input, and generates 3DGS scenes. It includes WorldLens, a high‑performance 3DGS rendering platform for interactive exploration.
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.14268)

- **NVIDIA OmniDreams: Real-Time Generative World Model for Closed-Loop Autonomous Vehicle Simulation**
  - Publication: arXiv 2026
  - Highlights: NVIDIA's real‑time generative world model for closed‑loop autonomous driving simulation, with an action‑conditioned generative world model at its core, fine‑tuned on Cosmos for mid‑ and post‑training.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.03159)

- **SimWorld: An Open-ended Simulator for Agents in Physical Environments**
  - Publication: arXiv 2025
  - Highlights: A simulator built on Unreal Engine 5, designed for developing and evaluating LLM/VLM agents in rich real‑world scenarios, providing realistic and open‑ended world simulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2512.01078)

- **stable-worldmodel (SWM): Reproducible World Modeling Research and Evaluation**
  - Publication: arXiv 2026
  - Highlights: A modular, tested, and well‑documented ecosystem for world model research, offering efficient data collection tools, standardised environments, and planning algorithms.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2605.21800)

- **Nano World Models: A Minimalist Implementation of Future Video Prediction**
  - Publication: arXiv 2026
  - Highlights: A minimalist implementation of future video prediction that supports exporting generated videos to downstream 3D pipelines.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.23993)

- **A Survey: Learning Embodied Intelligence from Physical Simulators and World Models**
  - Publication: arXiv 2025
  - Highlights: A systematic survey of recent advances in learning embodied AI through the integration of physical simulators and world models.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2507.00917)

### 11.2 Differentiable Physics Engines & Neural Simulators

- **OrbiSim: World Models as Differentiable Physics Engines for Embodied Intelligence**
  - Publication: arXiv 2026
  - Highlights: Redefines world models as fully differentiable physics engines with a decoupled neural architecture (OrbiSim‑Dynamics and OrbiSim‑Vision), supporting end‑to‑end differentiable contact modelling, gradient‑based policy optimisation, and physical reasoning under sparse rewards.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.16395)

- **MoSim: Neural Motion Simulator — Pushing the Limit of World Models in Reinforcement Learning**
  - Publication: arXiv 2025
  - Highlights: A world model that predicts future physical states of embodied systems from current observations and actions, significantly outperforming prior work.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.07095)

- **GWM: Towards Scalable Gaussian World Models for Robotic Manipulation**
  - Publication: arXiv 2025
  - Highlights: A 3D Gaussian Splatting‑based world model that enhances visual representation learning and serves as a robust neural simulator for model‑based reinforcement learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.17600)

- **Physically Embodied Gaussian Splatting: A Realtime Correctable World Model for Robotics**
  - Publication: arXiv 2024
  - Highlights: A dual Gaussian‑Particle representation that models the physical world while supporting future state prediction and online observation correction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2406.10788)

- **PIN-WM: Learning Physics-Informed World Models for Non-Prehensile Manipulation**
  - Publication: arXiv 2025
  - Highlights: Employs differentiable physics simulation to end‑to‑end identify 3D rigid‑body dynamics systems from a small number of visual interaction trajectories.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.16693)

- **Physically Interpretable World Models (PIWM) via Weakly Supervised Representation Learning**
  - Publication: arXiv 2024
  - Highlights: Aligns latent representations with real‑world physical quantities and constrains their evolution using partially known physical dynamics.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2412.12870)

### 11.3 Interactive World Models & Game Engines

- **NeoWorld: Neural Simulation of Explorable Virtual Worlds via Progressive 3D Unfolding**
  - Publication: arXiv 2025
  - Highlights: A deep learning framework that supports user‑driven object manipulation and physics‑based dynamic simulation, enabling interactive world generation in continuously expanding 3D environments.
  - Paper Link: [arXiv](https://arxiv.org/abs/2509.24441)

- **Matrix-Game 2.0: An Open-Source, Real-Time, and Streaming Interactive World Model**
  - Publication: arXiv 2025
  - Highlights: Generates interactive videos in real time via few‑step autoregressive diffusion, addressing the long inference time of existing models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2508.13009)

- **Matrix-Game: Interactive World Foundation Model**
  - Publication: arXiv 2025
  - Highlights: An interactive world foundation model for controllable game‑world generation, trained with a two‑stage pipeline.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.18701)

- **Infinite-World: Scaling Interactive World Models to 1000-Frame Horizons via Pose-Free Hierarchical Memory**
  - Publication: arXiv 2026
  - Highlights: Extends interactive world models to 1000‑frame horizons through pose‑free hierarchical memory.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.02393)

- **MineWorld: a Real-Time and Open-Source Interactive World Model on Minecraft**
  - Publication: arXiv 2025
  - Highlights: A real‑time interactive world model on Minecraft that generates game scenes using a visual‑action autoregressive Transformer.
  - Paper Link: [arXiv](https://arxiv.org/abs/2504.08388)

- **LatticeWorld: A Multimodal Large Language Model-Empowered Framework for Interactive Complex World Generation**
  - Publication: arXiv 2025
  - Highlights: Takes text descriptions and visual instructions as multimodal input to create large‑scale 3D interactive worlds with dynamic agents, high‑fidelity physics simulation, and real‑time rendering.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2509.05263)

- **GameFactory: Creating New Games with Generative Interactive Videos**
  - Publication: arXiv 2025
  - Highlights: Creates new games using generative interactive videos.
  - Paper Link: [arXiv](https://arxiv.org/abs/2501.08325)

- **Position: Interactive Generative Video as Next-Generation Game Engine**
  - Publication: arXiv 2025
  - Highlights: Proposes interactive generative video (IGV) as the foundation of generative game engines (GGE), supporting unlimited novel content generation.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2503.17359)

### 11.4 Physics Simulation & Engine Integration


- **VDAWorld: World Modelling via VLM-Directed Abstraction and Simulation**
  - Publication: arXiv 2025
  - Highlights: VLMs act as agents to autonomously construct scene representations and select compatible physics simulators (rigid‑body, fluid, etc.), inferring latent dynamics from static scenes.
  - Paper Link: [arXiv](https://arxiv.org/abs/2512.11061)

- **PhysWorld: From Real Videos to World Models of Deformable Objects via Physics-Aware Demonstration Synthesis**
  - Publication: arXiv 2025
  - Highlights: Leverages simulators to generate physically plausible and diverse demonstrations, learning efficient world models for deformable objects that are 47× faster in inference than SOTA.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2510.21447)

- **LLMPhy: Complex Physical Reasoning Using Large Language Models and World Models**
  - Publication: arXiv 2024
  - Highlights: A zero‑shot black‑box optimisation framework that combines LLMs’ physical knowledge and program synthesis capabilities with built‑in world models in modern physics engines.
  - Paper Link: [arXiv](https://arxiv.org/abs/2411.08027)

- **RoboScape: Physics-informed Embodied World Model**
  - Publication: arXiv 2025
  - Highlights: A unified physics‑informed world model that jointly learns RGB video generation, temporal depth prediction, and adaptive keypoint tracking within a single framework.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.23135)

- **ContactGaussian-WM: Learning Physics-Grounded World Model from Videos**
  - Publication: arXiv 2024
  - Highlights: A differentiable physics‑grounded rigid‑body world model that learns physical laws from sparse videos, using a unified Gaussian representation for visual appearance and collision geometry.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2602.11021)

- **ProTerrain: Probabilistic Physics-Informed Rough Terrain World Modeling**
  - Publication: arXiv 2025
  - Highlights: Models spatially correlated uncertainty of terrain parameters as a probabilistic world model, propagated through differentiable physics engines for probabilistic trajectory prediction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.19364)

- **PhysMani: Physics-principled 3D World Model for Dynamic Object Manipulation**
  - Publication: arXiv 2026 (ECCV 2026)
  - Highlights: Combines a physics‑principled 3D Gaussian world model with a future‑aware action policy model for dynamic object manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.01938)

### 11.5 Benchmarks for World Model Simulation

- **World-in-World: World Models in a Closed-Loop World**
  - Publication: arXiv 2025
  - Highlights: The first open platform for benchmarking world models in a closed‑loop world, mirroring real agent‑environment interactions, with unified online planning strategies and standardised action APIs.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.18135)

- **WorldArena: A Unified Benchmark for Evaluating Perception and Functional Utility of Embodied World Models**
  - Publication: arXiv 2025
  - Highlights: A unified benchmark for evaluating perception and functional utility of embodied world models.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2602.08971)

- **SmallWorlds: Assessing Dynamics Understanding of World Models in Isolated Environments**
  - Publication: arXiv 2025
  - Highlights: Evaluates world models’ understanding of fundamental physics principles (e.g., gravity, elastic collisions) under isolated and precisely controlled dynamics conditions.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2511.23465)

- **WorldSimBench: Towards Video Generation Models as World Simulators**
  - Publication: arXiv 2024
  - Highlights: A benchmark for evaluating video generation models as world simulators.
  - Paper Link: [arXiv](https://arxiv.org/abs/2410.18072)

- **WorldBench: Disambiguating Physics for Diagnostic Evaluation of World Models**
  - Publication: arXiv 2025
  - Highlights: Provides a more fine‑grained and scalable framework through concept‑specific evaluation, rigorously assessing the physical reasoning capabilities of video generation and world models.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2601.21282)

- **WorldPrediction: A Benchmark for High-level World Modeling and Long-horizon Procedural Planning**
  - Publication: arXiv 2025
  - Highlights: A video‑based benchmark for evaluating AI models’ world modeling and procedural planning abilities.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2506.04363)

- **RoboWorld: Fast and Reliable Neural Simulators for Generalist Robot Policy Evaluation**
  - Publication: arXiv 2026
  - Highlights: An automated evaluation pipeline combining fast autoregressive video world models with task‑progress‑aware VLM scoring.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2607.01060)

### 11.6 Code Agents & Simulation Construction

- **Coding Agent Is Good As World Simulator**
  - Publication: arXiv 2026
  - Highlights: Builds physics‑based world models through executable simulation code, with a framework coordinating planning, code generation, visual review, and physics analysis agents.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2605.14398)

- **Agentic Real2Sim: Physics-based World Modeling with Vision-Language Agents**
  - Publication: arXiv 2026
  - Highlights: Converts real‑world object‑robot interaction recordings into simulatable episodic digital twins, preserving observations, geometry, robot interactions, and object states.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2607.19190)

- **Web World Models (WWM)**
  - Publication: arXiv 2025
  - Highlights: World states and “physics” are implemented in ordinary web code to ensure logical consistency; LLMs generate context, narratives, and high‑level decisions on top of this structured latent state.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2512.23676)

### 11.7 Surveys & Perspectives

- **Simulating the Visual World with Artificial Intelligence: A Roadmap**
  - Publication: arXiv 2025
  - Highlights: Defines physical world models as complex digital engines that encode comprehensive world knowledge to simulate real‑world dynamics, following intrinsic physical and mathematical laws.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2511.08585)

- **From Generative Engines to Actionable Simulators: The Imperative of Physical Grounding in World Models**
  - Publication: arXiv 2026
  - Highlights: Emphasises the necessity of physical grounding for world models to transition from generative engines to actionable simulators.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.15533)

- **Critique of World Model**
  - Publication: arXiv 2025
  - Highlights: Argues that the primary goal of world models is to simulate all actionable possibilities of the real world for purposeful reasoning and action.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2507.05169)

---

## 🔬 Theory, Interpretability & Positions


- **Grounding Spatial Relations in a Compact World Model: Instruction Leakage and a Goal-Free Dynamics Fix**
  - Publication: arXiv 2026
  - Highlights: Identifies "instruction leakage" problem in goal-conditioned world models and proposes a fix.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.06925)

- **Path-Measure Dynamics of Attention-Driven World Models: A Nonlocal Onsager–Machlup Approach**
  - Publication: arXiv 2026
  - Highlights: Studies how attention enables world models to condition on entire histories for long-term memory.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2607.02154)

- **Why We Need World Models for AGI: Where LLMs Fail and How World Models May Outperform**
  - Publication: arXiv 2026
  - Highlights: Argues that world models operate on latent states, making causal prediction and planning more natural.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2605.23972)

- **Research on World Models Is Not Merely Injecting World Knowledge into Specific Tasks**
  - Publication: arXiv 2026
  - Highlights: Argues that robust world models should be a normative framework integrating interaction, perception, reasoning, and spatial representation.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2602.01630)

- **GeoWorld: Geometric World Models**
  - Publication: arXiv 2026
  - Highlights: Energy-based predictive world model for multi-step visual planning via latent energy landscapes.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2602.23058)

- **From Kepler to Newton: Inductive Biases Guide Learned World Models in Transformers**
  - Publication: arXiv 2026
  - Highlights: Shows how inductive biases guide transformers to learn world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.06923)

- **General agents Contain World Models**
  - Publication: arXiv 2025
  - Highlights: General agents contain world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2506.01622)

- **When Do Neural Networks Learn World Models?**
  - Publication: arXiv 2025
  - Highlights: Investigates when neural networks learn world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2502.09297)

- **Reconstruction or Semantics? What Makes a Latent Space Useful for Robotic World Models**
  - Publication: arXiv 2025
  - Highlights: Investigates what makes a latent space useful for robotic world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.06388)

- **What Does it Mean for a Neural Network to Learn a 'World Model'?**
  - Publication: arXiv 2025
  - Highlights: Conceptual analysis of what it means for a neural network to learn a world model.
  - Paper Link: [arXiv](https://arxiv.org/abs/2507.21513)

- **How Hard is it to Confuse a World Model?**
  - Publication: arXiv 2025
  - Highlights: Studies the robustness of world models to confusion.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.21232)

- **Partially Observable Safety: How Well Do Latent World Models Understand Partially Observable Safety Constraints?**
  - Publication: arXiv 2025
  - Highlights: Evaluates latent world models on partially observable safety constraints.
  - Paper Link: [arXiv](https://arxiv.org/abs/2510.06492)

- **ICL Emergence: Context and Diversity Matter – The Emergence of In-Context Learning in World Models**
  - Publication: arXiv 2025
  - Highlights: Studies the emergence of in-context learning in world models.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2509.22353)

- **Linear Spatial World Models Emerge in Large Language Models**
  - Publication: arXiv 2025
  - Highlights: Linear spatial world models emerge in LLMs.
  - Paper Link: [arXiv](https://arxiv.org/pdf/2506.02996) | [Code](https://github.com/matthieu-perso/spatial_world_models)

- **Scaling Laws for Pre-training Agents and World Models**
  - Publication: arXiv 2024
  - Highlights: Scaling laws for pre-training agents and world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2411.04434)

- **Revisiting the Othello World Model Hypothesis**
  - Publication: arXiv 2025
  - Highlights: Revisits the Othello world model hypothesis.
  - Paper Link: [arXiv](https://arxiv.org/abs/2503.04421)

- **Transformers Use Causal World Models in Maze-Solving Tasks**
  - Publication: arXiv 2024
  - Highlights: Transformers use causal world models in maze-solving tasks.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.11867)

- **A Causal World Model Underlying Next Token Prediction: Exploring GPT in a Controlled Environment**
  - Publication: arXiv 2024
  - Highlights: Explores the causal world model underlying next-token prediction in GPT.
  - Paper Link: [arXiv](https://arxiv.org/abs/2412.07446)

- **The Trinity of Consistency as a Defining Principle for General World Models**
  - Publication: arXiv 2026
  - Highlights: Proposes that world models must be grounded on the trinity of consistency: modal, spatial, and temporal.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.23152)

- **Lifting Embodied World Models for Planning and Control**
  - Publication: arXiv 2026
  - Highlights: Lifting methods for embodied world models in planning and control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.26182)

- **From Generative Engines to Actionable Simulators: The Imperative of Physical Grounding in World Models**
  - Publication: arXiv 2026
  - Highlights: Emphasizes the imperative of physical grounding in world models to transition from generative engines to actionable simulators.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.15533)



---

## 🔗 Related Awesome Lists

- [Awesome-World-Model-for-Autonomous-Driving](https://github.com/LMD0311/Awesome-World-Model)
- [Awesome-World-Model-for-Robotics](https://github.com/leofan90/Awesome-World-Models)
- [Awesome World Models for Healthcare](https://github.com/chengwang96/Awesome-World-Models-for-Healthcare)
- [General World Models Survey](https://github.com/GigaAI-research/General-World-Models-Survey)
- [Physics Cognition in Video Generation](https://github.com/minnie-lin/Awesome-Physics-Cognition-based-Video-Generation)

---

## 🔑 Key Research Challenges

Based on the synthesis of newly added papers, additional key research challenges include:

- **Persistent State Core** — World models need to maintain persistent world states independent of observations, rather than rendering plausible frames only at observation time.
- **Physical Grounding** — Shifting from visual engines to actionable simulators, emphasizing structured 4D interfaces, constraint-aware dynamics, and closed-loop evaluation.
- **Instruction Leakage** — Identifying and fixing instruction leakage in goal-conditioned world models.
- **Counterfactual Controllability** — The core criterion for self-evolving world models is counterfactual controllability: the ability to ask what would happen under a given action.
- **Model Mismatch** — Adaptive re-planning under model mismatch in neural world-model predictive control.
- **Reactive Capability** — Evaluating how well world model simulators respond to agent behaviors that differ from the log.
- **Modality-Aware Distillation** — Developing distillation techniques that respect different noise regimes across modalities (video vs. action).
- **Verifiability** — In systems that cannot fail, the biggest obstacle to deploying world models is verifiability rather than prediction fidelity.

---

## ❤️ Contact
If you have suggestions for new papers or datasets, spot any inaccuracies, or find this curated resource list helpful, feel free to reach out to Yuanliang Sun via email at sun254667307@gmail.com.
For inquiries about research internship opportunities in world models, you are welcome to contact me at any time.

## 📄 License
CC0 1.0 Universal. Full terms available in the `LICENSE` file of this repository.
