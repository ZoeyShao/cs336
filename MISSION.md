# Mission: CS336 Language Modeling from Scratch

## Why
你是 AI 专业硕士，已有一定大模型基础。学习 CS336 的目标不是从零入门，而是系统补齐从 tokenizer、Transformer、训练系统、scaling law、数据、评测到 post-training 的工程闭环，形成能读懂、实现、诊断和取舍现代语言模型训练栈的知识体系。

## Success looks like
- 能把一篇 LLM 训练或 post-training 论文拆成模型、数据、优化、系统、评测五类假设。
- 能从头实现一个最小 Transformer LM 训练栈，并解释 tokenizer、loss、optimizer、checkpoint、采样和 perplexity 的关键边界条件。
- 能估算一次训练或推理的 FLOPs、显存、通信和数据需求，知道瓶颈大致在哪里。
- 能判断 scaling law、数据清洗、评测和 alignment 方法在具体项目中的适用范围。

## Constraints
- 以查漏补缺为主，优先补课程中容易被高层 LLM 综述跳过的底层实现和系统细节。
- 以官方课程材料、assignment handout、论文和高质量工程文档为知识来源。
- 练习应尽量可本地验证；需要 GPU 的部分先在 CPU 或小规模样例上做正确性验证。

## Out of scope
- 不追求完整复现大规模模型训练成本。
- 不优先学习面向产品的 prompt engineering 或 agent 应用层套路。
- 不使用公开作业答案替代自己的实现。
