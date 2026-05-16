# 第六章 RAG 基础全流程

> 让 AI 学会查资料，而不是死记硬背。

## 本章内容

| 文章 | 主题 |
|------|------|
| [00. 导言](00.%20导言.md) | RAG 是什么、为什么需要、与微调对比 |
| [01. 第一节 RAG 概述](01.%20第一节%20RAG概述与工作流程.md) | RAG 三组件、三大流程、与微调对比 |
| [02. 第二节 向量数据库](02.%20第二节%20向量数据库与Embedding.md) | Embedding 原理、ChromaDB/FAISS、相似度计算 |
| [03. 第三节 文档分块](03.%20第三节%20文档分块策略.md) | 固定大小/递归/语义分块、Parent Document |
| [04. 第四节 检索策略](04.%20第四节%20检索策略与排序.md) | BM25/向量/混合搜索、Reranking、MMR |
| [05. 第五节 生成阶段](05.%20第五节%20生成阶段与上下文注入.md) | Prompt 模板、上下文组织、生成后验证 |
| [06. 第六节 完整 Pipeline](06.%20第六节%20完整RAGPipeline实现.md) | 端到端代码实现、生产部署建议 |

## 核心概念

**RAG = 检索（Retrieval）+ 增强（Augmented）+ 生成（Generation）**

**Embedding**：把文本转为向量，语义相似的内容向量也相似

**分块策略**：chunk_size（块大小）和 chunk_overlap（重叠）的平衡

**混合搜索**：BM25（精确）+ 向量搜索（语义）的融合

## 章节速览

- **第一节**：RAG 三组件（Ingestion/Retrieval/Generation）、与微调对比
- **第二节**：Embedding 原理、向量数据库选型（ChromaDB/FAISS/Milvus）
- **第三节**：分块策略（固定/递归/语义）、Parent Document Retrieval
- **第四节**：三种检索方法、Reranking（MMR/Cross-Encoder）、查询优化
- **第五节**：Prompt 模板设计、上下文压缩、生成后验证
- **第六节**：完整 RAG Pipeline 代码实现（700+ 行）