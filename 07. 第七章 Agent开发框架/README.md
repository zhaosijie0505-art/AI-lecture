# 第七章 Agent 开发框架

> 框架，让开发 AI 应用像搭积木一样简单。

## 本章内容

| 文章 | 主题 |
|------|------|
| [00. 导言](00.%20导言.md) | 为什么需要框架、主流框架对比 |
| [01. 第一节 Agent 框架概述](01.%20第一节%20Agent框架概述.md) | Chain/Agent/Tool/Callback 核心概念 |
| [02. 第二节 LangChain 深度指南](02.%20第二节%20LangChain深度指南.md) | LCEL、Chain、Tool、Agent、Memory |
| [03. 第三节 LlamaIndex 深度指南](03.%20第三节%20LlamaIndex深度指南.md) | RAG Pipeline、Query Engine、索引类型 |
| [04. 第四节 AutoGen 与多 Agent 框架](04.%20第四节%20AutoGen与多Agent框架.md) | AutoGen、CrewAI、多 Agent 协作 |
| [05. 第五节 企业级框架选型](05.%20第五节%20企业级框架选型.md) | Semantic Kernel、LangGraph、选型建议 |
| [06. 第六节 实战](06.%20第六节%20实战构建企业知识库问答.md) | 完整项目：FastAPI + LlamaIndex + Streamlit |

## 核心概念

**Chain**：串联多个组件的机制，LLMChain/SequentialChain/RouterChain

**Agent**：能够自主决策并执行动作的实体

**Tool**：Agent 可调用的外部能力，@tool 装饰器或 StructuredTool

**Callback**：执行过程中的钩子（日志、监控、Streaming）

## 章节速览

- **第一节**：Chain/Agent/Tool/Callback 核心概念、LangChain vs LlamaIndex 对比
- **第二节**：LCEL 语法、Chain 用法（LLMChain/SequentialChain/RouterChain）、Tool 定义、Memory
- **第三节**：LlamaIndex 数据加载、索引类型（Vector/Summary/Tree）、Query Engine、检索器
- **第四节**：AutoGen 多 Agent 协作、CrewAI 角色定义、Sequential/Group Chat
- **第五节**：Semantic Kernel（微软企业）、LangGraph（复杂工作流）、选型决策树
- **第六节**：完整企业知识库问答实战（FastAPI + LlamaIndex + LangChain + Streamlit）