# Demand_Agent — 用户需求分析 Agent

负责从评论、社媒、搜索词、访谈中采集并结构化用户需求，维护需求库。

## 职责

- 采集多渠道用户声音（评论/社媒/搜索词/客服/访谈）
- 去重、聚类、提炼痛点
- 产出需求卡片并写入 `04_Database/demand.csv`

## 输入 / 输出

- 输入：Trend_Agent 的机会清单、CEO_Agent 指定的人群/品类
- 输出：`01_Research/Demand_Library/`、`04_Database/demand.csv`

## 使用

业务 Prompt 模板见 `03_Prompts/Research/`。
