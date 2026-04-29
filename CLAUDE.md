# Claude Code 开发指南

## MCP 工具

### codebase-memory-mcp
代码知识图谱 MCP 工具，基于 Tree-Sitter 索引了整个项目。可大幅提升代码探索效率。

**已索引项目**: claude-code-source (`~/Desktop/explore/claude-code-source`)
**图谱规模**: 22,549 nodes / 70,275 edges

**常用查询**:
- `search_graph` — 按名称/标签/文件搜索符号
- `trace_call_path` — 追踪函数调用链（depth=1-5）
- `query_graph` — Cypher 风格查询（MATCH/RETURN）
- `get_architecture` — 获取项目架构总览
- `get_code_snippet` — 按函数名直接读取源码
- `detect_changes` — Git diff 变更影响分析

探索代码时，优先使用 `codebase-memory-mcp` 工具代替多轮 Grep/Glob。
