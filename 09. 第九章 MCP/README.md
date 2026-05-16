# 第九章 MCP（模型上下文协议）

> 让 AI 连接一切的标准协议。

## 本章内容

| 文章 | 主题 |
|------|------|
| [00. 导言](00.%20导言.md) | 为什么需要 MCP、章节速览 |
| [01. 第一节 MCP 概述](01.%20第一节%20MCP概述.md) | 协议原理、核心概念、与传统 API 对比 |
| [02. 第二节 MCP 架构详解](02.%20第二节%20MCP架构详解.md) | Host/Client/Server 架构、协议流程、传输层、安全模型 |
| [03. 第三节 MCP 工具开发](03.%20第三节%20MCP工具开发.md) | 工具/资源/Prompt 开发、完整 Server 模板 |
| [04. 第四节 开源 MCP Servers](04.%20第四节%20开源MCP_Servers.md) | 官方/社区 Server、Claude Desktop 配置 |
| [05. 第五节 MCP 实战](05.%20第五节%20MCP实战.md) | 本地配置、自定义 Server 开发、Cursor 集成 |

## 核心概念

**MCP = Model Context Protocol**：连接 AI 与外部工具/数据/文件系统的标准协议

**核心架构**：Host（Claude Desktop/Cursor）→ Client → Server（文件系统/GitHub/数据库等）

**三大核心概念**：
- **Tools**：AI 可调用的函数
- **Resources**：AI 可读取的数据
- **Prompts**：可复用模板

## 章节速览

- **第一节**：MCP 解决了工具重复开发、接口不统一的问题，核心概念（Host/Client/Server/Tools/Resources/Prompts）
- **第二节**：详细架构（stdio/HTTP/WebSocket 传输）、协议消息格式、安全模型（用户确认/资源隔离/权限控制）
- **第三节**：工具开发（@list_tools/@call_tool）、资源开发、Prompt 模板开发、完整天气 Server 示例
- **第四节**：官方 Server（文件系统/GitHub/Slack/Brave/Google Maps）、社区 Server（数据库/云服务/消息通知）、Claude Desktop 配置
- **第五节**：本地配置实战、自定义公司知识库 MCP（文档/员工/项目工具）、Cursor 集成