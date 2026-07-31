# SOP04 — 内容生产

- 版本：v1
- 主导：Content_Agent
- 参与：Product_Agent、Demand_Agent、Competitor_Agent、Marketing_Agent
- 触发：选品立项后

## 目标
产出可投放、可拍摄的内容包。

## 流程
1. Content_Agent 接收卖点（Product）/痛点（Demand）/差异化（Competitor）。
2. 生成 Hook 库 → `06_Content/Hooks/`（≥5 条/产品，含 AB 变体）。
3. 生成视频脚本与分镜 → `06_Content/Videos/`。
4. 生成详情页文案 → `06_Content/Scripts/`。
5. 生成 UGC/达人脚本 → `06_Content/UGC/`。
6. 生成 CTA 库 → `06_Content/CTA/`。
7. Marketing_Agent 反馈数据后迭代内容。

## 产出
- `06_Content/` 各子目录文件
- 每条内容关联 product_id

## 验收标准
- Hook 前 3 秒抓人且有平台适配说明
- 视频脚本含分镜/口播/字幕/BGM
- 文案 ≥2 AB 变体
