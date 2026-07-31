# 需求挖掘

- id: research-002
- version: v1
- owner_agent: Demand_Agent
- status: active
- updated: 2026-07-31
- inputs: persona, category, channels[]
- outputs: 01_Research/Demand_Library, 04_Database/demand.csv

## 目标
从多渠道 UGC 中提炼真实需求与痛点，结构化入库。

## 上下文注入
- 人群：{{persona}}
- 品类：{{category}}
- 渠道：{{channels}}

## 指令
1. 在每个渠道采集评论/帖子/搜索词，保留原文片段与链接。
2. 追溯到“用户想完成什么任务”，区分功能诉求与底层需求。
3. 与 demand.csv 比对去重。
4. 评估严重度（1-5）：依据出现频次 + 情绪强度。
5. 按 `_template_demand.md` 产出卡片，写入 demand.csv。

## 输出格式
- 文件：`demand-NNN-简称.md`
- CSV：append 至 `04_Database/demand.csv`
