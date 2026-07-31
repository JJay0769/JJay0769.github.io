# 竞品单店分析

- id: research-005
- version: v1
- owner_agent: Competitor_Agent
- status: active
- updated: 2026-07-31
- inputs: product_id, competitor_scope
- outputs: 01_Research/Competitor, 04_Database/competitors.csv

## 目标
对竞品店铺做六维深度分析，输出差异化攻击点。

## 上下文注入
- 关联产品：{{product_id}}
- 竞品范围：{{competitor_scope}}

## 指令
1. 发现竞品店铺（搜索/广告库/达人/关联推荐）。
2. 六维分析：流量、价格带、内容、口碑、履约、营销。
3. 流量/销量数据标注“估算”并给依据。
4. 给出可执行的差异化攻击点。
5. 按 `_template_competitor.md` 产出，关键数据写入 competitors.csv。

## 输出格式
- 文件：`competitor-店铺名_YYYYMMDD.md`
- CSV：append competitors.csv
