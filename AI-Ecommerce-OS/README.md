# AI-Ecommerce-OS

> AI 驱动的跨境电商创业操作系统（AI-Ecommerce Operating System）
> 由 AI Agent 协助完成从市场研究到自动化的跨境电商全链路工作。

---

## 项目愿景

用一个由 AI Agent 组成的协作系统，协助创业者完成跨境电商的全流程：

1. **市场研究** — 发现趋势、判断机会
2. **用户需求分析** — 提炼真实需求与痛点
3. **产品筛选** — 从需求反推可售产品
4. **竞争分析** — 评估竞争强度与差异化空间
5. **供应链分析** — 评估货源、成本、履约能力
6. **内容生产** — 批量生产素材、文案、脚本
7. **数据分析** — 监控 KPI、归因、迭代
8. **自动化** — 用工作流串联以上环节

---

## 目录结构

```
AI-Ecommerce-OS/
├── 01_Research/      市场研究产出（报告/需求库/产品库/竞品/趋势）
├── 02_Agents/        7 个 AI Agent 的配置、Prompt、任务
├── 03_Prompts/       Prompt 管理系统（按场景分类）
├── 04_Database/      结构化数据库（CSV，可导入工具）
├── 05_SOP/           标准操作流程（7 个 SOP）
├── 06_Content/       内容素材库（图/视频/脚本/Hook/CTA/UGC）
├── 07_Website/       独立站与落地页资产
├── 08_Automation/    自动化（n8n/MCP/API/Cron/Workflows）
├── 09_Analytics/     数据分析与看板
├── 10_Archive/       归档（已结案/历史版本）
└── Assets/           通用素材与品牌资产
```

---

## Agent 与 8 大目标的职责映射

| 8 大目标            | 主要负责 Agent      | 支撑模块                |
| ------------------- | ------------------- | ----------------------- |
| 1. 市场研究         | Trend_Agent         | 01_Research, 03_Prompts |
| 2. 用户需求分析     | Demand_Agent        | 01_Research             |
| 3. 产品筛选         | Product_Agent       | 04_Database             |
| 4. 竞争分析         | Competitor_Agent    | 01_Research             |
| 5. 供应链分析       | Product_Agent + CEO | 05_SOP03, 04_Database   |
| 6. 内容生产         | Content_Agent       | 06_Content              |
| 7. 数据分析         | Marketing_Agent     | 09_Analytics            |
| 8. 自动化           | CEO_Agent + 08 模块 | 08_Automation           |

> `CEO_Agent` 为总调度，负责跨 Agent 协调、供应链/数据研判、自动化编排。

---

## 快速开始

1. 阅读 [ROADMAP.md](./ROADMAP.md) 了解 30 天计划
2. 查看 [TODO.md](./TODO.md) 获取当前任务
3. 进入 `02_Agents/` 选择需要启用的 Agent，按其 `agent.yaml` 配置
4. 按 `05_SOP/` 中的标准流程执行
5. 所有产出物写入对应目录，并在 `CHANGELOG.md` 记录

---

## 维护原则

- **目录结构稳定**：不随意修改目录，新增能力在既有目录内扩展
- **README 先行**：每个文件夹必有 README 说明用途
- **模板驱动**：新产出物从模板复制，保证一致性
- **数据落库**：结构化数据写入 `04_Database/`，避免散落
- **变更留痕**：每次迭代写入 `CHANGELOG.md`，遵循 [Keep a Changelog](https://keepachangelog.com/) 规范
- **版本语义化**：项目遵循 `MAJOR.MINOR.PATCH` 语义化版本

---

## 版本

- 当前版本：`v0.1.0`（初始化项目骨架）
- 详见 [CHANGELOG.md](./CHANGELOG.md)
