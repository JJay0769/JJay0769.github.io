# SOP01 — 市场研究

- 版本：v1
- 主导：Trend_Agent
- 参与：Demand_Agent、CEO_Agent
- 触发：每周例行 / 临时任务

## 目标
发现趋势信号，产出市场综述与机会清单。

## 流程
1. CEO_Agent 派发扫描主题、关键词、平台、时间窗口。
2. Trend_Agent 多源采集（搜索量/社媒/达人/店铺/官方信号）。
3. 评估信号强度（1-5）与置信度，判断阶段与窗口。
4. 产出趋势快报 → `01_Research/Trends/`，必要时升级为市场综述 → `01_Research/Market_Report/`。
5. Demand_Agent 基于机会挖掘需求 → `01_Research/Demand_Library/` + `demand.csv`。
6. CEO_Agent 复核后落库 `ideas.csv`。

## 产出
- `01_Research/Trends/*.md`
- `01_Research/Market_Report/*.md`（按需）
- `01_Research/Demand_Library/*.md`
- `04_Database/ideas.csv`、`demand.csv`

## 验收标准
- 每条机会 ≥3 类独立数据源
- 每条需求 ≥2 个独立证据
- 文件命名与模板规范
