# 第八章 RAG 进阶

> 从"能跑"到"跑好"，RAG 高级技巧实战。

## 本章内容

| 文章 | 主题 |
|------|------|
| [00. 导言](00.%20导言.md) | 为什么需要 RAG 进阶、章节速览 |
| [01. 第一节 Query 改写与扩展](01.%20第一节%20Query改写与扩展.md) | HyDE、Query Expansion、Query Decomposition、Step-Back |
| [02. 第二节 多跳推理与链式检索](02.%20第二节%20多跳推理与链式检索.md) | CoT Retrieval、Forward/Backward Chain、Iterative RAG、Graph RAG |
| [03. 第三节 Agentic RAG](03.%20第三节%20AgenticRAG.md) | Agent 驱动的 RAG、工具集、自主决策 |
| [04. 第四节 RAG 评估与优化](04.%20第四节%20RAG评估与优化.md) | RAGAs、Hit Rate/MRR/NDCG、问题定位与解决 |

## 核心概念

**HyDE**：用 LLM 生成假设答案，再检索，提高语义模糊查询的效果

**Query Decomposition**：分解复杂问题为多个子问题，分别检索再合并

**Multi-hop Reasoning**：需要多步推理的复杂问题，链式检索

**Agentic RAG**：Agent 作为大脑，自主决定检索策略和迭代

**RAGAs**：主流 RAG 评估框架（Faithfulness/Answer Relevance/Context Precision）

## 章节速览

- **第一节**：HyDE（假设答案检索）、Query Expansion（多角度扩展）、Query Decomposition（问题分解）、Step-Back（退后一步泛化）
- **第二节**：CoT Retrieval（思维链检索）、Forward/Backward Chain（图推理）、Iterative RAG（迭代）、Graph RAG（知识图谱增强）
- **第三节**：Agentic RAG 架构（Agent + 工具集 + Memory）、完整代码实现、Self-RAG 简介
- **第四节**：RAGAs 指标体系、传统 IR 指标（Hit Rate/MRR/NDCG）、常见问题定位（召回率低/幻觉/截断）与解决、完整评估 Pipeline