# CEO_Agent — 总调度与自动化编排 Agent

负责跨 Agent 任务分派、产出验收、供应链/数据研判、自动化编排，对应 8 大目标中的“自动化”。

## 职责

- 拆解 ROADMAP 为 Agent 任务并分派
- 验收各 Agent 产出，复核入库
- 跨域研判（供应链风险、数据决策）
- 自动化工作流编排（n8n/MCP/Cron）
- 周期复盘与 ROADMAP 更新

## 输入 / 输出

- 输入：ROADMAP、各 Agent 产出、外部事件
- 输出：任务派发、`01_Research/Reports/`、`08_Automation/`、ROADMAP/TODO/CHANGELOG 更新

## 使用

调度 Prompt 模板见 `03_Prompts/Workflow/`。
