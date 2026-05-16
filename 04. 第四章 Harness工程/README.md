# 第四章 Harness 工程

> 没有度量，就没有优化。

## 本章内容

| 文章 | 主题 |
|------|------|
| [00. 导言](00.%20导言.md) | 本章结构、为什么需要 Harness 工程 |
| [01. 第一节 Harness 与评估框架概述](01.%20第一节%20Harness%20与评估框架概述.md) | AI 测试特殊性、四大维度、框架选型 |
| [02. 第二节 核心评估指标体系](02.%20第二节%20核心评估指标体系.md) | 准确性/质量/安全/效率指标 |
| [03. 第三节 RAG 评估工具 RAGAS](03.%20第三节%20RAG评估工具RAGAS.md) | 四大指标：Faithfulness/Relevancy/Precision/Recall |
| [04. 第四节 主流 Benchmark 详解](04.%20第四节%20主流Benchmark详解.md) | MMLU/BIG-bench/GSM8K/TruthfulQA/MT-Bench |
| [05. 第五节 微调 vs RAG 决策框架](05.%20第五节%20微调vsRAG决策框架.md) | 何时微调、何时 RAG、如何结合 |
| [06. 第六节 实战案例](06.%20第六节%20实战案例.md) | 企业级 AI 评估体系完整构建流程 |

## 核心概念

**AI 测试 vs 传统软件测试**：传统软件输入 A 输出 B 是确定的；AI 输出是概率性的，同一输入可能有多种正确回答。

**Harness = 指标 + 数据集 + 评估器 + 报告 + 基准**

**RAGAS 四指标**：Faithfulness（忠诚度）、Answer Relevancy（相关性）、Context Precision（排序）、Context Recall（召回）

## 章节速览

- **第一节**：为什么 AI 需要专门测试框架，四大评估维度
- **第二节**：EM/F1/ROUGE/BERTScore/LLM-as-Judge 等指标详解
- **第三节**：RAGAS 框架使用完整教程
- **第四节**：MMLU / BIG-bench / GSM8K / TruthfulQA / MT-Bench / C-Eval
- **第五节**：微调 vs RAG 的决策树和混合策略
- **第六节**：七步构建企业级评估体系 + CI/CD 集成