# 阶段复盘

- id: workflow-002
- version: v1
- owner_agent: CEO_Agent
- status: active
- updated: 2026-07-31
- inputs: phase, kpi_actual, deliverables
- outputs: 01_Research/Reports

## 目标
对阶段目标 vs 实际做复盘，沉淀 Keep/Drop/Improve。

## 上下文注入
- 阶段：{{phase}}
- KPI 实际：{{kpi_actual}}
- 交付物：{{deliverables}}

## 指令
1. 对照目标与实际，列差距与归因。
2. 提炼 Keep / Drop / Improve。
3. 输出下一阶段行动项（含负责 Agent 与截止）。
4. 沉淀资产（SOP/Prompt/数据更新）。
5. 按 `_template_retro.md` 产出。

## 输出格式
- 文件：`YYYYMMDD_阶段_retro_vX.md` → `01_Research/Reports/`
