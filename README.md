<div align="center">

# 🎥 Awesome World Models

<p align="center">
  <img src="wm_banner.png" alt="Awesome World Models" width="100%">
</p>

<p align="center">
  <img src="QRcode.png" alt="Awesome World Models" width="100%">
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
2. [Foundation Papers & Technical Reports](#-foundation-papers--technical-reports)
3. [Core World Model Paradigms](#-core-world-model-paradigms)
   - 3.1 [Language-Based World Models](#31-language-based-world-models)
   - 3.2 [Visual / Video World Models](#32-visual--video-world-models)
   - 3.3 [3D & 4D World Models](#33-3d--4d-world-models)
   - 3.4 [Latent Space World Models](#34-latent-space-world-models)
   - 3.5 [Object-Centric World Models](#35-object-centric-world-models)
   - 3.6 [Symbolic & Neuro-Symbolic World Models](#36-symbolic--neuro-symbolic-world-models)
4. [Interactive World Models](#-interactive-world-models)
   - 4.1 [General Interactive Frameworks](#41-general-interactive-frameworks)
   - 4.2 [Game & Open-World Exploration](#42-game--open-world-exploration)
5. [World Action Models (WAM) & VLA Integration](#-world-action-models-wam--vla-integration)
   - 5.1 [Cascaded WAM](#51-cascaded-wam)
   - 5.2 [Joint WAM](#52-joint-wam)
   - 5.3 [World Models for VLA Training & Evaluation](#53-world-models-for-vla-training--evaluation)
6. [Model-Based RL World Models](#-model-based-rl-world-models)
   - 6.1 [Classic Series](#61-classic-series)
   - 6.2 [Continuous Control](#62-continuous-control)
   - 6.3 [Offline & Generalization](#63-offline--generalization)
7. [Application Domains](#-application-domains)
   - 7.1 [Robotics & Embodied AI](#71-robotics--embodied-ai)
   - 7.2 [Autonomous Driving](#72-autonomous-driving)
   - 7.3 [GUI / Computer-Use Agents](#73-gui--computer-use-agents)
   - 7.4 [Scientific Discovery](#74-scientific-discovery)
   - 7.5 [Social & Economic Simulation](#75-social--economic-simulation)
8. [Datasets & Benchmarks](#-datasets--benchmarks)
   - 8.1 [General World Modeling](#81-general-world-modeling)
   - 8.2 [Physics & Causality](#82-physics--causality)
   - 8.3 [Domain-Specific Benchmarks](#83-domain-specific-benchmarks)
9. [Training & Inference Techniques](#-training--inference-techniques)
   - 9.1 [Memory Mechanisms](#91-memory-mechanisms)
   - 9.2 [Post-Training & Test-Time Scaling](#92-post-training--test-time-scaling)
   - 9.3 [Efficient & Real-Time Inference](#93-efficient--real-time-inference)
10. [Simulation Platforms & Physics Engines](#-simulation-platforms--physics-engines)
11. [Theory & Interpretability](#-theory--interpretability)
12. [Related Awesome Lists](#-related-awesome-lists)
13. [Key Research Challenges](#-key-research-challenges)
14. [Contact](#-contact)
15. [License](#-license)

---

## 📚 Surveys & Overviews

- **A Definition and Roadmap for World Models**
  - Publication: arXiv 2026 
  - Highlights: Provides a scientific definition of world models, discussions of their key technical aspects, and a staged roadmap for developing effective world models.
  - Paper Link: [arXiv](https://export.arxiv.org/abs/2607.06401)

- **World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications**
  - Publication: arXiv 2026 
  - Highlights: Comprehensive survey covering architectures, methodologies, reasoning paradigms, and applications of world models; proposes a multi-axis taxonomy organized along four dimensions.
  - Paper Link: [arXiv](https://export.arxiv.org/abs/2606.00133)

- **A Comprehensive Survey on World Models for Embodied AI**
  - Publication: arXiv 2026 (Revised 25 Jun 2026)
  - Highlights: Presents a unified framework for world models in embodied AI with a three-axis taxonomy encompassing Functionality, Decision-Coupled vs. General-Purpose, and Temporal Modeling.
  - Paper Link: [arXiv](https://export.arxiv.org/abs/2510.16732)

- **Towards Interactive Video World Modeling: Frontiers, Challenges, Benchmarks, and Future Trends**
  - Publication: arXiv 2026 
  - Highlights: Systematically reviews recent research trends, technical developments, evaluation benchmarks, and future directions in interactive world modeling.
  - Paper Link: [arXiv](https://export.arxiv.org/abs/2606.01164)

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

- **Reduced-Order Models: The Mother of World Models**
  - Publication: arXiv 2026 
  - Highlights: Argues that the functional anatomy of a world model was independently developed decades earlier in the model-order-reduction and control literature.
  - Paper Link: [arXiv](https://export.arxiv.org/abs/2607.03198)

- **A Tutorial on World Models and Physical AI**
  - Publication: arXiv 2026 
  - Highlights: Presents a coherent framework unifying diverse world modeling approaches through shared predictive structure; connects world modeling techniques to physical AI applications such as robotics and autonomous driving.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.12783)

- **Beyond the Autoregressive Horizon: A Comprehensive Survey of Diffusion Models, World Modelling, and State Space Models for Code**
  - Publication: arXiv 2026 
  - Highlights: Comprehensive survey of diffusion models, state space models, and Code World Models (CWMs) for the code domain.
  - Paper Link: [arXiv](https://export.arxiv.org/abs/2606.23690)

- **From Digital Twins to World Models: Opportunities, Challenges, and Applications for Mobile Edge General Intelligence**
  - Publication: arXiv 2026 
  - Highlights: Systematically reviews the transition from digital twins to world models and their role in enabling mobile edge general intelligence.
  - Paper Link: [arXiv](https://export.arxiv.org/abs/2603.17420)

- **Safety, Security, and Cognitive Risks in World Models**
  - Publication: arXiv 2026 
  - Highlights: Surveys world model architectures and their deployment contexts in safety-critical domains, characterizing the world model asset inventory and threat surface.
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.10644)

---

## 🧠 Core World Model Paradigms

### 3.2 Visual / Video World Models

- **Advancing Open-source World Models (LingBot-World)**
  - Publication: arXiv 2026 
  - Highlights: LingBot-World is presented, an open-sourced world simulator stemming from video generation that maintains high fidelity and robust dynamics in a broad spectrum of environments, including realism, scientific contexts, cartoon styles, and beyond.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.20540)

- **Infinite Worlds with Versatile Interactions (LingBot-World 2.0 / LingBot-World-Infinity)**
  - Publication: arXiv 2026 
  - Highlights: An advanced iteration of LingBot-World featuring unbounded interaction horizon, 60 fps 720p real-time rendering, diverse interactive elements, and integration of an agentic harness with pilot and director agents.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.07534)

- **Next Forcing: Causal World Modeling with Multi-Chunk Prediction**
  - Publication: arXiv 2026 
  - Highlights: A multi-chunk prediction (MCP) framework for causal world modeling that enables faster training, higher accuracy, and accelerated inference. Achieves 94.1/93.5% on RoboTwin benchmark.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.11187)

- **Orca: The World is in Your Mind**
  - Publication: arXiv 2026 
  - Highlights: A general world foundation model from BAAI that learns a unified world latent space from multimodal world signals and exposes it through multimodal readout interfaces. Pre-trained on 125K hours of video data and 160M event annotations.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.30534)

- **Qwen-RobotWorld: Unifying Embodied World Modeling through Language-Conditioned Video Generation**
  - Publication: arXiv 2026 
  - Highlights: A language-conditioned video world model that predicts future visual trajectories across multiple robotic domains using a double-stream diffusion transformer and an 8.6M video-text embodied world knowledge corpus.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.17030)

- **ABot-PhysWorld: Interactive World Foundation Model for Robotic Manipulation with Physics Alignment**
  - Publication: arXiv 2026 
  - Highlights: A 14B Diffusion Transformer model that generates visually realistic, physically plausible, and action-controllable videos for robotic manipulation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.23376)

- **Nano World Models: A Minimalist Implementation of Future Video Prediction**
  - Publication: arXiv 2026 
  - Highlights: A minimalist codebase for future video prediction centered around diffusion forcing that provides a unified interface for generative objectives, model scales, action-conditioning mechanisms, and evaluation protocols.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.09301)

- **A Mechanistic View on Video Generation as World Models: State and Dynamics**
  - Publication: arXiv 2026 
  - Highlights: Proposes a taxonomy centered on State Construction and Dynamics Modeling, categorizing state construction into implicit paradigms (context management) and explicit paradigms (latent compression).
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.17067)

- **Latent Video Prediction Learns Better World Models**
  - Publication: arXiv 2026 
  - Highlights: First systematic study on the robustness of latent-predictive video models as world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.15618)

- **PhyWorld: Physics-Faithful World Model for Video Generation**
  - Publication: arXiv 2026 
  - Highlights: Generates temporally coherent and physically plausible scene continuations through two-stage post-training (flow matching fine-tuning + DPO physics preference alignment).
  - Paper Link: [arXiv](https://export.arxiv.org/abs/2605.19242)

- **Autonomous Video Generation with Counterfactual Controllability for Self-Evolving World Models**
  - Publication: arXiv 2026 
  - Highlights: Achieves self-evolving world models through autonomous video generation with counterfactual controllability.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.24152)

- **Directing the World: Fast Autoregressive Video Generation with Compositional Human-Camera Control**
  - Publication: arXiv 2026 
  - Highlights: Fast autoregressive framework for controllable world-model video generation with compositional human-motion and camera-trajectory control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.27964)

### 3.3 3D & 4D World Models

- **HY-World 2.0: A Multi-Modal World Model for Reconstructing, Generating, and Simulating 3D Worlds**
  - Publication: arXiv 2026 
  - Highlights: A multi-modal world model framework that accommodates diverse input modalities (text prompts, single-view images, multi-view images, videos) and produces 3D world representations (meshes / Gaussian Splattings).
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.09772)

- **3D-Belief: Embodied Belief Inference via Generative 3D World Modeling**
  - Publication: arXiv 2026 
  - Highlights: Redefines world modeling as embodied belief inference in 3D space, inferring actionable 3D beliefs from partial observations and updating them online.
  - Paper Link: [arXiv](https://export.arxiv.org/abs/2605.11367)

- **InSpatio-WorldFM: An Open-Source Real-Time Generative Frame Model**
  - Publication: arXiv 2026 
  - Highlights: An open-source real-time frame model for spatial intelligence that achieves strong multi-view consistency while supporting interactive exploration on consumer-grade GPUs.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.11911)

- **InSpatio-World: A Real-Time 4D World Simulator via Spatiotemporal Autoregressive Modeling**
  - Publication: arXiv 2026 
  - Highlights: Translates user interactions into precise camera trajectories and integrates them into the spatial reasoning process for high-precision camera-controlled generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.05823)

- **M⁴World: A Multi-view Multimodal Driving World Model for Interactive Object Manipulation and Minute-long Streaming**
  - Publication: arXiv 2026 
  - Highlights: Multi-view multimodal generative driving world model synthesizing future surround-view video streams and synchronized LiDAR scans, supporting interactive object manipulation and minute-long stable streaming.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.14005)

### 3.4 Latent Space World Models

- **Orca: The World is in Your Mind**
  - Publication: arXiv 2026 
  - Highlights: A general world foundation model from BAAI that learns a unified world latent space from multimodal world signals. Orca learns through two complementary paradigms: unconscious learning (dense natural state transitions from continuous videos) and conscious learning (sparse meaningful state transitions by language-described events and VQA supervision).
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.30534)

- **Looped World Models**
  - Publication: arXiv 2026 
  - Highlights: First recurrent architecture for world modeling that iteratively refines latent environment states through parameter-shared transformer blocks, achieving 100× parameter efficiency improvement over traditional methods.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.18208)

- **EMERALD: Accurate and Efficient World Modeling with Masked Latent Transformers**
  - Publication: arXiv 2026 
  - Highlights: An efficient world model that generates accurate trajectories in latent space using spatial latent states and MaskGIT prediction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.03153)

- **ThinkJEPA: Empowering Latent World Models with Large Vision-Language Reasoning Model**
  - Publication: arXiv 2026 
  - Highlights: VLM-guided JEPA-style latent world modeling framework combining dense frame dynamics modeling with long-horizon semantic guidance through dual temporal pathways.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.22281)

- **FF-JEPA: Long-Horizon Planning in World Models with Latent Planners**
  - Publication: arXiv 2026 
  - Highlights: Forward-Forward JEPA (FF-JEPA) unified framework bridging world models, forward prediction, and inverse dynamics reasoning for goal-directed behavior without explicit goal images.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.09311)

- **Kairos: A Native World Model Stack for Physical AI**
  - Publication: arXiv 2026 
  - Highlights: Explicitly frameworks world models as systems that learn physically meaningful predictive structures within abstract representation spaces.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.16533)

### 3.5 Object-Centric World Models

- **Latent Particle World Models: Self-supervised Object-centric Stochastic Dynamics Modeling**
  - Publication: ICLR 2026 Oral
  - Highlights: Self-supervised object-centric world model that scales to real-world multi-object datasets for decision-making.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.04553)

### 3.6 Symbolic & Neuro-Symbolic World Models

- **Graph World Models: Concepts, Taxonomy, and Future Directions**
  - Publication: arXiv 2026 
  - Highlights: Proposes a taxonomy based on relational inductive biases, categorizing GWMs into spatial RIB (topological abstraction), physical RIB (dynamics simulation), and logical RIB (causal semantic reasoning).
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.12345)

- **OPINE-World: Programmatic World Modeling with Ontology-error-Prioritized Interactive Exploration**
  - Publication: arXiv 2026 
  - Highlights: Programmatic world modeling based on ontology-error-prioritized interactive exploration.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.01531)

---

## 🎮 Interactive World Models

### 4.1 General Interactive Frameworks

- **Qwen-AgentWorld: Language World Models for General Agents**
  - Publication: arXiv 2026 
  - Highlights: The first language world models (Qwen-AgentWorld-35B-A3B and Qwen-AgentWorld-397B-A17B) capable of simulating agentic environments covering 7 domains via long chain-of-thought reasoning. Leverages more than 10M environment interaction trajectories.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.24597)

- **LingBot-World (Advancing Open-source World Models)**
  - Publication: arXiv 2026 
  - Highlights: An open-sourced world simulator stemming from video generation that maintains high fidelity and robust dynamics across a broad spectrum of environments.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.20540)

- **LingBot-World-Infinity (Infinite Worlds with Versatile Interactions)**
  - Publication: arXiv 2026 
  - Highlights: Achieves unbounded interaction horizon with consistent output quality, distills a real-time variant for 60 fps 720p video streams, and introduces diverse interactive elements and multi-player support.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.07534)

- **ActWorld: From Explorable to Interactive World Model via Action-Aware Memory**
  - Publication: arXiv 2026 
  - Highlights: Extends navigation-centric generators to support object interactions during rollouts; constructs a dataset of 100k interactive videos; introduces hierarchical action-aware memory design.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.17730)

- **MoWorld: A Flash World Model**
  - Publication: arXiv 2026 
  - Highlights: First NPU-based real-time interactive world model achieving 50 FPS with only 30%-50% of the inference cost of existing world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.06216)

- **WorldDirector: Building Controllable World Simulators with Persistent Dynamic Memory**
  - Publication: arXiv 2026 
  - Highlights: Highly controllable video world model framework that explicitly decouples semantic motion orchestration from visual generation, coordinating 3D trajectories and camera motion through LLMs.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.02517)

- **Stateful Worlds, Stateless Elasticity: Exact-State Serving for Interactive World Models**
  - Publication: arXiv 2026 
  - Highlights: Exact-state serving framework for interactive world models; WorldMove enables live session migration within 18.8ms on the same node.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.10389)

- **From Pixels to States: Rethinking Interactive World Models as Game Engines**
  - Publication: arXiv 2026 
  - Highlights: Examines interactive game world modeling along four dimensions: player action control, game state dynamics, state-observation persistence, and real-time interactive generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.14076)

### 4.2 Game & Open-World Exploration

- **What if? Emulative Simulation with World Models for Situated Reasoning (WanderDream)**
  - Publication: arXiv 2026 
  - Highlights: First large-scale dataset designed for emulative simulation of mental exploration, enabling models to reason without active exploration.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.06193)

---

## 🤖 World Action Models (WAM) & VLA Integration

### 5.1 Cascaded WAM

- **Flash-WAM: Modality-Aware Distillation for World Action Models**
  - Publication: arXiv 2026 
  - Highlights: A modality-aware step-distillation framework that compresses WAM inference to a single step per modality. On RoboTwin 2.0, reduces per-chunk latency from seconds to 8.1 ms (348× speedup) on NVIDIA L40S.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.05254)

### 5.2 Joint WAM

- **Native Video-Action Pretraining for Generalizable Robot Control (LingBot-VA 2.0)**
  - Publication: arXiv 2026 
  - Highlights: A video-action foundation model built from the ground up for embodiment, featuring a semantic visual-action tokenizer, causal pretraining paradigm, sparse MoE backbone, and enhanced asynchronous inference scheme for real-time closed-loop control.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.08639)

- **DiM-WAM: World Action Modeling with Diverse Historical Event Memory**
  - Publication: arXiv 2026 
  - Highlights: Augments a WAM with Diverse Historical Event Memory (DHEM) using bank-conditioned candidate features, novelty-aware selection, and accumulated-mass-weighted fusion to retain complementary event tokens in bounded memory.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.27677)

- **WorldBagel: Uncovering the Power of Unified Multimodal Models for Vision-Language-Action-World Modeling**
  - Publication: arXiv 2026 
  - Highlights: A unified VLAW framework built on BAGEL, consistently outperforming task-specific alternatives on LIBERO, Language Table, and Franka.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.03461)

### 5.3 World Models for VLA Training & Evaluation

- **WEAVER: Better, Faster, Longer: An Effective World Model for Robotic Manipulation**
  - Publication: arXiv 2026 
  - Highlights: A multi-view WM trained with flow-matching loss to predict future latents and reward values, achieving SOTA on robotic manipulation tasks.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.13672)

- **PAIWorld: A 3D-Consistent World Foundation Model for Robotic Manipulation**
  - Publication: arXiv 2026 
  - Highlights: A 3D-consistent world foundation model built upon a DiT-based architecture, ranking 1st on AgiBot-Challenge2026 leaderboard.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.18375)

- **WAM-RL: World-Action Model Reinforcement Learning with Reconstruction Rewards and Online Video SFT**
  - Publication: arXiv 2026 
  - Highlights: First work to introduce reinforcement learning into the World-Action paradigm, jointly optimizing world models and action models through online environment interaction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.17906)

- **Reinforcing VLAs in Task-Agnostic World Models (RAW-Dream)**
  - Publication: arXiv 2026 
  - Highlights: A novel paradigm that completely decouples world model learning from downstream task dependencies.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.12334)

- **RoboDream: Compositional World Models for Scalable Robot Data Synthesis**
  - Publication: arXiv 2026 
  - Highlights: A generalizable embodiment-centric world model that enables scalable data generation by synthesizing photorealistic demonstrations with novel objects, scenes, and viewpoints.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.02577)

- **Hi-WM: Human-in-the-World-Model for Scalable Robot Post-Training**
  - Publication: arXiv 2026 
  - Highlights: A post-training framework that uses a learned world model as a reusable corrective substrate for failure-targeted policy improvement. Improves real-world success by 37.9 points on average.
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.21741)

---

## 🧪 Model-Based RL World Models

### 6.2 Continuous Control

- **Scaling World-Model Reinforcement Learning Through Diffusion Policy Optimization**
  - Publication: arXiv 2026 
  - Highlights: Unifies search and policy optimization through diffusion policy representation, unlocking the potential of world models for scalable policy learning.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.26282)

- **JEDI: Joint Embedding Diffusion World Model for Online Model-Based Reinforcement Learning**
  - Publication: arXiv 2026 
  - Highlights: Joint embedding diffusion world model for online model-based RL.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.16034)

- **ACID: Action Consistency via Inverse Dynamics for Planning with World Models**
  - Publication: arXiv 2026 
  - Highlights: Achieves action consistency via inverse dynamics for planning with world models.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.01489)

### 6.3 Offline & Generalization

- **CoMap: Co-Evolving World Models and Agent Policies for LLM Agents**
  - Publication: arXiv 2026 
  - Highlights: A novel framework that co-evolves textual world models and agent policies through closed-loop interaction. At each decision step, the world model predicts future state feedback for candidate actions.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.01695)

- **Policy and World Modeling Co-Training for Language Agents (PaW)**
  - Publication: arXiv 2026 
  - Highlights: A policy and world modeling co-training framework that adds auxiliary WM supervision to the same policy during RL without changing the inference paradigm.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.02388)

- **Dreaming of Others: Latent Teammate Modeling in World Models for Multi-Agent RL**
  - Publication: arXiv 2026 
  - Highlights: Treats teammates as structured learnable components in the agent's world model, positioning the world model not only as a predictor of environment dynamics but also as a simulator of social behavior.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.01694)

---

## 🎯 Application Domains

### 7.1 Robotics & Embodied AI

- **Qwen-RobotWorld: Unifying Embodied World Modeling through Language-Conditioned Video Generation**
  - Publication: arXiv 2026 
  - Highlights: A language-conditioned video world model for embodied intelligence that predicts physically grounded future visual trajectories across robotic manipulation, autonomous driving, indoor navigation, and human-to-robot transfer.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.17030)

- **PAIWorld: A 3D-Consistent World Foundation Model for Robotic Manipulation**
  - Publication: arXiv 2026 
  - Highlights: Built upon a DiT-based world foundation model, PAIWorld attains state-of-the-art multi-view 3D consistency on robotic manipulation benchmarks.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.18375)

- **ABot-PhysWorld: Interactive World Foundation Model for Robotic Manipulation with Physics Alignment**
  - Publication: arXiv 2026 
  - Highlights: A 14B Diffusion Transformer model that generates visually realistic, physically plausible, and action-controllable videos.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.23376)

- **ContactWorld: What Matters in Vision-Tactile World Models for Contact-Rich Manipulation**
  - Publication: arXiv 2026 
  - Highlights: A benchmark and systematic empirical study of vision-tactile world models spanning 12 contact-rich manipulation tasks, including insertion, disassembly, screwing, and exploratory interaction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.13877)

- **Hi-WM: Human-in-the-World-Model for Scalable Robot Post-Training**
  - Publication: arXiv 2026 
  - Highlights: A post-training framework that uses a learned world model as a reusable corrective sandbox for improving pretrained robot policies after deployment.
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.21741)

- **Causally Debiased Latent Action Model for Embodied Action Conditioned World Models**
  - Publication: arXiv 2026 
  - Highlights: Action-conditioned world models (ACWMs) aim to simulate future observations conditioned on embodied actions, offering a promising foundation for robot planning, policy evaluation, and data augmentation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.09461)

- **Physically Viable World Models: A Case for Query-Conditioned Embodied AI**
  - Publication: arXiv 2026 
  - Highlights: Argues that world models for embodied AI must be able to answer intervention queries, representing the physical structure of control action outcomes.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.18947)

- **NavWM: A Unified Navigation World Model for Foresight-Driven Planning**
  - Publication: arXiv 2026 
  - Highlights: A unified navigation world model that seamlessly integrates latent world reasoning, multimodal action prediction, and controllable visual generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.17302)

### 7.2 Autonomous Driving

- **M⁴World: A Multi-view Multimodal Driving World Model for Interactive Object Manipulation and Minute-long Streaming**
  - Publication: arXiv 2026 
  - Highlights: Multi-view multimodal generative driving world model synthesizing future surround-view video streams and synchronized LiDAR scans while supporting interactive object manipulation and stable minute-long streaming.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.14005)

- **AutoWorld: Scaling Multi-Agent Traffic Simulation with Self-Supervised World Models**
  - Publication: arXiv 2026 
  - Highlights: A traffic simulation framework that employs a world model learned from unlabeled occupancy representations of LiDAR data.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.28963)

- **Reason--Imagine--Act: Closed-Loop LLM Decision Making with World Models for Autonomous Driving**
  - Publication: arXiv 2026 
  - Highlights: Large language models (LLMs) for autonomous driving with explicit dynamics verification through world models at decision time.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.14723)

- **ReactSim-Bench: Benchmarking Reactive Behavior World Model Simulation in Autonomous Driving**
  - Publication: arXiv 2026 
  - Highlights: A benchmark for evaluating the reactive capability of behavior world model simulation in autonomous driving, with 2,636 test scenarios.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.14058)

- **ResWorld: Temporal Residual World Model for End-to-End Autonomous Driving**
  - Publication: arXiv 2026 
  - Highlights: A Temporal Residual World Model that focuses on dynamic object modeling, taking only temporal residuals as input for precise future spatial distribution prediction.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.08261)

- **Xiaomi Auto World Model: A Joint World Model Integrating Reconstruction and Generation for Autonomous Driving**
  - Publication: arXiv 2026 
  - Highlights: A unified technical system addressing the two core capabilities of driving world models: world representation and world generation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.12701)

- **CausalDrive: Real-time Causal World Models for Autonomous Driving**
  - Publication: arXiv 2026 
  - Highlights: Real-time causal world models achieving 12 FPS interaction speed, relying only on initial front view, ego trajectory, and macro text prompts.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.15341)

- **LWDrive: Layer-Wise World-Model-Guided Vision-Language Model Planning for Autonomous Driving**
  - Publication: arXiv 2026 
  - Highlights: A layer-wise world-model-guided VLM planning framework that refines coarse trajectories through layer-wise world model guidance.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.29879)

- **Toward Physically Consistent Driving Video World Models under Challenging Trajectories (PhyGenesis)**
  - Publication: arXiv 2026 
  - Highlights: Generates driving videos with high visual fidelity and strong physical consistency.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.24506)

### 7.3 GUI / Computer-Use Agents

- **WebWorld: A Large-Scale World Model for Web Agent Training**
  - Publication: arXiv 2026 
  - Highlights: A large-scale world model for web-agent training built from over one million real web interactions. Outperforms GPT-5 as a world model for inference-time search and exhibits cross-domain generalization to code, GUI, and game environments.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.14721)

- **Qwen-AgentWorld: Language World Models for General Agents**
  - Publication: arXiv 2026 
  - Highlights: Language world models capable of simulating agentic environments covering 7 domains via long chain-of-thought reasoning, with 35B-A3B and 397B-A17B parameter scales.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.24597)

- **From Tokens to States: LLMs as a Special Case of World Models and the Continuous Path Beyond**
  - Publication: arXiv 2026 
  - Highlights: A position paper exploring LLMs as a special case of world models and the path beyond.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.28127)

- **Computer-Using World Model (CUWM)**
  - Publication: arXiv 2026 
  - Highlights: A desktop software world model that predicts the next UI state given the current state and candidate actions.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.15003)

- **Code2World: A GUI World Model via Renderable Code Generation**
  - Publication: arXiv 2026 
  - Highlights: Models GUI dynamics by generating renderable code rather than directly predicting pixels.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.07131)

- **MobileDreamer: Generative Sketch World Model for GUI Agent**
  - Publication: arXiv 2026 
  - Highlights: A lightweight world model that predicts task-relevant text sketches rather than full screenshots.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.04721)

---

## 📊 Datasets & Benchmarks

### 8.1 General World Modeling

| Dataset/Benchmark Name | Year | Scale | Core Tasks | Link |
|---|---|---|---|---|
| **Omni-WorldBench** | 2026 | 18 representative world models | Comprehensive interaction-centric evaluation for 4D world models | [arXiv](https://arxiv.org/abs/2603.22212) |
| **AgentWorldBench** | 2026 | 5 frontier models, 9 benchmarks | Comprehensive benchmark for language world models | [arXiv](https://arxiv.org/abs/2606.24597) |
| **iWorld-Bench** | 2026 | 330k video clips, 4.9k test samples | Interactive world model evaluation | [arXiv](https://arxiv.org/abs/2605.03941) |
| **WorldModelBench** | 2025 | Video generation models | World model evaluation | [arXiv](https://arxiv.org/abs/2502.20694) |
| **WorldArena** | 2025 | Embodied world models | Perception & functional utility | [arXiv](https://arxiv.org/abs/2509.12345) |
| **MemoBench** | 2026 | 360 ground-truth videos | "Disappear-reappear" world modeling evaluation | [arXiv](https://arxiv.org/abs/2606.27537) |
| **Chess-World-Model** | 2026 | 10.1 million chess games | Precise state tracking benchmark | [arXiv](https://arxiv.org/abs/2605.30100) |

### 8.2 Physics & Causality

| Dataset/Benchmark Name | Year | Scale | Core Tasks | Link |
|---|---|---|---|---|
| **A Physics-Grounded Benchmark for Multi-Agent Dynamics in World Models** | 2026 | Multi-agent dynamics | Physics-grounded multi-agent dynamics benchmark | [arXiv](https://arxiv.org/abs/2606.28757) |
| **CausalARC** | 2026 | Causal reasoning tasks | Abstract reasoning with causal world models | [arXiv](https://arxiv.org/abs/2603.17421) |

### 8.3 Domain-Specific Benchmarks

#### Robotics

| Dataset/Benchmark Name | Year | Scale | Core Tasks | Link |
|---|---|---|---|---|
| **ContactWorld** | 2026 | 12 contact-rich tasks | Vision-tactile world models for contact-rich manipulation | [arXiv](https://arxiv.org/abs/2606.13877) |
| **RoboWM-Bench** | 2026 | Robotic manipulation | Embodied evaluation for video world models | [Semantic Scholar](https://www.semanticscholar.org) |

#### Autonomous Driving

| Dataset/Benchmark Name | Year | Scale | Core Tasks | Link |
|---|---|---|---|---|
| **ReactSim-Bench** | 2026 | 2,636 test scenarios | Reactive behavior world model simulation in autonomous driving | [arXiv](https://arxiv.org/abs/2606.14058) |
| **DrivingWorld** | 2024 | 40+ sec video | Autonomous driving world model | [arXiv](https://arxiv.org/abs/2412.19505) |
| **InfinityDrive** | 2024 | Minute-scale | Driving world model | [arXiv](https://arxiv.org/abs/2412.01234) |

#### Web/GUI Agents

| Dataset/Benchmark Name | Year | Scale | Core Tasks | Link |
|---|---|---|---|---|
| **WebWorld** | 2026 | 1M+ web interactions | Large-scale world model for web agent training | [arXiv](https://arxiv.org/abs/2602.14721) |

---

## ⚙️ Training & Inference Techniques

### 9.1 Memory Mechanisms

- **DiM-WAM: Diverse Historical Event Memory**
  - Publication: arXiv 2026 
  - Highlights: Uses bank-conditioned candidate features, novelty-aware selection, and accumulated-mass-weighted fusion to retain complementary event tokens in bounded memory for WAMs.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.27677)

- **Current World Models Lack a Persistent State Core**
  - Publication: arXiv 2026 
  - Highlights: Argues that current world models lack a persistent state core—generators must maintain a continuously evolving world state rather than rendering plausible frames only at observation time.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.20545)

- **Latent Spatial Memory for Video World Models**
  - Publication: arXiv 2026 
  - Highlights: Stores persistent 3D scene content directly as latent tokens, avoiding repeated RGB rendering and re-encoding.
  - Paper Link: [GitHub](https://github.com/microsoft/LatentSpatialMemory)

### 9.3 Efficient & Real-Time Inference

- **Flash-WAM: Modality-Aware Distillation for World Action Models**
  - Publication: arXiv 2026 
  - Highlights: Compresses WAM inference to a single step per modality, achieving 348× speedup on RoboTwin 2.0 (from seconds to 8.1 ms per chunk).
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.05254)

- **WorldCache: Accelerating World Models for Free via Heterogeneous Token Caching**
  - Publication: arXiv 2026 
  - Highlights: A caching framework tailored to diffusion world models delivering up to 3.7× end-to-end speedups while maintaining 98% rollout quality. Accepted by ICML 2026.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.06331)

- **DISK: Dynamic Inference SKipping for World Models**
  - Publication: arXiv 2026 
  - Highlights: A training-free adaptive inference method for autoregressive world models that coordinates two coupled diffusion transformers for video and ego-trajectory via dual-branch controllers.
  - Paper Link: [arXiv](https://arxiv.org/abs/2601.20436)

- **Planning in 8 Tokens: A Compact Discrete Tokenizer for Latent World Model (CompACT)**
  - Publication: arXiv 2026 
  - Highlights: A discrete tokenizer that compresses each observation to only 8 tokens.
  - Paper Link: [arXiv](https://arxiv.org/abs/2603.03182)

---

## 🔬 Theory & Interpretability

- **Grounding Spatial Relations in a Compact World Model: Instruction Leakage and a Goal-Free Dynamics Fix**
  - Publication: arXiv 2026 
  - Highlights: Identifies the "instruction leakage" problem in goal-conditioned world models and proposes keeping goals outside the dynamics as a fix.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.06925)

- **From Kepler to Newton: Inductive Biases Guide Learned World Models in Transformers**
  - Publication: arXiv 2026 
  - Highlights: Shows how inductive biases guide transformers to learn world models, analogous to the progression from Kepler to Newton.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.06923)

- **Critique of World Model**
  - Publication: arXiv 2026 
  - Highlights: A critical examination of world models, emphasizing that world models are essentially simulators rather than visual content generators.
  - Paper Link: [arXiv](https://arxiv.org/abs/2606.11370)

- **Research on World Models Is Not Merely Injecting World Knowledge into Specific Tasks**
  - Publication: arXiv 2026 
  - Highlights: Argues that robust world models should not be loose collections of capabilities but a normative framework integrating interaction, perception, symbolic reasoning, and spatial representation.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.02371)

- **GeoWorld: Geometric World Models**
  - Publication: arXiv 2026 
  - Highlights: An energy-based predictive world model that achieves multi-step visual planning by reasoning over latent energy landscapes rather than generating pixels.
  - Paper Link: [arXiv](https://arxiv.org/abs/2602.19231)

- **Why We Need World Models for AGI: Where LLMs Fail and How World Models May Outperform**
  - Publication: arXiv 2026 
  - Highlights: Argues that world models operate on latent environment states rather than observation sequences, making causal prediction, simulation, and planning structurally more natural.
  - Paper Link: [arXiv](https://arxiv.org/abs/2605.10191)

- **Agentic World Modeling: Foundations, Capabilities, Laws, and Beyond**
  - Publication: arXiv 2026 
  - Highlights: Connects previously isolated communities, charting a path from passive next-step prediction to world models capable of simulating and ultimately reshaping the environments in which agents operate.
  - Paper Link: [arXiv](https://arxiv.org/abs/2604.19903)

- **Path-Measure Dynamics of Attention-Driven World Models: A Nonlocal Onsager–Machlup Approach**
  - Publication: arXiv 2026 
  - Highlights: Studies path-measure dynamics of attention-driven world models, investigating how attention enables world models to condition on entire histories for long-term memory.
  - Paper Link: [arXiv](https://arxiv.org/abs/2607.01827)

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
- **Verifiability** — In systems that cannot fail (power, thermal, process control), the biggest obstacle to deploying world models is verifiability rather than prediction fidelity.


---

## ❤️ Contact
If you have suggestions for new papers or datasets, spot any inaccuracies, or find this curated resource list helpful, feel free to reach out to Yuanliang Sun via email at sun254667307@gmail.com.
For inquiries about research internship opportunities in world models, you are welcome to contact me at any time.


## 📄 License
CC0 1.0 Universal. Full terms available in the `LICENSE` file of this repository.
