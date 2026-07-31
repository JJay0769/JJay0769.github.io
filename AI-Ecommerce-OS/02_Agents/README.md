# 02_Agents — AI Agent 配置中心

> 7 个 AI Agent 的配置、人设 Prompt、任务清单统一管理于此。
> Agent 之间通过 `04_Database/` 与 `01_Research/` 进行数据协作，由 CEO_Agent 统一调度。

---

## Agent 清单

| Agent              | 职责                       | 对应 8 大目标                |
| ------------------ | -------------------------- | ---------------------------- |
| Trend_Agent        | 趋势扫描、市场研究         | 1. 市场研究                  |
| Demand_Agent       | 用户需求采集与结构化       | 2. 用户需求分析              |
| Product_Agent      | 产品筛选、供应链研判       | 3. 产品筛选 / 5. 供应链分析  |
| Competitor_Agent   | 竞品监控与差异化分析       | 4. 竞争分析                  |
| Marketing_Agent    | 投放、数据分析、增长       | 7. 数据分析                  |
| Content_Agent      | 内容生产                   | 6. 内容生产                  |
| CEO_Agent          | 总调度、复盘、自动化编排   | 8. 自动化 / 跨域研判         |

---

## 每个 Agent 目录的标准结构

```
<Agent>/
├── README.md        Agent 说明与使用方式
├── agent.yaml       Agent 配置（身份/能力/工具/输入输出/约束）
├── prompt.md        Agent 系统 Prompt（人设 + 工作准则）
└── tasks.md         该 Agent 的任务追踪看板
```

> Agent 的具体业务 Prompt 模板统一放在 `03_Prompts/`，本目录的 `prompt.md` 仅放系统级人设。

---

## Agent 协作机制

1. CEO_Agent 根据 ROADMAP 拆解任务并分派
2. 各 Agent 接收任务 → 产出 → 写入对应目录 + 数据库
3. 产出物由 CEO_Agent 验收，结果记录在各自 `tasks.md`
4. 跨 Agent 协作通过 `04_Database/` 的共享表（如 demand/products）传递

## 配置加载方式

`agent.yaml` 是 Agent 的单一配置源，可被 n8n / 自研编排器 / MCP 读取。字段说明见各 Agent 的 `agent.yaml` 内注释。
