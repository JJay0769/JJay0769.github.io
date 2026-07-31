# API 对接开发

- id: coding-002
- version: v1
- owner_agent: CEO_Agent
- status: active
- updated: 2026-07-31
- inputs: platform, endpoints[], use_case
- outputs: 08_Automation/API

## 目标
规范对接第三方平台 API（Shopify/Meta/TikTok/Google 等）。

## 上下文注入
- 平台：{{platform}}
- 端点：{{endpoints}}
- 用途：{{use_case}}

## 指令
1. 在 `08_Automation/API/` 产出对接说明：鉴权、限流、字段映射。
2. 给出请求/响应示例与错误码处理。
3. 凭证走环境变量，写入 `.env.example`。
4. 标注数据落库去向（04_Database 或 09_Analytics）。

## 输出格式
- 文件：`api-平台-用途_vX.md`
