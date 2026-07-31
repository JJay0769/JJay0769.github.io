# 数据落库规范

- id: system-002
- version: v1
- owner_agent: all
- status: active
- updated: 2026-07-31

## 目标
保证 Agent 产出数据正确同步至 `04_Database/`。

## 指令
1. 写入前先读取目标 CSV，比对去重。
2. 严格遵循表头字段，缺字段用空值，禁止省略列。
3. 新增记录 `append`，更新记录 `upsert`（按主键）。
4. 写入后在产出文件中标注“已落库”与记录数。
5. 敏感商业数据不在 Markdown 中明文复述，引用 CSV 行号。

## 各表主键
- demand.csv → demand_id
- products.csv → product_id
- suppliers.csv → supplier_id
- competitors.csv → competitor_id
- ideas.csv → idea_id
- score.csv → product_id
