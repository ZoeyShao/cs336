# CS336 Language Modeling from Scratch Resources

Curated on 2026-06-28. Prefer these links over generic blog posts when grounding future lessons.

## Knowledge

- [Course: CS336 official site, Spring 2026](https://cs336.stanford.edu/)
  主入口。Use for: 课程目标、先修要求、日程、作业入口、lecture materials。
- [Videos: CS336 Spring 2026 YouTube playlist](https://www.youtube.com/playlist?list=PLoROMvodv4rMqXOcazWaTUHhq-yembLCV)
  18 个公开视频。Use for: 按课程顺序观看 lectures。
- [Lecture materials: stanford-cs336/lectures](https://github.com/stanford-cs336/lectures)
  Spring 2026 课件和可执行 lecture 脚本。Use for: 对照视频复盘公式、代码和 trace。
- [Archive: CS336 Spring 2025](https://cs336.stanford.edu/spring2025/)
  上一版课程网站。Use for: 对比 2025 版本安排和材料。
- [Archive: CS336 Spring 2024](https://cs336.stanford.edu/spring2024/)
  早期版本课程网站。Use for: 查历史 lecture/assignment 变化。
- [Assignment 1: Basics](https://github.com/stanford-cs336/assignment1-basics)
  Tokenizer、Transformer LM、cross-entropy、AdamW、training loop。Use for: 补齐最小训练栈。
- [Assignment 2: Systems](https://github.com/stanford-cs336/assignment2-systems)
  Profiling、benchmarking、Triton FlashAttention2、memory-efficient/distributed training。Use for: 系统性能与 GPU 瓶颈。
- [Assignment 3: Scaling](https://github.com/stanford-cs336/assignment3-scaling)
  组件理解和 scaling law 拟合。Use for: 从小实验推断大规模训练。
- [Assignment 4: Data](https://github.com/stanford-cs336/assignment4-data)
  Common Crawl 到预训练数据、过滤、去重、混合。Use for: 数据质量和训练结果的联系。
- [Assignment 5: Alignment](https://github.com/stanford-cs336/assignment5-alignment)
  SFT、GRPO、数学推理，另有 optional safety/RLHF supplement。Use for: post-training 和 preference/reasoning RL。
- [Paper: Attention Is All You Need](https://arxiv.org/abs/1706.03762)
  Transformer 原论文。Use for: architecture baseline and notation.
- [Paper: Scaling Laws for Neural Language Models](https://arxiv.org/abs/2001.08361)
  Kaplan scaling laws。Use for: compute/model/data tradeoffs before Chinchilla.
- [Paper: Training Compute-Optimal Large Language Models](https://arxiv.org/abs/2203.15556)
  Chinchilla。Use for: compute-optimal token/model scaling.
- [Paper: FlashAttention-2](https://arxiv.org/abs/2307.08691)
  高效 attention 的 work partitioning。Use for: Assignment 2 的算法背景。
- [Paper: Megatron-LM on GPU clusters](https://arxiv.org/abs/2104.04473)
  tensor/pipeline/data parallel 组合。Use for: parallelism lectures.
- [Paper: Switch Transformers](https://arxiv.org/abs/2101.03961)
  MoE sparse activation。Use for: attention alternatives and MoE tradeoffs.
- [Paper: MMLU](https://arxiv.org/abs/2009.03300)
  经典能力评测基准。Use for: evaluation lecture.
- [Paper: InstructGPT/RLHF](https://arxiv.org/abs/2203.02155)
  SFT + reward model + RLHF pipeline。Use for: post-training baseline.
- [Paper: Direct Preference Optimization](https://arxiv.org/abs/2305.18290)
  DPO。Use for: optional safety alignment and preference optimization.
- [Paper: DeepSeekMath / GRPO](https://arxiv.org/abs/2402.03300)
  GRPO 来源之一。Use for: Assignment 5 reasoning RL.
- [Docs: Triton language](https://triton-lang.org/)
  官方 Triton 文档。Use for: kernels and Assignment 2 implementation.
- [Docs: PyTorch tutorials](https://docs.pytorch.org/tutorials/index.html)
  官方 PyTorch 教程。Use for: profiling, distributed, memory debugging.
- [Docs: einops](https://einops.rocks/)
  tensor rearrangement 文档。Use for: Lecture 2 和 readable tensor code.
- [Docs: NVIDIA CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-programming-guide/index.html)
  CUDA 官方完整指南。Use for: GPU memory hierarchy, kernels, occupancy 背景。
- [Book/site: The Ultra-Scale Playbook](https://nanotron-ultrascale-playbook.static.hf.space/)
  Hugging Face/nanotron 的大规模训练系统实战资源。Use for: distributed training, 5D parallelism, ZeRO, communication overlap.

## Wisdom (Communities)

- [stanford-cs336 GitHub organization](https://github.com/stanford-cs336)
  官方代码和 issue 入口。Use for: assignment bugs, clarifications, release changes; avoid using public solution repos as shortcuts.
- [PyTorch Discuss](https://discuss.pytorch.org/)
  PyTorch 社区。Use for: autograd, distributed training, profiler, CUDA memory questions.
- [NVIDIA Developer Forums: CUDA](https://forums.developer.nvidia.com/c/accelerated-computing/cuda/206)
  CUDA/GPU performance 社区。Use for: kernel-level performance and memory hierarchy questions.
- [Hugging Face Forums](https://discuss.huggingface.co/)
  模型训练、datasets、evaluation、transformers 生态问题。Use for: practical data/model tooling questions.

## Gaps

- 课程官方 Slack 对校外自学者不可用；需要用 GitHub issues、PyTorch/NVIDIA/Hugging Face 社区替代。
- GPU 预算会影响 Assignment 2/4/5 的完整体验；未来需要按你的预算设计 CPU-first 和 small-GPU variants。
