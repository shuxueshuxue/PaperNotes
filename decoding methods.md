#paper 

[DSVD_Dynamic_SelfVerify_Decoding_for_Faithful_Generation_in_Large_Language_Models_697eb3e375cbf9a636a266c6_main](DSVD_Dynamic_SelfVerify_Decoding_for_Faithful_Generation_in_Large_Language_Models_697eb3e375cbf9a636a266c6_main.pdf)

## A. Decoding-Time Control / Guided Decoding

| 论文 | 链接 | 简介 |
|------|------|------|
| **Reward-Augmented Decoding (RAD)** — Deng & Raffel, EMNLP 2023 | [PDF](https://aclanthology.org/2023.emnlp-main.721.pdf) | 每步取 top-k token，用 reward model 打分后加回 logits 做 soft bias。最像"hook→action"的解码原语。 |
| **DeAL: Decoding-time Alignment** — ACL 2025 | [PDF](https://aclanthology.org/2025.acl-long.1274.pdf) | 把解码建模成 search，用 heuristic 函数引导路径选择。可插拔约束，偏搜索视角。 |
| **DExperts / LM Arithmetic** — Hinton et al. | [Paper](https://arxiv.org/abs/2105.03023) | 用正/负专家 prompt 分别跑 logits，然后做线性组合（logits = base + α·expert − β·anti-expert）。零训练 soft steering。 |

---

## B. Activation Steering / Representation Engineering

| 论文 | 链接 | 简介 |
|------|------|------|
| **Representation Engineering (RepE)** — Zou et al., 2023 | [PDF](https://arxiv.org/pdf/2310.01405) | 用对比 prompt 抽取"概念方向"向量，在残差流上加减实现 soft 控制（情感、风格、安全等）。 |
| **Steering Vectors / Activation Addition** — Turner et al. | [Blog](https://www.lesswrong.com/posts/5spBue2z2tw4JuDCx/steering-gpt-2-xl-by-adding-an-activation-vector) / [Paper](https://arxiv.org/abs/2308.10248) | 更早期的 steering 工作，展示在中间层加向量能改变行为。 |

---

## C. Uncertainty / Sensitivity 作为触发信号

| 论文 | 链接 | 简介 |
|------|------|------|
| **Semantic Entropy** — Farquhar et al., Nature 2024 | [PDF](https://www.nature.com/articles/s41586-024-07421-0) | 用"语义聚类后的熵"度量不确定性，区分"措辞多样"和"含义分歧"。可作为内部 hook 触发信号。 |
| **Shaking to Reveal: Perturbation-Based Hallucination Detection** — 2025 | [PDF](https://seongheon-96.github.io/assets/pdf/shaking.pdf) | 对输入加扰动，看中间层表征变化幅度，用来检测幻觉。"扰动敏感性→触发"的直接实现。 |

---

## D. Guardrails / Runtime Rule Systems（偏工程但有参考价值）

| 项目/论文 | 链接 | 简介 |
|-----------|------|------|
| **NeMo Guardrails** — NVIDIA, EMNLP 2023 Demo | [GitHub](https://github.com/NVIDIA/NeMo-Guardrails) / [Paper](https://aclanthology.org/2023.emnlp-demo.40.pdf) | 可编程的对话 rails，支持 input/output/dialog/retrieval/execution 多阶段触发。偏 runtime 流程，但架构思路有用。 |

---

## E. Speculative / Verifier-Guided Decoding（机制相关）

| 论文 | 链接 | 简介 |
|------|------|------|
| **Speculative Decoding** — Leviathan et al., 2023 | [PDF](https://arxiv.org/pdf/2211.17192) | Draft-then-verify 范式的原版。你的 PRD 本质上是把 verifier 从"概率一致性"换成"语义规则"。 |

---

## F. 你吐槽过但仍有参考价值的

| 论文 | 链接 | 简介 |
|------|------|------|
| **DISCIPL (Self-Steering LMs)** — MIT, 2025 | [PDF](https://arxiv.org/pdf/2504.07081) | 用 SMC 做 inference-time 控制，允许写 score update 作为 soft constraint。框架表达力强，但例子确实像玩具。 |
