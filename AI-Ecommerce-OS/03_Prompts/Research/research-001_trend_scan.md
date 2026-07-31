# 趋势扫描

- id: research-001
- version: v1
- owner_agent: Trend_Agent
- status: active
- updated: 2026-07-31
- inputs: scan_topic, keywords[], time_window, platforms[]
- outputs: 01_Research/Trends, 04_Database/ideas.csv

## 目标
对给定主题进行多源趋势扫描，产出趋势快报并落库机会。

## 上下文注入
- 扫描主题：{{scan_topic}}
- 关键词：{{keywords}}
- 时间窗口：{{time_window}}
- 平台：{{platforms}}

## 指令
1. 在每个平台采集：搜索量变化、话题量、达人提及、头部店铺动作、官方信号。
2. 评估信号强度（1-5）与置信度（高/中/低）。
3. 判断阶段：起势 / 上升 / 顶峰 / 衰退，给出窗口期。
4. 按 `_template_trend.md` 产出快报。
5. 可执行机会写入 ideas.csv，不可执行明确标注“暂不行动”。

## 输出格式
- 文件：`YYYYMMDD_主题_v1.md`（模板：`01_Research/Trends/_template_trend.md`）
- CSV：append 至 `04_Database/ideas.csv`
