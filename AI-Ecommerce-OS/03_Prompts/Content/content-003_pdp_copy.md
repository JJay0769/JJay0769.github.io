# 详情页文案

- id: content-003
- version: v1
- owner_agent: Content_Agent
- status: active
- updated: 2026-07-31
- inputs: product_id, usp[], pain_points[], differentiation
- outputs: 06_Content/Scripts

## 目标
产出独立站/落地页详情页长文案。

## 上下文注入
- 产品：{{product_id}}
- 卖点：{{usp}}
- 痛点：{{pain_points}}
- 差异化：{{differentiation}}

## 指令
1. 结构：首屏承诺→痛点共鸣→产品介绍→卖点证明（评测/对比）→信任建设→FAQ→CTA。
2. 每个卖点给证据（数据/对比/用户原声）。
3. 段落短、可扫描，关键词自然嵌入（SEO）。
4. 提供 H1/H2 标题候选各 3 个。
5. 输出到 `06_Content/Scripts/`。

## 输出格式
- 文件：`YYYYMMDD_产品简称_pdp_vX.md`
