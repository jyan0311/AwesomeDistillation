# Awesome On-Policy Distillation

A curated list of papers, frameworks, and resources on On-Policy Distillation (OPD).

## Contents

- [Surveys & Overviews](#surveys--overviews)
- [Foundations](#foundations)
- [Core Methods](#core-methods)
- [Stability & Training Dynamics](#stability--training-dynamics)
- [Self-Distillation](#self-distillation)
- [Privileged Information](#privileged-information)
- [Applications](#applications)
- [Frameworks](#frameworks)
- [Industrial Recipes](#industrial-recipes)
- [Contributing](#contributing)
- [License](#license)

## Surveys & Overviews

| Title | Venue | Year | Links |
|---|---|---|---|
| [On-Policy Distillation: A Survey](https://arxiv.org/abs/2604.00626) | arXiv | 2026 | [PDF](https://arxiv.org/pdf/2604.00626) |

## Foundations

- [GKD: Generalized Knowledge Distillation](https://arxiv.org/abs/2306.13649) ![NeurIPS](https://img.shields.io/badge/NeurIPS-2023-blue) ![arXiv](https://img.shields.io/badge/arXiv-2306.13649-red)
  - Unifies forward KL, reverse KL, and JSD under a single distillation framework.
- [MiniLLM: Knowledge Distillation of Large Language Models](https://arxiv.org/abs/2306.08543) ![ICLR](https://img.shields.io/badge/ICLR-2024-blue) ![arXiv](https://img.shields.io/badge/arXiv-2306.08543-red)
  - Uses reverse KL to avoid overestimating low-probability regions of the teacher.

## Core Methods

- [AOPD: Asymmetric On-Policy Distillation](https://arxiv.org/abs/XXXX.XXXXX) ![ICML](https://img.shields.io/badge/ICML-2026-blue)
  - Uses different divergences for positive and negative advantage regions.
- [TrOPD: Trust Region On-Policy Distillation](https://arxiv.org/abs/XXXX.XXXXX) ![ICLR](https://img.shields.io/badge/ICLR-2026-blue)
  - Restricts OPD to teacher-reliable regions.
- [DistiLLM: Towards Streamlined Distillation for Large Language Models](https://arxiv.org/abs/2402.03898) ![ICML](https://img.shields.io/badge/ICML-2024-blue) ![arXiv](https://img.shields.io/badge/arXiv-2402.03898-red)
  - Introduces skew KL and adaptive off-policy strategy.
- [DistiLLM-2: A Contrastive Approach Boosts the Distillation of LLMs](https://arxiv.org/abs/2503.07067) ![ICML](https://img.shields.io/badge/ICML-2025-blue) ![arXiv](https://img.shields.io/badge/arXiv-2503.07067-red)
  - Uses skew KL for teacher outputs and skew reverse KL for student outputs.

## Stability & Training Dynamics

- [CADENCE: Coverage-Adaptive Divergence Scheduling for On-Policy Distillation](https://arxiv.org/abs/XXXX.XXXXX) ![ICLR](https://img.shields.io/badge/ICLR-2026-blue)
  - Adaptively schedules forward/reverse KL based on student coverage.
- [SEAD: Capability-Aware Curriculum for On-Policy Distillation](https://arxiv.org/abs/XXXX.XXXXX) ![NeurIPS](https://img.shields.io/badge/NeurIPS-2025-blue)
  - Uses prompt-level pass rates to schedule OPD supervision.

## Self-Distillation

- [OPSD: On-Policy Self-Distillation](https://arxiv.org/abs/XXXX.XXXXX) ![NeurIPS](https://img.shields.io/badge/NeurIPS-2025-blue)
  - Student samples on-policy; teacher provides reverse-KL penalty.

## Privileged Information

- [π-Distill: Privileged Information Distillation](https://arxiv.org/abs/2602.04942) ![ICML](https://img.shields.io/badge/ICML-2026-blue) ![arXiv](https://img.shields.io/badge/arXiv-2602.04942-red)
  - Jointly trains a PI-conditioned teacher and an unconditioned student with shared parameters.
- [PC-OPD: Privileged Contrastive On-Policy Distillation](https://arxiv.org/abs/XXXX.XXXXX) ![arXiv](https://img.shields.io/badge/arXiv-XXXX.XXXXX-red)
  - Combines offline teacher anchoring with asymmetric on-policy OPD and support-driven scheduling.

## Applications

- [Speculative Decoding via On-Policy Distillation](https://arxiv.org/abs/XXXX.XXXXX) ![ICML](https://img.shields.io/badge/ICML-2025-blue)
  - Distills draft models on-policy for speculative decoding.

## Frameworks

- [verl](https://github.com/volcengine/verl) ![GitHub](https://img.shields.io/badge/GitHub-verl-green)
  - RL framework with OPD support.
- [EasyOPD](https://github.com/nick7nlp/EasyOPD) ![GitHub](https://img.shields.io/badge/GitHub-EasyOPD-green)
  - A lightweight framework for on-policy distillation experiments.

## Industrial Recipes

- [Qwen3 Technical Report](https://arxiv.org/abs/2505.09388) ![arXiv](https://img.shields.io/badge/arXiv-2505.09388-red)
  - Includes strong-to-weak distillation recipe.
- [DeepSeek-V4 Technical Report](https://arxiv.org/abs/XXXX.XXXXX) ![arXiv](https://img.shields.io/badge/arXiv-XXXX.XXXXX-red)
  - Discusses on-policy distillation for reasoning models.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

[CC0](LICENSE)