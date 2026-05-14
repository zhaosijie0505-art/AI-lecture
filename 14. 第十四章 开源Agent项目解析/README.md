# 第十四章：开源 Agent 项目解析

> 本章选取 Hermes Agent 作为深度解剖对象，带你从源码层面理解一个 production 级别的 AI Agent 是如何构建的。

---

## 本章目录

### Hermes项目深度分析

- **00. 导言** —— 本章学习目标与 Hermes 简介
- **第一节：架构总览与设计哲学** —— 三层架构、入口分工、文件依赖链、五条核心设计原则
- **第二节：run_agent.py 核心循环** —— 迭代预算、持久化事件循环、工具并行化、中断机制
- **第三节：工具注册与编排** —— 自注册模式、AST 发现、ToolEntry、handle_function_call
- **第四节：CLI 配置与交互** —— argparse subcommand、Profile 多租户、TTY 检测、皮肤引擎
- **第五节：消息网关** —— 适配器模式、GatewayRunner、会话管理、凭证锁
- **第六节：会话状态与数据库** —— SQLite WAL 模式、抖动重试、FTS5 全文搜索、用量追踪
- **第七节：子代理委托** —— MapReduce 模式、子代理隔离、工具集限制、心跳保活
- **第八节：MCP 集成** —— Stdio/HTTP 双传输、安全环境过滤、凭证脱敏、采样回调
- **第九节：上下文压缩与提示构建** —— prompt_builder、prompt injection 检测、context_compressor、model_metadata
- **第十节：终端与定时任务** —— 多环境后端、sudo 处理、危险命令审批、cron 调度器、结果投递
- **第十一节：工程智慧与设计哲学** —— 设计模式总结、关键工程细节、演进历史的教训
