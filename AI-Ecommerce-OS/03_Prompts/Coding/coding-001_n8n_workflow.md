# n8n 工作流开发

- id: coding-001
- version: v1
- owner_agent: CEO_Agent
- status: active
- updated: 2026-07-31
- inputs: workflow_goal, trigger, nodes_spec
- outputs: 08_Automation/n8n, 08_Automation/Workflows

## 目标
按规范产出 n8n 工作流设计与实现。

## 上下文注入
- 目标：{{workflow_goal}}
- 触发器：{{trigger}}
- 节点规格：{{nodes_spec}}

## 指令
1. 先在 `08_Automation/Workflows/` 产出设计稿（节点图 + 数据流 + 异常处理）。
2. 实现放入 `08_Automation/n8n/`，命名 `wf-NNN-简称.json`。
3. 含 dry-run 与错误重试策略。
4. 标注所需凭证（不写入真实密钥）。
5. 更新 `08_Automation/Cron/` 定时配置。

## 输出格式
- 设计稿：`wf-NNN-简称_design.md`
- 实现：`wf-NNN-简称.json`
