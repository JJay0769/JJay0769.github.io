# 异常升级处理

- id: workflow-003
- version: v1
- owner_agent: CEO_Agent
- status: active
- updated: 2026-07-31
- inputs: alert_source, severity, context
- outputs: TODO.md, 人工确认请求

## 目标
对异常（数据暴跌/合规风险/供应链中断/平台封禁）做分级处理与升级。

## 上下文注入
- 告警来源：{{alert_source}}
- 严重度：{{severity}}     # P0/P1/P2
- 上下文：{{context}}

## 指令
1. P0（影响收入/合规）→ 立即暂停相关自动化，升级人工确认。
2. P1（影响指标）→ 24h 内出诊断与止损方案。
3. P2（观察项）→ 记入 TODO 待观察。
4. 所有处理记录写入 CHANGELOG。
5. 涉及重大决策走 CEO_Agent 的 escalation。

## 输出格式
- TODO.md 增加异常条目
- 必要时产出诊断报告 → `09_Analytics/Reports/`
