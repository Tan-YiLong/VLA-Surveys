# :sunglasses: Autonomous Driving Decision-Making Across Paradigms

This repository summarizes the methods, datasets, benchmarks, and related surveys mentioned in our survey **"Autonomous Driving Decision-Making Across Paradigms: A Survey of Reasoning, Action, Simulation, and Generation"** :fire:.

The survey organizes autonomous driving decision-making into five paradigms: **LLM/VLM-based driving agents**, **Vision-Action (VA) models**, **Vision-Language-Action (VLA) models**, **Driving World Models (DWMs)**, and **Diffusion-Based Planning Models (DBPMs)**.

Any problems, please contact tanyilong@csuft.edu.cn. Interesting papers or codes are welcome. If this repository is useful to your research or work, it is really appreciated to star this repository :heart:

## Foundation Models Used in Autonomous Driving

### Autonomous-Driving-Specialized Models

| Model | Paradigm | Main Role | Link |
|:-:|:-:|:-|:-:|
| `DiLu` | LLM Agent | Knowledge-driven driving reasoning | [Paper](https://arxiv.org/abs/2309.16292) |
| `Agent-Driver` | LLM Agent | Language-agent planning | [Paper](https://arxiv.org/abs/2311.10813) |
| `DriveGPT4` | LLM/VLM Agent | Interpretable driving reasoning and planning | [Paper](https://arxiv.org/abs/2310.01412) / [Project](https://tonyxuqaq.github.io/projects/DriveGPT4/) |
| `Dolphins` | VLM Agent | Multimodal driving understanding | [Paper](https://arxiv.org/abs/2312.00432) / [Project](https://vlm-driver.github.io/) |
| `DriveMLM` | MLLM Agent | Behavior-state aligned planning | [Paper](https://arxiv.org/abs/2312.09245) |
| `LMDrive` | VLA | Closed-loop language-conditioned driving | [Paper](https://arxiv.org/abs/2312.07488) |
| `DriveVLM` | VLA | Large VLM-based end-to-end driving | [Paper](https://arxiv.org/abs/2402.12289) / [Project](https://tsinghua-mars-lab.github.io/DriveVLM/) / [GitHub](https://github.com/hanker-zhu/DriveVLM-project) |
| `RDA-Driver` | LLM/VLM Agent | Reasoning-decision alignment | [Paper](https://arxiv.org/abs/2409.07246) |
| `VLAAD` | VLM Assistant | Vision-language driving assistance | [GitHub](https://github.com/sungyeonparkk/vision-assistant-for-driving) |
| `WiseAD` | VLM/VLA | Knowledge-augmented end-to-end driving | [Paper](https://arxiv.org/abs/2412.09644) / [Project](https://wyddmw.github.io/WiseAD_demo/) / [GitHub](https://github.com/wyddmw/WiseAD) |
| `OpenEMMA` | VLM/VLA-style E2E | Open-source multimodal planning | [Paper](https://arxiv.org/abs/2412.15208) / [GitHub](https://github.com/taco-group/OpenEMMA) |
| `EMMA` | Multimodal E2E | End-to-end multimodal driving model | [Paper](https://arxiv.org/abs/2410.23262) |
| `ORION` | VLA | Vision-language instructed action generation | [Paper](https://arxiv.org/abs/2503.19755) / [GitHub](https://github.com/xiaomi-mlab/Orion) |
| `AlphaDrive` | VLA/RL | Reinforcement learning and reasoning | [Paper](https://arxiv.org/abs/2503.07608) / [GitHub](https://github.com/hustvl/AlphaDrive) |
| `OpenDriveVLA` | VLA | Open large VLA for end-to-end driving | [Paper](https://arxiv.org/abs/2503.23463) / [Project](https://drivevla.github.io/) / [GitHub](https://github.com/DriveVLA/OpenDriveVLA) |
| `AutoVLA` | VLA/RL | Adaptive reasoning and action tokenization | [Paper](https://arxiv.org/abs/2506.13757) / [Project](https://autovla.github.io/) / [GitHub](https://github.com/ucla-mobility/AutoVLA) |
| `Drive-R1` | VLA/RL | Reasoning-planning bridge for VLM driving | [Paper](https://arxiv.org/abs/2506.18234) |
| `DriveAgent-R1` | VLM Agent | Active perception and hybrid thinking | [OpenReview](https://openreview.net/forum?id=r2g8TV4nJy) / [ICLR](https://iclr.cc/virtual/2026/poster/10007182) |
| `OmniReason` | VLA | Temporal-guided action reasoning | [Paper](https://arxiv.org/abs/2509.00789) |
| `OpenREAD` | VLA/RL | Open-ended reasoning with LLM-as-critic | [Paper](https://arxiv.org/abs/2512.01830) |
| `Reasoning-VLA` | VLA | Fast general action reasoning | [Paper](https://arxiv.org/abs/2511.19912) / [HF Paper](https://huggingface.co/papers/2511.19912) |
| `MindDrive` | VLA/RL | Online RL with language-as-action | [Paper](https://arxiv.org/abs/2512.13636) / [Project](https://xiaomi-mlab.github.io/MindDrive/) / [GitHub](https://github.com/xiaomi-mlab/MindDrive) |
| `DynVLA` | VLA/World Dynamics | Dynamics-aware action reasoning | [Project](https://yaoyao-jpg.github.io/dynvla/) |
| `VLAWorld` | VLA World Model | Vision-language-action world modeling | [Project](https://vlaworld.github.io/) |

### Open Vision-Language and Multimodal Backbones

| Model | Provider | Main Role in AD | Link |
|:-:|:-:|:-|:-:|
| `Qwen-VL` | Alibaba | Early open VLM backbone | [Link](https://huggingface.co/Qwen/Qwen-VL) |
| `Qwen2-VL` | Alibaba | Multimodal perception and VQA | [Link](https://qwenlm.github.io/blog/qwen2-vl/) |
| `Qwen2.5-VL` | Alibaba | Strong VLM backbone for driving agents and VLA | [Link](https://qwenlm.github.io/blog/qwen2.5-vl/) |
| `Qwen2.5-VL-32B` | Alibaba | Larger VLM reasoning backbone | [Link](https://qwenlm.github.io/blog/qwen2.5-vl-32b/) |
| `DeepSeek-VL` | DeepSeek | Vision-language understanding | [Link](https://huggingface.co/collections/deepseek-ai/deepseek-vl-65f295948133d9cf92b706d3) |
| `InternVL2` | OpenGVLab | Open multimodal driving perception backbone | [Link](https://github.com/OpenGVLab/InternVL) |
| `InternVL3` | OpenGVLab | Advanced open VLM backbone | [Link](https://github.com/OpenGVLab/InternVL) |
| `InternVL3.5` | OpenGVLab | Multimodal reasoning and embodied-agent backbone | [Link](https://internvl.github.io/blog/2025-08-26-InternVL-3.5/) / [GitHub](https://github.com/OpenGVLab/InternVL) |
| `LLaVA-1.5` | LLaVA | VLM baseline for driving QA and reasoning | [Link](https://github.com/haotian-liu/LLaVA) |
| `LLaVA-NeXT` | LLaVA | Higher-resolution VLM reasoning | [Link](https://github.com/LLaVA-VL/LLaVA-NeXT) |
| `LLaVA-OneVision` | LLaVA | Image-video-language backbone | [Link](https://github.com/LLaVA-VL/LLaVA-NeXT) |
| `Yi-VL` | 01-ai | Bilingual VLM backbone | [Link](https://huggingface.co/collections/01-ai/yi-vl-663f557228538eae745769f3) |
| `CogVLM2` | Zhipu AI / THUDM | Vision-language reasoning backbone | [Link](https://huggingface.co/collections/THUDM/cogvlm2-6645f36a29948b67dc4eef75) |
| `MiniCPM-V` | OpenBMB | Lightweight edge-friendly VLM | [Link](https://github.com/OpenBMB/MiniCPM-V) |
| `Phi-4-multimodal` | Microsoft | Lightweight multimodal reasoning | [Link](https://huggingface.co/microsoft/Phi-4-multimodal-instruct) |
| `Gemma 3` | Google | Open multimodal model for text-image reasoning | [Link](https://blog.google/technology/developers/gemma-3/) |
| `Llama 3.2 Vision` | Meta | Open vision-language backbone | [Link](https://llama.meta.com/) |
| `Pixtral 12B` | Mistral AI | Open multimodal model | [Link](https://mistral.ai/news/pixtral-12b) |
| `Pixtral Large` | Mistral AI | Larger multimodal model | [Link](https://legal.mistral.ai/ai-governance/models/pixtral-large) |

### Open Language and Reasoning Backbones

| Model | Provider | Main Role in AD | Link |
|:-:|:-:|:-|:-:|
| `Qwen3` | Alibaba | Reasoning, tool use, agentic planning | [Link](https://qwenlm.github.io/blog/qwen3/) |
| `Qwen2.5` | Alibaba | General LLM backbone | [Link](https://qwenlm.github.io/blog/qwen2.5/) |
| `Qwen2.5-Coder` | Alibaba | Code/tool-using driving agents | [Link](https://qwenlm.github.io/blog/qwen2.5-coder/) |
| `DeepSeek-R1` | DeepSeek | Reasoning-heavy driving agents | [Link](https://github.com/deepseek-ai/DeepSeek-R1) |
| `DeepSeek-V3.1` | DeepSeek | Hybrid thinking and tool calling | [Link](https://huggingface.co/deepseek-ai/DeepSeek-V3.1) |
| `Llama 3.1` | Meta | General open LLM backbone | [Link](https://llama.meta.com/) |
| `Llama 3.3` | Meta | Stronger open LLM backbone | [Link](https://llama.meta.com/) |
| `Mistral 7B` | Mistral AI | Efficient LLM baseline | [Link](https://mistral.ai/news/announcing-mistral-7b/) |
| `Mixtral-8x7B` | Mistral AI | Sparse MoE reasoning baseline | [Link](https://mistral.ai/news/mixtral-of-experts/) |
| `Mixtral-8x22B` | Mistral AI | Larger sparse MoE backbone | [Link](https://mistral.ai/news/mixtral-8x22b/) |
| `Codestral` | Mistral AI | Code and tool-use backbone | [Link](https://mistral.ai/news/codestral/) |
| `Phi-4-mini-reasoning` | Microsoft | Small reasoning backbone | [Link](https://huggingface.co/microsoft) |
| `InternLM2` | Shanghai AI Laboratory | General open LLM backbone | [Link](https://huggingface.co/collections/internlm/internlm2-65b0ce04970888799707893c) |
| `GLM-4` | Zhipu AI | General and tool-using LLM backbone | [Link](https://github.com/THUDM/GLM-4) |
| `Yi-1.5` | 01-ai | General bilingual LLM backbone | [Link](https://huggingface.co/collections/01-ai/yi-15-2024-05-663f3ecab5f815a3eaca7ca8) |
| `OLMo` | AllenAI | Fully open research LLM | [Link](https://huggingface.co/collections/allenai/olmo-suite-65aeaae8fe5b6b2122b46778) |

### Closed-Source Models Commonly Used as Strong Baselines

| Model | Provider | Main Role in AD | Link |
|:-:|:-:|:-|:-:|
| `GPT-5.2` | OpenAI | Frontier multimodal/reasoning baseline | [Link](https://platform.openai.com/docs/models) |
| `GPT-5.1` | OpenAI | Coding, reasoning, and agentic baseline | [Link](https://platform.openai.com/docs/models/gpt) |
| `GPT-4.1` | OpenAI | Non-reasoning VLM/agent baseline | [Link](https://platform.openai.com/docs/models) |
| `Claude Opus 4.1` | Anthropic | Strong reasoning and image-input baseline | [Link](https://docs.anthropic.com/en/docs/about-claude/models/all-models) |
| `Claude Sonnet 4` | Anthropic | Efficient reasoning and multimodal baseline | [Link](https://docs.anthropic.com/en/docs/models-overview) |
| `Gemini 2.5 Pro` | Google | Multimodal reasoning over image/video/code | [Link](https://cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/2-5-pro) |
| `Gemini 2.5 Flash` | Google | Efficient multimodal reasoning baseline | [Link](https://cloud.google.com/vertex-ai/generative-ai/docs/models/gemini) |
| `Grok 4` | xAI | Closed multimodal/reasoning baseline | [Link](https://docs.oracle.com/en-us/iaas/Content/generative-ai/xai-grok-4.htm) |
| `Mistral Large` | Mistral AI | Closed/API LLM baseline | [Link](https://www.aboutamazon.com/news/aws/mistral-ai-mistral-large-amazon-bedrock) |
| `Pixtral Large` | Mistral AI | Closed/API multimodal baseline | [Link](https://www.aboutamazon.com/news/aws/aws-mistral-ai-pixtral-large) |


## Contents

- [1. LLM/VLM-Based Driving Agents](#1-llmvlm-based-driving-agents)
- [2. Vision-Action Models](#2-vision-action-models)
- [3. Vision-Language-Action Models](#3-vision-language-action-models)
- [4. Driving World Models](#4-driving-world-models)
- [5. Diffusion-Based Planners](#5-diffusion-based-planners)
- [6. Datasets and Benchmarks](#6-datasets-and-benchmarks)

---


## 1. LLM/VLM-Based Driving Agents

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
| `PRAM-R` | [PRAM-R: A Perception-Reasoning-Action-Memory Framework with LLM-Guided Modality Routing for Adaptive Autonomous Driving](https://arxiv.org/abs/2603.04222) | arXiv 2026 | - | - |
| `Vlm-mpc` | [VLM-MPC: Model Predictive Controller Augmented Vision Language Model for Autonomous Driving](https://arxiv.org/abs/2603.04222) | Transportation Research Part C 2026 | - | - |
| `LaMPilot` | [LaMPilot: An Open Benchmark Dataset for Autonomous Driving with Language Model Programs](https://arxiv.org/abs/2405.15158) | CVPR 2024 | - | [![GitHub](https://img.shields.io/github/stars/PurdueDigitalTwin/LaMPilot)](https://github.com/PurdueDigitalTwin/LaMPilot) |
| `DiLu` | [DiLu: A Knowledge-Driven Approach to Autonomous Driving with Large Language Models](https://arxiv.org/abs/2309.16292) | arXiv 2023 | - | - |
| `Agent-Driver` | [A Language Agent for Autonomous Driving](https://arxiv.org/abs/2311.10813) | COLM 2023 | - | - |
| `DriveAgent` | [DriveAgent: Multi-Agent Structured Reasoning with LLM and Multimodal Sensor Fusion for Autonomous Driving](https://arxiv.org/abs/2501.03230) | IEEE RA-L 2025 | - | - |
| `LLM-ASSIST` | [LLM-ASSIST: Enhancing Closed-Loop Planning with Language-Based Reasoning](https://arxiv.org/abs/2401.00125) | arXiv 2023 | - | - |
| `DriveCoT` | [DriveCoT: Integrating Chain-of-Thought Reasoning with End-to-End Driving](https://arxiv.org/abs/2403.16996) | arXiv 2024 | - | - |
| `DriveGPT4` | [DriveGPT4: Interpretable End-to-End Autonomous Driving via Large Language Model](https://arxiv.org/abs/2310.01412) | IEEE RA-L 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://tonyxuqaq.github.io/projects/DriveGPT4/) | - |
| `Dolphins` | [Dolphins: Multimodal Language Model for Driving](https://arxiv.org/abs/2312.00432) | ECCV 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://vlm-driver.github.io/) | - |
| `OmniDrive-R1` | [OmniDrive-R1: Reinforcement-driven Interleaved Multi-modal Chain-of-Thought for Trustworthy Vision-Language Autonomous Driving](https://arxiv.org/abs/2512.14044) | arXiv 2025 | - | - |
| `ELM` | [ELM: Embodied Understanding of Driving Scenarios](https://arxiv.org/abs/2311.16777) | ECCV 2024 | - | - |
| `LangCoop` | [LangCoop: Collaborative Driving with Language](https://arxiv.org/abs/2504.13406) | CVPR 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://xiangbogaobarry.github.io/LangCoop/) | [![GitHub](https://img.shields.io/github/stars/taco-group/LangCoop)](https://github.com/taco-group/LangCoop) |
| `V2V-LLM` | [V2V-LLM: Vehicle-to-Vehicle Cooperative Autonomous Driving with Multi-Modal Large Language Models](https://arxiv.org/abs/2502.09980) | arXiv 2025 | - | - |
| `DriveMLM` | [DriveMLM: Aligning Multi-Modal Large Language Models with Behavioral Planning States for Autonomous Driving](https://arxiv.org/abs/2312.09245) | Visual Intelligence 2025 | - | - |
| `RDA-Driver` | [RDA-Driver: Making Large Language Models Better Planners with Reasoning-Decision Alignment](https://arxiv.org/abs/2409.07246) | ECCV 2024 | - | - |
| `DriVLMe` | [DriVLMe: Enhancing LLM-based Autonomous Driving Agents with Embodied and Social Experiences](https://arxiv.org/abs/2409.07246) | IROS 2024 | - | - |
| `LLaDA` | [LLaDA: Driving Everywhere with Large Language Model Policy Adaptation](https://arxiv.org/abs/2409.07246) | CVPR 2024 | - | - |
| `VLAAD` | [VLAAD: Vision and Language Assistant for Autonomous Driving](https://arxiv.org/abs/2312.00432) | WACV 2024 | - | [![GitHub](https://img.shields.io/github/stars/sungyeonparkk/vision-assistant-for-driving)](https://github.com/sungyeonparkk/vision-assistant-for-driving) |
| `WKER` | [WKER: World Knowledge-Enhanced Reasoning Using Instruction-Guided Interactor in Autonomous Driving](https://arxiv.org/abs/2501.03230) | AAAI 2025 | - | - |
| `S4-Driver` | [S4-Driver: Scalable Self-Supervised Driving Multimodal Large Language Model with Spatio-Temporal Visual Representation](https://arxiv.org/abs/2501.03230) | CVPR 2025 | - | - |
| `Occ-LLM` | [Occ-LLM: Enhancing Autonomous Driving with Occupancy-based Large Language Models](https://arxiv.org/abs/2501.03230) | ICRA 2025 | - | - |
| `FutureSightDrive` | [FutureSightDrive: Thinking Visually with Spatio-Temporal CoT for Autonomous Driving](https://arxiv.org/abs/2505.17685) | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://miv-xjtu.github.io/FSDrive.github.io/) | [![GitHub](https://img.shields.io/github/stars/MIV-XJTU/FSDrive)](https://github.com/MIV-XJTU/FSDrive) |
| `WiseAD` | [WiseAD: Knowledge Augmented End-to-End Autonomous Driving with Vision-Language Model](https://arxiv.org/abs/2412.09644) | arXiv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://wyddmw.github.io/WiseAD_demo/) | [![GitHub](https://img.shields.io/github/stars/wyddmw/WiseAD)](https://github.com/wyddmw/WiseAD) |
| `VLP` | [VLP: Vision Language Planning for Autonomous Driving](https://arxiv.org/abs/2401.05577) | CVPR 2024 | - | - |
| `ALN-P3` | [ALN-P3: Unified Language Alignment for Perception, Prediction, and Planning in Autonomous Driving](https://arxiv.org/abs/2505.15158) | arXiv 2025 | - | - |
| `VERDI` | [VERDI: VLM-Embedded Reasoning for Autonomous Driving](https://arxiv.org/abs/2505.15925) | arXiv 2025 | - | - |
| `3R` | [3R: Receive, Reason, and React: Drive as You Say, with Large Language Models in Autonomous Vehicles](https://arxiv.org/abs/2409.07246) | IEEE ITSM 2024 | - | - |
| `LMAD` | [LMAD: Integrated End-to-End Vision-Language Model for Explainable Autonomous Driving](https://arxiv.org/abs/2508.12404) | arXiv 2025 | - | - |

---

## 2. Vision-Action Models

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
| `LBC` | [Learning by Cheating](https://arxiv.org/abs/1912.12294) | CoRL 2020 | - | [![GitHub](https://img.shields.io/github/stars/bradyz/2020_CARLA_challenge)](https://github.com/bradyz/2020_CARLA_challenge) |
| `Latent-DRL` | [End-to-End Model-Free Reinforcement Learning for Urban Driving using Implicit Affordances](https://arxiv.org/abs/2006.08126) | CVPR 2020 | - | - |
| `NEAT` | [NEAT: Neural Attention Fields for End-to-End Autonomous Driving](https://arxiv.org/abs/2109.04456) | ICCV 2021 | - | [![GitHub](https://img.shields.io/github/stars/autonomousvision/neat)](https://github.com/autonomousvision/neat) |
| `Roach` | [End-to-End Urban Driving by Imitating a Reinforcement Learning Coach](https://arxiv.org/abs/2108.08265) | ICCV 2021 | - | [![GitHub](https://img.shields.io/github/stars/zhejz/carla-roach)](https://github.com/zhejz/carla-roach) |
| `WoR` | [Learning to Drive from a World on Rails](https://arxiv.org/abs/2105.00636) | ICCV 2021 | - | - |
| `Urban-Driver` | [Urban Driver: Learning to Drive from Real-World Demonstrations using Policy Gradients](https://arxiv.org/abs/2109.13333) | CoRL 2022 | - | - |
| `TCP` | [Trajectory-Guided Control Prediction for End-to-End Autonomous Driving: A Simple yet Strong Baseline](https://arxiv.org/abs/2206.08129) | NeurIPS 2022 | - | [![GitHub](https://img.shields.io/github/stars/OpenDriveLab/TCP)](https://github.com/OpenDriveLab/TCP) |
| `LAV` | [Learning from All Vehicles](https://arxiv.org/abs/2202.02605) | CVPR 2022 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://dotchen.github.io/LAV/) | [![GitHub](https://img.shields.io/github/stars/dotchen/LAV)](https://github.com/dotchen/LAV) |
| `TransFuser` | [TransFuser: Imitation with Transformer-Based Sensor Fusion for Autonomous Driving](https://arxiv.org/abs/2205.15997) | IEEE TPAMI 2022 | - | [![GitHub](https://img.shields.io/github/stars/autonomousvision/transfuser)](https://github.com/autonomousvision/transfuser) |
| `GRI` | [GRI: General Reinforced Imitation and Its Application to Vision-Based Autonomous Driving](https://www.mdpi.com/2218-6581/12/5/127) | Robotics 2023 | - | - |
| `BEVPlanner` | [Is Ego Status All You Need for Open-Loop End-to-End Autonomous Driving?](https://arxiv.org/abs/2312.03031) | CVPR 2024 | - | [![GitHub](https://img.shields.io/github/stars/NVlabs/BEV-Planner)](https://github.com/NVlabs/BEV-Planner) |
| `RAD` | [RAD: Training an End-to-End Driving Policy via Large-Scale 3DGS-Based Reinforcement Learning](https://arxiv.org/abs/2502.13144) | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://hgao-cv.github.io/RAD) | - |
| `ST-P3` | [ST-P3: End-to-End Vision-Based Autonomous Driving via Spatial-Temporal Feature Learning](https://arxiv.org/abs/2207.07601) | ECCV 2022 | - | [![GitHub](https://img.shields.io/github/stars/OpenDriveLab/ST-P3)](https://github.com/OpenDriveLab/ST-P3) |
| `UniAD` | [Planning-Oriented Autonomous Driving](https://arxiv.org/abs/2212.10156) | CVPR 2023 | - | [![GitHub](https://img.shields.io/github/stars/OpenDriveLab/UniAD)](https://github.com/OpenDriveLab/UniAD) |
| `VAD` | [VAD: Vectorized Scene Representation for Efficient Autonomous Driving](https://arxiv.org/abs/2303.12077) | ICCV 2023 | - | [![GitHub](https://img.shields.io/github/stars/hustvl/VAD)](https://github.com/hustvl/VAD) |
| `OccNet` | [Scene as Occupancy](https://arxiv.org/abs/2306.09242) | ICCV 2023 | - | [![GitHub](https://img.shields.io/github/stars/OpenDriveLab/OccNet)](https://github.com/OpenDriveLab/OccNet) |
| `Hydra-MDP` | [Hydra-MDP: End-to-End Multimodal Planning with Multi-Target Hydra-Distillation](https://arxiv.org/abs/2406.06978) | arXiv 2024 | - | - |
| `SparseAD` | [SparseAD: Sparse Query-Centric Paradigm for Efficient End-to-End Autonomous Driving](https://arxiv.org/abs/2404.06892) | arXiv 2024 | - | - |
| `GaussianAD` | [GaussianAD: Gaussian-Centric End-to-End Autonomous Driving](https://arxiv.org/abs/2412.10371) | arXiv 2024 | - | - |
| `DiFSD` | [DiFSD: Ego-Centric Fully Sparse Paradigm with Uncertainty Denoising and Iterative Refinement for Efficient End-to-End Self-Driving](https://arxiv.org/abs/2409.09777) | arXiv 2024 | - | - |
| `DriveTransformer` | [DriveTransformer: Unified Transformer for Scalable End-to-End Autonomous Driving](https://arxiv.org/abs/2503.07656) | ICLR 2025 | - | [![GitHub](https://img.shields.io/github/stars/Thinklab-SJTU/DriveTransformer)](https://github.com/Thinklab-SJTU/DriveTransformer) |
| `SparseDrive` | [SparseDrive: End-to-End Autonomous Driving via Sparse Scene Representation](https://arxiv.org/abs/2405.19620) | ICRA 2025 | - | [![GitHub](https://img.shields.io/github/stars/swc-17/SparseDrive)](https://github.com/swc-17/SparseDrive) |
| `ETA` | [ETA: Efficiency through Thinking Ahead, A Dual Approach to Self-Driving with Large Models](https://arxiv.org/abs/2506.07725) | ICCV 2025 | - | [![GitHub](https://img.shields.io/github/stars/OpenDriveLab/ETA)](https://github.com/OpenDriveLab/ETA) |
| `Geo` | [Spatial Retrieval Augmented Autonomous Driving](https://arxiv.org/abs/2503.09517) | arXiv 2025 | - | - |
| `NaviHydra` | [NaviHydra: Controllable Navigation-Guided End-to-End Autonomous Driving with Hydra-Distillation](https://arxiv.org/abs/2512.10660) | arXiv 2025 | - | - |


## 3. Vision-Language-Action Models

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
| `AutoVLA` | [AutoVLA: A Vision-Language-Action Model for End-to-End Autonomous Driving with Adaptive Reasoning and Reinforcement Fine-Tuning](https://arxiv.org/abs/2506.13757) | NeurIPS 2025 | - | [![GitHub](https://img.shields.io/github/stars/autovla/autovla)](https://github.com/autovla/autovla) |
| `DriveVLM` | [DriveVLM: The Convergence of Autonomous Driving and Large Vision-Language Models](https://arxiv.org/abs/2402.12289) | CoRL 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://tsinghua-mars-lab.github.io/DriveVLM/) | [![GitHub](https://img.shields.io/github/stars/hanker-zhu/DriveVLM-project)](https://github.com/hanker-zhu/DriveVLM-project) |
| `LMDrive` | [LMDrive: Closed-Loop End-to-End Driving with Large Language Models](https://arxiv.org/abs/2312.07488) | CVPR 2024 | - | - |
| `Senna` | [Senna: Bridging Large Vision-Language Models and End-to-End Autonomous Driving](https://arxiv.org/abs/2410.22313) | arXiv 2024 | - | - |
| `Driving-RAG` | [Driving-RAG: Driving Scenarios Embedding, Search, and RAG Applications](https://arxiv.org/abs/2602.06214) | Automotive Innovation 2026 | - | - |
| `OpenDriveVLA` | [OpenDriveVLA: Towards End-to-End Autonomous Driving with Large Vision Language Action Model](https://arxiv.org/abs/2503.23463) | AAAI 2026 | - | [![GitHub](https://img.shields.io/github/stars/DriveVLA/OpenDriveVLA)](https://github.com/DriveVLA/OpenDriveVLA) |
| `DriveMoE` | [DriveMoE: Mixture-of-Experts for Vision-Language-Action Model in End-to-End Autonomous Driving](https://arxiv.org/abs/2505.16278) | arXiv 2025 | - | - |
| `SafeAuto` | [SafeAuto: Knowledge-Enhanced Safe Autonomous Driving with Multimodal Foundation Models](https://arxiv.org/abs/2503.00211) | ICML 2025 | - | - |
| `CoVLA` | [CoVLA: Comprehensive Vision-Language-Action Dataset for Autonomous Driving](https://arxiv.org/abs/2408.10845) | WACV 2025 | - | - |
| `SpaceDrive` | [SpaceDrive: Infusing Spatial Awareness into VLM-based Autonomous Driving](https://arxiv.org/abs/2512.10719) | arXiv 2025 | - | - |
| `PARA-Drive` | [PARA-Drive: Parallelized Architecture for Real-Time Autonomous Driving](https://arxiv.org/abs/2409.07246) | CVPR 2024 | - | - |
| `DiffVLA` | [DiffVLA: Vision-Language Guided Diffusion Planning for Autonomous Driving](https://arxiv.org/abs/2505.19381) | arXiv 2025 | - | - |
| `ORION` | [ORION: A Holistic End-to-End Autonomous Driving Framework by Vision-Language Instructed Action Generation](https://arxiv.org/abs/2503.19755) | ICCV 2025 | - | [![GitHub](https://img.shields.io/github/stars/xiaomi-mlab/Orion)](https://github.com/xiaomi-mlab/Orion) |
| `Drive-R1` | [Drive-R1: Bridging Reasoning and Planning in VLMs for Autonomous Driving with Reinforcement Learning](https://arxiv.org/abs/2506.18234) | AAAI 2026 | - | - |
| `Alpamayo-R1` | [Alpamayo-R1: Bridging Reasoning and Action Prediction for Generalizable Autonomous Driving in the Long Tail](https://arxiv.org/abs/2511.00088) | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/NVlabs/alpamayo)](https://github.com/NVlabs/alpamayo) |
| `DynVLA` | [DynVLA: Learning World Dynamics for Action Reasoning in Autonomous Driving](https://arxiv.org/abs/2603.11041) | arXiv 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://yaoyao-jpg.github.io/dynvla/) | - |
| `AdaThinkDrive` | [AdaThinkDrive: Adaptive Thinking via Reinforcement Learning for Autonomous Driving](https://arxiv.org/abs/2509.13769) | arXiv 2025 | - | - |
| `ReasonPlan` | [ReasonPlan: Unified Scene Prediction and Decision Reasoning for Closed-loop Autonomous Driving](https://arxiv.org/abs/2501.03230) | CoRL 2025 | - | - |
| `ImpromptuVLA` | [ImpromptuVLA: Open Weights and Open Data for Driving Vision-Language-Action Models](https://arxiv.org/abs/2501.03230) | NeurIPS D&B 2025 | - | - |
| `Sce2DriveX` | [Sce2DriveX: A Generalized MLLM Framework for Scene-to-Drive Learning](https://arxiv.org/abs/2501.03230) | IEEE RA-L 2025 | - | - |
| `EMMA` | [EMMA: End-to-End Multimodal Model for Autonomous Driving](https://arxiv.org/abs/2410.23262) | TMLR 2024 | - | - |
| `DriveAgent-R1` | [DriveAgent-R1: Advancing VLM-based Autonomous Driving with Active Perception and Hybrid Thinking](https://arxiv.org/abs/2507.20879) | ICLR 2026 | - | [![GitHub](https://img.shields.io/github/stars/Zwc2003/DriveAgent-R1)](https://github.com/Zwc2003/DriveAgent-R1) |
| `FastDriveVLA` | [FastDriveVLA: Efficient End-to-End Driving via Plug-and-Play Reconstruction-based Token Pruning](https://arxiv.org/abs/2501.03230) | AAAI 2026 | - | - |
| `OmniReason` | [OmniReason: A Temporal-Guided Vision-Language-Action Framework for Autonomous Driving](https://arxiv.org/abs/2509.00789) | arXiv 2025 | - | - |
| `OpenREAD` | [OpenREAD: Reinforced Open-Ended Reasoning for End-to-End Autonomous Driving with LLM-as-Critic](https://arxiv.org/abs/2512.01830) | arXiv 2025 | - | - |
| `PLA` | [PLA: A Unified Perception-Language-Action Framework for Adaptive Autonomous Driving](https://arxiv.org/abs/2501.03230) | FLLM 2025 | - | - |
| `AlphaDrive` | [AlphaDrive: Unleashing the Power of VLMs in Autonomous Driving via Reinforcement Learning and Reasoning](https://arxiv.org/abs/2503.07608) | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/hustvl/AlphaDrive)](https://github.com/hustvl/AlphaDrive) |
| `BEVDriver` | [BEVDriver: Leveraging BEV Maps in LLMs for Robust Closed-Loop Driving](https://arxiv.org/abs/2501.03230) | IROS 2025 | - | - |
| `DriveGPT4-V2` | [DriveGPT4-V2: Harnessing Large Language Model Capabilities for Enhanced Closed-Loop Autonomous Driving](https://arxiv.org/abs/2501.03230) | CVPR 2025 | - | - |
| `DSDrive` | [DSDrive: Distilling Large Language Model for Lightweight End-to-End Autonomous Driving with Unified Reasoning and Planning](https://arxiv.org/abs/2505.05360) | arXiv 2025 | - | - |
| `OccVLA` | [OccVLA: Vision-Language-Action Model with Implicit 3D Occupancy Supervision](https://arxiv.org/abs/2509.05578) | arXiv 2025 | - | - |
| `E3AD` | [E3AD: An Emotion-Aware Vision-Language-Action Model for Human-Centric End-to-End Autonomous Driving](https://arxiv.org/abs/2512.04733) | arXiv 2025 | - | - |
| `UniUGP` | [UniUGP: Unifying Understanding, Generation, and Planning for End-to-End Autonomous Driving](https://arxiv.org/abs/2512.09864) | arXiv 2025 | - | - |
| `MindDrive` | [MindDrive: A Vision-Language-Action Model for Autonomous Driving via Online Reinforcement Learning](https://arxiv.org/abs/2512.13636) | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://xiaomi-mlab.github.io/MindDrive/) | [![GitHub](https://img.shields.io/github/stars/xiaomi-mlab/MindDrive)](https://github.com/xiaomi-mlab/MindDrive) |
| `OpenEMMA` | [OpenEMMA: Open-Source Multimodal Model for End-to-End Autonomous Driving](https://arxiv.org/abs/2412.15208) | WACV 2025 | - | [![GitHub](https://img.shields.io/github/stars/taco-group/OpenEMMA)](https://github.com/taco-group/OpenEMMA) |
| `Percept-WAM` | [Percept-WAM: Perception-Enhanced World-Awareness-Action Model for Robust End-to-End Autonomous Driving](https://arxiv.org/abs/2511.19221) | arXiv 2025 | - | - |
| `Reasoning-VLA` | [Reasoning-VLA: A Fast and General Vision-Language-Action Reasoning Model for Autonomous Driving](https://arxiv.org/abs/2511.19912) | arXiv 2025 | - | - |
| `VLM-AD` | [VLM-AD: End-to-End Autonomous Driving through Vision-Language Model Supervision](https://arxiv.org/abs/2501.03230) | CoRL 2025 | - | - |
| `DiMA` | [DiMA: Digging into Multigranular Archetype for Fine-Grained Object Detection](https://arxiv.org/abs/2501.03230) | IEEE TGRS 2024 | - | - |
| `VLM-E2E` | [VLM-E2E: Enhancing End-to-End Autonomous Driving with Multimodal Driver Attention Fusion](https://arxiv.org/abs/2502.18042) | arXiv 2025 | - | - |
| `SparseOccVLA` | [SparseOccVLA: Bridging Occupancy and Vision-Language Models via Sparse Queries for Unified 4D Scene Understanding and Planning](https://arxiv.org/abs/2601.06474) | arXiv 2026 | - | - |

---

## 4. Driving World Models

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
| `Epona` | [Epona: Autoregressive Diffusion World Model for Autonomous Driving](https://arxiv.org/abs/2506.24113) | ICCV 2025 | - | [![GitHub](https://img.shields.io/github/stars/Kevin-thu/Epona)](https://github.com/Kevin-thu/Epona) |
| `DriveDreamer` | [DriveDreamer: Towards Real-World-Drive World Models for Autonomous Driving](https://arxiv.org/abs/2409.09733) | ECCV 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://drivedreamer-policy.github.io/) | - |
| `DriveDreamer-2` | [DriveDreamer-2: LLM-Enhanced World Models for Diverse Driving Video Generation](https://arxiv.org/abs/2501.03230) | AAAI 2025 | - | - |
| `HERMES` | [HERMES: A Unified Self-Driving World Model for Simultaneous 3D Scene Understanding and Generation](https://arxiv.org/abs/2504.08544) | ICCV 2025 | - | [![GitHub](https://img.shields.io/github/stars/HERMES-AD/HERMES)](https://github.com/HERMES-AD/HERMES) |
| `Vista` | [Vista: A Generalizable Driving World Model with High Fidelity and Versatile Controllability](https://arxiv.org/abs/2405.17398) | NeurIPS 2024 | - | - |
| `DriveScape` | [DriveScape: Towards High-Resolution Controllable Multi-View Driving Video Generation](https://arxiv.org/abs/2409.05463) | arXiv 2024 | - | - |
| `Copilot4D` | [Copilot4D: Learning Unsupervised World Models for Autonomous Driving via Discrete Diffusion](https://arxiv.org/abs/2401.03230) | ICLR 2024 | - | - |
| `OccWorld` | [OccWorld: Learning a 3D Occupancy World Model for Autonomous Driving](https://arxiv.org/abs/2405.03668) | ECCV 2024 | - | [![GitHub](https://img.shields.io/github/stars/wzzheng/OccWorld)](https://github.com/wzzheng/OccWorld) |
| `UnO` | [UnO: Unsupervised Occupancy Fields for Perception and Forecasting](https://arxiv.org/abs/2406.09731) | CVPR 2024 | - | - |
| `GaussianWorld` | [GaussianWorld: Gaussian World Model for Streaming 3D Occupancy Prediction](https://arxiv.org/abs/2412.10373) | CVPR 2025 | - | [![GitHub](https://img.shields.io/github/stars/zuosc19/GaussianWorld)](https://github.com/zuosc19/GaussianWorld) |
| `BEVWorld` | [BEVWorld: A Multimodal World Simulator for Autonomous Driving via Scene-Level BEV Latents](https://arxiv.org/abs/2407.05679) | arXiv 2024 | - | - |
| `VaViM` | [VaViM and VaVAM: Autonomous Driving through Video Generative Modeling](https://arxiv.org/abs/2502.15672) | arXiv 2025 | - | - |
| `GenAD` | [GenAD: Generative End-to-End Autonomous Driving](https://arxiv.org/abs/2409.10830) | ECCV 2024 | - | - |
| `DriveLaW` | [DriveLaW: Unifying Planning and Video Generation in a Latent Driving World](https://arxiv.org/abs/2512.23421) | CVPR 2026 | - | [![GitHub](https://img.shields.io/github/stars/xiaomi-research/drivelaw)](https://github.com/xiaomi-research/drivelaw) |
| `World4Drive` | [World4Drive: End-to-End Autonomous Driving via Intention-aware Physical Latent World Model](https://arxiv.org/abs/2501.03230) | ICCV 2025 | - | [![GitHub](https://img.shields.io/github/stars/ucaszyp/World4Drive)](https://github.com/ucaszyp/World4Drive) |
| `DrivingWorld` | [DrivingWorld: Constructing World Model for Autonomous Driving via Video GPT](https://arxiv.org/abs/2412.19505) | arXiv 2024 | - | - |
| `LMGenDrive` | [LMGenDrive: LLM Reasoning Meets World Models for End-to-End Driving](https://arxiv.org/abs/2501.03230) | ICLR 2026 | - | - |
| `SimLingo` | [SimLingo: Vision-Only Closed-Loop Autonomous Driving with Language-Action Alignment](https://arxiv.org/abs/2503.09594) | CVPR 2025 | - | - |
| `DrivingGPT` | [DrivingGPT: Unifying Driving World Modeling and Planning with Multi-Modal Autoregressive Transformers](https://arxiv.org/abs/2501.03230) | ICCV 2025 | - | - |
| `UniDrive-WM` | [UniDrive-WM: Unified Understanding, Planning and Generation World Model For Autonomous Driving](https://arxiv.org/abs/2601.04453) | arXiv 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://unidrive-wm.github.io/UniDrive-WM) | - |
| `Raw2Drive` | [Raw2Drive: Reinforcement Learning with Aligned World Models for End-to-End Autonomous Driving (in CARLA v2)](https://arxiv.org/abs/2505.16394) | arXiv 2025 | - | - |
| `OccVAR` | [OccVAR: Scalable 4D Occupancy Prediction via Next-Scale Prediction](https://arxiv.org/abs/2501.03230) | ICLR 2025 | - | - |
| `RenderWorld` | [RenderWorld: World Model with Self-Supervised 3D Label](https://arxiv.org/abs/2501.03230) | ICRA 2025 | - | - |
| `DFIT-OccWorld` | [DFIT-OccWorld: An Efficient Occupancy World Model via Decoupled Dynamic Flow and Image-Assisted Training](https://arxiv.org/abs/2412.13772) | arXiv 2024 | - | - |
| `Drive-OccWorld` | [Drive-OccWorld: Driving in the Occupancy World: Vision-Centric 4D Occupancy Forecasting and Planning via World Models for Autonomous Driving](https://arxiv.org/abs/2501.03230) | AAAI 2025 | - | - |
| `T³Former` | [T³Former: Temporal Graph Classification with Topological Machine Learning](https://arxiv.org/abs/2501.03230) | AAAI 2026 | - | - |
| `OmniNWM` | [OmniNWM: Omniscient Driving Navigation World Models](https://arxiv.org/abs/2510.18313) | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/Ma-Zhuang/OmniNWM)](https://github.com/Ma-Zhuang/OmniNWM) |
| `AD-R1` | [AD-R1: Closed-Loop Reinforcement Learning for End-to-End Autonomous Driving with Impartial World Models](https://arxiv.org/abs/2511.20325) | arXiv 2025 | - | - |
| `WoTE` | [WoTE: End-to-End Driving with Online Trajectory Evaluation via BEV World Model](https://arxiv.org/abs/2501.03230) | ICCV 2025 | - | [![GitHub](https://img.shields.io/github/stars/liyingyanUCAS/WoTE)](https://github.com/liyingyanUCAS/WoTE) |
| `LAW` | [LAW: Enhancing End-to-End Autonomous Driving with Latent World Model](https://arxiv.org/abs/2501.03230) | ICLR 2025 | - | [![GitHub](https://img.shields.io/github/stars/BraveGroup/LAW)](https://github.com/BraveGroup/LAW) |
| `Drive-WM` | [Drive-WM: Driving into the Future: Multiview Visual Forecasting and Planning with World Model for Autonomous Driving](https://arxiv.org/abs/2405.14852) | CVPR 2024 | - | - |
| `SSR` | [SSR: Navigation-Guided Sparse Scene Representation for End-to-End Autonomous Driving](https://arxiv.org/abs/2409.18341) | arXiv 2024 | - | - |
| `SeerDrive` | [SeerDrive: Future-Aware End-to-End Driving: Bidirectional Modeling of Trajectory Planning and Scene Evolution](https://arxiv.org/abs/2510.11092) | arXiv 2025 | - | - |
| `Drive-JEPA` | [Drive-JEPA: Video JEPA Meets Multimodal Trajectory Distillation for End-to-End Driving](https://arxiv.org/abs/2601.22032) | arXiv 2026 | - | - |
| `OccLLaMA` | [OccLLaMA: An Occupancy-Language-Action Generative World Model for Autonomous Driving](https://arxiv.org/abs/2409.03272) | arXiv 2024 | - | - |
| `Doe-1` | [Doe-1: Closed-Loop Autonomous Driving with Large World Model](https://arxiv.org/abs/2412.09627) | arXiv 2024 | - | - |
| `Imagine-2-Drive` | [Imagine-2-Drive: Leveraging High-Fidelity World Models via Multi-Modal Diffusion Policies](https://arxiv.org/abs/2501.03230) | IROS 2025 | - | - |
| `NeMo` | [NeMo: Neural Volumetric World Models for Autonomous Driving](https://arxiv.org/abs/2501.03230) | ECCV 2024 | - | - |

---

## 5. Diffusion-Based Planners

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
| `DiffRefiner` | [DiffRefiner: Coarse to Fine Trajectory Planning via Diffusion Refinement with Semantic Interaction for End to End Autonomous Driving](https://arxiv.org/abs/2511.17150) | AAAI 2026 | - | [![GitHub](https://img.shields.io/github/stars/nullmax-vision/DiffRefiner)](https://github.com/nullmax-vision/DiffRefiner) |
| `DiffusionDrive` | [DiffusionDrive: Truncated Diffusion Model for End-to-End Autonomous Driving](https://arxiv.org/abs/2501.03230) | CVPR 2025 | - | [![GitHub](https://img.shields.io/github/stars/hustvl/DiffusionDrive)](https://github.com/hustvl/DiffusionDrive) |
| `Flow Planner` | [Flow Planner: Flow Matching-Based Autonomous Driving Planning with Advanced Interactive Behavior Modeling](https://arxiv.org/abs/2501.03230) | NeurIPS 2025 | - | - |
| `BEVDiffuser` | [BEVDiffuser: Plug-and-Play Diffusion Model for BEV Denoising with Ground-Truth Guidance](https://arxiv.org/abs/2501.03230) | CVPR 2025 | - | - |
| `Hyper Diffusion Planner` | [Hyper Diffusion Planner: Unleashing the Potential of Diffusion Models for End-to-End Autonomous Driving](https://arxiv.org/abs/2602.22801) | arXiv 2026 | - | - |
| `SafeDiffuser` | [SafeDiffuser: Safe Planning with Diffusion Probabilistic Models](https://arxiv.org/abs/2501.03230) | ICLR 2025 | - | [![GitHub](https://img.shields.io/github/stars/Weixy21/SafeDiffuser)](https://github.com/Weixy21/SafeDiffuser) |
| `CTG++` | [CTG++: Language-Guided Traffic Simulation via Scene-Level Diffusion](https://arxiv.org/abs/2501.03230) | CoRL 2023 | - | - |
| `AutoScenario` | [AutoScenario: Auto-Scenario Generator for Autonomous Vehicle Safety: Multi-Modal Attention-Based Image Captioning Model Using Digital Twin Data](https://arxiv.org/abs/2501.03230) | IEEE Access 2024 | - | - |
| `SceneDiffuser` | [SceneDiffuser: Efficient and Controllable Driving Simulation Initialization and Rollout](https://arxiv.org/abs/2501.03230) | NeurIPS 2024 | - | [![GitHub](https://img.shields.io/github/stars/scenediffuser/scenediffuser)](https://github.com/scenediffuser/scenediffuser) |
| `ReCogDrive` | [ReCogDrive: A Reinforced Cognitive Framework for End-to-End Autonomous Driving](https://arxiv.org/abs/2506.08052) | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://xiaomi-research.github.io/recogdrive) | - |
| `TrajDiff` | [TrajDiff: Trajectory Prediction With Diffusion Probabilistic Models](https://arxiv.org/abs/2501.03230) | IEEE TIP 2025 | - | - |
| `GoalFlow` | [GoalFlow: Goal-Driven Flow Matching for Multimodal Trajectories Generation in End-to-End Autonomous Driving](https://arxiv.org/abs/2503.05689) | CVPR 2025 | - | [![GitHub](https://img.shields.io/github/stars/YvanYin/GoalFlow)](https://github.com/YvanYin/GoalFlow) |
| `GuideFlow` | [GuideFlow: Constraint-Guided Flow Matching for Planning in End-to-End Autonomous Driving](https://arxiv.org/abs/2511.18729) | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/liulin815/GuideFlow)](https://github.com/liulin815/GuideFlow) |
| `DiffusionDriveV2` | [DiffusionDriveV2: Reinforcement Learning-Constrained Truncated Diffusion Modeling in End-to-End Autonomous Driving](https://arxiv.org/abs/2512.07745) | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/hustvl/DiffusionDriveV2)](https://github.com/hustvl/DiffusionDriveV2) |
| `Mimir` | [Mimir: A Customizable Agent Tuning Platform for Enhanced Scientific Applications](https://arxiv.org/abs/2501.03230) | EMNLP Demo 2024 | - | - |
| `ReflectDrive` | [ReflectDrive: Discrete Diffusion for Reflective Vision-Language-Action Models in Autonomous Driving](https://arxiv.org/abs/2509.20109) | arXiv 2025 | - | - |
| `dVLM-AD` | [dVLM-AD: Enhance Diffusion Vision-Language-Model for Driving via Controllable Reasoning](https://arxiv.org/abs/2512.04459) | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://dvlm-ad.github.io) | - |
| `WAM-Diff` | [WAM-Diff: A Masked Diffusion VLA Framework with MoE and Online Reinforcement Learning for Autonomous Driving](https://arxiv.org/abs/2512.11872) | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/fudan-generative-vision/WAM-Diff)](https://github.com/fudan-generative-vision/WAM-Diff) |
| `VDRive` | [VDRive: Leveraging Reinforced VLA and Diffusion Policy for End-to-End Autonomous Driving](https://arxiv.org/abs/2510.15446) | arXiv 2025 | - | - |
| `ViLaD` | [ViLaD: A Large Vision Language Diffusion Framework for End-to-End Autonomous Driving](https://arxiv.org/abs/2508.12603) | arXiv 2025 | - | - |



## 6 Datasets and Benchmarks

### 6.1 Common Datasets (Sorted by Year)

| Dataset | Type | Download | Year | Size |
|:-:|:-:|:-:|:-:|:-:|
| `CARLA` | Sim | https://github.com/carla-simulator/carla | 2017 | - |
| `nuScenes` | Real | https://www.nuscenes.org/nuscenes | 2020 | 1.4M |
| `Waymo` | Real | https://waymo.com/open/ | 2020 | 200M |
| `nuPlan` | Real | https://www.nuscenes.org/nuplan | 2021 | 4.6M |
| `Bench2Drive` | Sim | https://github.com/Thinklab-SJTU/Bench2Drive | 2024 | 2M |
| `NAVSIM` | Real | https://github.com/autonomousvision/navsim | 2024 | - |

### 6.2 Datasets for LLM/VLM-Based Driving Agents (Sorted by Year)

| Dataset | Type | Download | Year | Size |
|:-:|:-:|:-:|:-:|:-:|
| `BDD-X` | Real | https://github.com/JinkyuKimUCB/BDD-X-dataset | 2018 | 26K annotations |
| `Talk2Car` | Real | https://macchina-ai.cs.kuleuven.be/downloads.html | 2019 | 12K |
| `BDD100K` | Real | https://bdd-data.berkeley.edu/ | 2020 | 100K videos |
| `DAIR-V2X` | Real | https://github.com/AIR-THU/DAIR-V2X | 2022 | - |
| `DriveMLMa` | Sim | https://github.com/xiandaguo/drive-mllm | 2023 | Sim |
| `DriveGPT4` | Real | https://cloud.tsinghua.edu.cn/d/adbc8fa3a2fc420ca7bc/ | 2024 | 56K VQA |
| `LaMPilot` | Sim | https://github.com/PurdueDigitalTwin/LaMPilot | 2024 | - |
| `LMDrive` | Sim | https://github.com/opendilab/LMDrive | 2024 | 64K clips |
| `nuScenes-QA` | Real | https://github.com/qiantianwen/NuScenes-QA | 2024 | 460K QA |
| `NuInstruct` | Real | https://github.com/xmed-lab/NuInstruct | 2024 | 91K QA |
| `Reason2Drive` | Real | https://github.com/fudan-zvg/reason2drive | 2024 | 632K |
| `VLAAD` | Real | https://github.com/sungyeonparkk/vision-assistant-for-driving | 2024 | 64K clips |
| `WOMD-Reasoning` | Real | https://waymo.com/open/licensing/ | 2024 | 2,940K QA |
| `AlphaDrive` | Real | https://github.com/hustvl/AlphaDrive | 2025 | 30K |
| `DriveBench` | Real | https://huggingface.co/drive-bench/datasets | 2025 | 20.5K QA |
| `Impromptu-VLA` | Real+Sim | https://github.com/ahydchh/Impromptu-VLA | 2025 | 80K clips |
| `OmniDrive` | Real | https://github.com/NVlabs/OmniDrive | 2025 | 200K QA |

### 6.3 Datasets for Vision-Action Models

| Dataset | Type | Download | Year | Size |
|:-:|:-:|:-:|:-:|:-:|
| `CARLA` | Sim | https://github.com/carla-simulator/carla | 2017 | - |
| `BDD100K` | Real | https://bdd-data.berkeley.edu/ | 2020 | 100K videos |
| `nuScenes` | Real | https://www.nuscenes.org/nuscenes | 2020 | 1.4M frames |
| `Waymo` | Real | https://waymo.com/open/ | 2020 | 200M frames |
| `Argoverse 2` | Real | https://www.argoverse.org/av2.html | 2021 | 250K scenarios |
| `Motion` | Real | https://waymo.com/open/data/motion/ | 2021 | - |
| `nuPlan` | Real | https://www.nuscenes.org/nuplan | 2021 | 4.6M |
| `Bench2Drive` | Sim | https://github.com/Thinklab-SJTU/Bench2Drive | 2024 | 2M |
| `NAVSIM` | Real | https://github.com/autonomousvision/navsim | 2024 | - |
| `RoboBEV` | Real | https://github.com/worldbench/RoboBEV | 2025 | 866K |
| `WOD-E2E` | Real | https://waymo.com/open/ | 2025 | 800K |

### 6.4 Datasets for Vision-Language-Action (VLA) Models (Sorted by Year)

| Dataset | Type | Download | Year | Size |
|:-:|:-:|:-:|:-:|:-:|
| `CARLA` | Sim | https://github.com/carla-simulator/carla | 2017 | - |
| `nuScenes` | Real | https://www.nuscenes.org/nuscenes | 2020 | 1.4M |
| `Waymo` | Real | https://waymo.com/open/ | 2020 | 200M |
| `Argoverse 2` | Real | https://www.argoverse.org/av2.html | 2021 | 250K scenarios |
| `Talk2Car` | Real | https://macchina-ai.cs.kuleuven.be/downloads.html | 2019 | 12K |
| `Bench2Drive` | Sim | https://github.com/Thinklab-SJTU/Bench2Drive | 2024 | 2M |
| `NAVSIM` | Real | https://github.com/autonomousvision/navsim | 2024 | - |
| `DriveLM` | Real | https://github.com/OpenDriveLab/DriveLM | 2024 | 445K QA |
| `DriveCoT` | Sim | https://drivecot.github.io/download.html | 2024 | 36K |
| `CoVLA` | Real | https://huggingface.co/datasets/turing-motors/CoVLA-Dataset | 2025 | 6M frames |
| `NuInteract` | Real | https://github.com/zc-zhao/drivemonkey | 2025 | 239K images |
| `DriveAction` | Real | https://huggingface.co/datasets/LiAuto-DriveAction/drive-action | 2025 | 16.18K QA |

### 6.5 Datasets for Driving World Models (Sorted by Year)

| Dataset | Type | Download | Year | Size |
|:-:|:-:|:-:|:-:|:-:|
| `CARLA` | Sim | https://github.com/carla-simulator/carla | 2017 | - |
| `nuScenes` | Real | https://www.nuscenes.org/nuscenes | 2020 | 1.4M |
| `Waymo` | Real | https://waymo.com/open/ | 2020 | 200M |
| `nuPlan` | Real | https://www.nuscenes.org/nuplan | 2021 | 4.6M |
| `Bench2Drive` | Sim | https://github.com/Thinklab-SJTU/Bench2Drive | 2024 | 2M |
| `NAVSIM` | Real | https://github.com/autonomousvision/navsim | 2024 | - |
| `OpenDV-YouTube` | Real | https://huggingface.co/datasets/OpenDriveLab/OpenDV-YouTube-Language | 2024 | - |
| `RoboBEV` | Real | https://github.com/worldbench/RoboBEV | 2025 | 866K |
| `WOD-E2E` | Real | https://waymo.com/open/ | 2025 | 800K |

### 6.6 Datasets for Diffusion-Based Planners (Sorted by Year)

| Dataset | Type | Download | Year | Size |
|:-:|:-:|:-:|:-:|:-:|
| `CARLA` | Sim | https://github.com/carla-simulator/carla | 2017 | - |
| `nuScenes` | Real | https://www.nuscenes.org/nuscenes | 2020 | 1.4M |
| `Waymo` | Real | https://waymo.com/open/ | 2020 | 200M |
| `nuPlan` | Real | https://www.nuscenes.org/nuplan | 2021 | 4.6M |    
| `Motion` | Real | https://waymo.com/open/data/motion/ | 2021 | - |
| `Bench2Drive` | Sim | https://github.com/Thinklab-SJTU/Bench2Drive | 2024 | 2M |
| `NAVSIM` | Real | https://github.com/autonomousvision/navsim | 2024 | - |
| `OpenDV-YouTube` | Real | https://huggingface.co/datasets/OpenDriveLab/OpenDV-YouTube-Language | 2024 | - |
