# Hook 生成

- id: content-001
- version: v1
- owner_agent: Content_Agent
- status: active
- updated: 2026-07-31
- inputs: product_id, usp[], pain_points[], platform
- outputs: 06_Content/Hooks

## 目标
生成前 3 秒抓人的 Hook 文案，含 AB 变体与平台适配。

## 上下文注入
- 产品：{{product_id}}
- 卖点：{{usp}}
- 痛点：{{pain_points}}
- 平台：{{platform}}

## 指令
1. 围绕卖点/痛点生成 ≥5 条 Hook，每条 ≤15 字。
2. 标注使用的注意力机制（悬念/反常识/痛点共鸣/利益承诺）。
3. 给平台适配说明（TikTok/Reels/Shorts 差异）。
4. 每条提供 AB 变体。
5. 输出到 `06_Content/Hooks/`。

## 输出格式
- 文件：`YYYYMMDD_产品简称_hooks_vX.md`
