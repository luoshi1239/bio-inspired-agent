# 关键论文索引

> 生物启发式 Agent 架构的核心论文与项目。
> 按模式分类，每条含：作者/机构、时间、核心贡献。

---

## 蜂群智能（Swarm Intelligence）

| 论文/项目 | 作者/机构 | 时间 | 核心贡献 |
|----------|----------|------|---------|
| **RecursiveMAS** — Recursive Multi-Agent Systems | Zou, Pan, Qiu, Lu et al.（Stanford / MIT / UIUC / HKUST / Tong Zhang组 / James Zou组） | 2026.04 | 递归多智能体系统，RecursiveLink潜空间传递。准确率+8.3%，速度1.2-2.4x，Token↓34.6-75.6%。三赢突破。 |
| **SOHM** — Society of HiveMind | ETH Zurich | 2025 | 6个小型模型（Llama-3-3B、Qwen-2.5-3B）蜂群协作，在MMLU-Pro上超越单体9.2%和6.2%，甚至超过Llama-3-8B单体4.4%。证明密集推理任务上小模型集体>大模型单体。 |
| **SwarmAgentic** — Towards Fully Automated Agentic System Generation via Swarm Intelligence | EMNLP 2025 | 2025 | 将Agent系统设计视为粒子群优化（PSO）问题，自动搜索最优的Agent角色分配、通信拓扑和任务分解策略。自动化Agent系统设计的主线之一。 |
| **Kimi K2.6 Agent Swarm** | Moonshot AI（月之暗面） | 2026.04 | Agent Swarm从100扩展到300子智能体，协调步骤1,500→4,000。Claw Groups实现跨模型异构蜂群（Claude/GPT/Kimi可在共享工作空间协作）。BrowseComp基准达86.3%。 |
| 蜜蜂巢址选择动态系统建模 | Naomi Leonard团队（普林斯顿） | — | 分叉动态、价值敏感型决策、摇摆舞强度传递质量信息。生物启发的理论源头。 |

---

## 蚁群优化与 Stigmergy

| 论文/项目 | 作者/机构 | 时间 | 核心贡献 |
|----------|----------|------|---------|
| **AMRO-S** — Efficient and Interpretable Multi-Agent LLM Routing via Ant Colony Optimization | Wang, Zhang, Zhang et al. | 2026.03 | 蚁群优化做LLM路由，信息素专家机制。4.7x加速，准确率稳定96%+，可解释（信息素可视化=自动工作流发现）。 |
| **S-MADRL** — Stigmergic Multi-Agent Deep Reinforcement Learning | Georgia Tech | 2025 | 虚拟信息素（Virtual Pheromones）实现去中心化涌现协调。可扩展性从3-4个Agent提升到8个（传统方法超过3-4个就退化）。 |
| **Understanding Graph** — for Claude Code Agent Teams | — | 2025 | 将Stigmergy直接应用于Claude Code Agent Teams，通过共享Graph（MCP读写）实现间接协调。Commit Message=协调层，Trigger标签=分类。 |

---

## 选择性遗忘与记忆

| 论文/项目 | 作者/机构 | 时间 | 核心贡献 |
|----------|----------|------|---------|
| **FadeMem** — Biologically-Inspired Agent Memory Architecture | — | 2025 | 基于艾宾浩斯遗忘曲线的Agent记忆架构。差异化衰减率、双层记忆层次、LLM引导的冲突解决。存储减少45%，多跳推理和检索性能一致提升。 |

---

## 免疫系统

| 论文/项目 | 作者/机构 | 时间 | 核心贡献 |
|----------|----------|------|---------|
| **ANIS** — Agent-Native Immune System | — | 2026.06 | 首个嵌入Agent认知循环的内生防御架构。六层免疫塔（L0-L5），Harness Triad（Meta/Self/Auto）驱动持续免疫学习（CIL）。对齐=静态宪法，免疫=动态执法。 |

---

## 鸟群与群体行为

| 论文/项目 | 作者/机构 | 时间 | 核心贡献 |
|----------|----------|------|---------|
| **Boids 模型** | Craig Reynolds | 1986 | 三条规则（分离/对齐/聚合）解释复杂群体行为。所有群体行为模拟的理论基础。 |
| LLM Flocking 研究 | — | — | 发现LLM无法直接理解"保持距离"等空间概念，倾向于收敛到平均位置或发散。提示：生物模式需工程化转换，不能直接映射。 |

---

## 效率对比总结（RecursiveMAS 数据）

| 维度 | 单Agent | 并行多Agent | 递归蜂群 (RecursiveMAS) |
|------|---------|------------|------------------------|
| 准确率 | 基线 | +3~5% | **+8.3%** |
| 推理速度 | 1x | 0.3~0.5x | **1.2~2.4x** |
| Token消耗 | 1x | 4~15x | **↓34.6~75.6%** |
| 思考深度 | 浅 | 中（分散） | **深（递归深化）** |
| 可扩展性 | 受上下文限制 | 边际递减 | **稳定梯度，高效** |

数据来源：RecursiveMAS (arXiv:2604.25917) 在9个基准测试上的综合结果。

---

## 搜索关键词

想找更多论文，用这些关键词：
- `multi-agent system` / `agentic system`
- `swarm intelligence` / `collective intelligence`
- `stigmergy` / `ant colony optimization` / `ACO`
- `agent memory` / `forgetting mechanism` / `memory architecture`
- `recursive reasoning` / `recursive multi-agent`
- `biologically inspired` / `bio-inspired AI`
- `agent safety` / `agent immune system`
