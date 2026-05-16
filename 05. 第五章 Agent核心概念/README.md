# 第五章 Agent 核心概念

> LLM 是大脑，Agent 是会行动的智能体。

## 本章内容

| 文章 | 主题 |
|------|------|
| [00. 导言](00.%20导言.md) | Agent 是什么、为什么需要 Agent |
| [01. 第一节 ReAct 范式](01.%20第一节%20ReAct范式.md) | 边推理边行动，Thought/Action/Observation 循环 |
| [02. 第二节 Plan-and-Execute](02.%20第二节%20Plan-and-Execute模式.md) | 先规划后执行，全局视角 |
| [03. 第三节 Tool Use](03.%20第三节%20ToolUse机制.md) | LLM 如何调用外部工具 |
| [04. 第四节 Memory 机制](04.%20第四节%20Memory机制.md) | 三层记忆架构：Sensory/Working/Long-Term |
| [05. 第五节 Self-Reflection](05.%20第五节%20Self-Reflection与纠错.md) | 自我检查、错误纠正、从反馈学习 |
| [06. 第六节 Autonomous Agent](06.%20第六节%20AutonomousAgent架构.md) | 完整 Agent 架构设计 |

## 核心概念

**Agent vs LLM**：LLM 是被动回答；Agent 是主动行动，能设定目标、使用工具、持续工作。

**ReAct 循环**：Thought（思考下一步）→ Action（执行）→ Observation（观察结果）→ 循环

**三层记忆**：Sensory（当前交互）→ Working（任务状态）→ Long-Term（跨会话知识）

**自我反思**：生成 → 反思 → 修正 → 再反思，直到满意或达到上限

## 章节速览

- **第一节**：ReAct 范式原理、实现代码、与 CoT 的对比
- **第二节**：Plan-and-Execute 先规划后执行、与 ReAct 的选择
- **第三节**：Tool Use 三组件（定义/选择/执行）、工具描述设计、安全考虑
- **第四节**：Memory 三层架构、记忆压缩与优先级管理
- **第五节**：Self-Reflection 三种类型（结果验证/过程回溯/对比学习）
- **第六节**：Autonomous Agent 完整架构、六层设计原则