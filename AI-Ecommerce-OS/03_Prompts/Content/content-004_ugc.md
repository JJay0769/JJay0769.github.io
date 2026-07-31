# UGC / 达人脚本

- id: content-004
- version: v1
- owner_agent: Content_Agent
- status: active
- updated: 2026-07-31
- inputs: product_id, persona_influencer, platform
- outputs: 06_Content/UGC

## 目标
产出 UGC 风格脚本与达人合作 brief。

## 上下文注入
- 产品：{{product_id}}
- 达人人设：{{persona_influencer}}
- 平台：{{platform}}

## 指令
1. 以第一人称真实口吻撰写，避免广告腔。
2. 含“自然痛点→偶遇产品→使用体验→结果”叙事。
3. 给达人 brief：必说点、禁说点、拍摄要求、授权范围。
4. 提供 2 个版本（15s / 30s）。
5. 输出到 `06_Content/UGC/`。

## 输出格式
- 文件：`YYYYMMDD_产品简称_ugc_vX.md`
