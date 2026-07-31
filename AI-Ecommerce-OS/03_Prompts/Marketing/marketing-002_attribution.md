# 数据归因分析

- id: marketing-002
- version: v1
- owner_agent: Marketing_Agent
- status: active
- updated: 2026-07-31
- inputs: date_range, attribution_model
- outputs: 09_Analytics/Reports

## 目标
对销售与广告数据做归因，给出优化方向。

## 上下文注入
- 时间窗口：{{date_range}}
- 归因模型：{{attribution_model}}

## 指令
1. 汇总各渠道花费、转化、ROAS、CPA、CVR。
2. 按选定归因模型分配贡献。
3. 识别异常波动并预警。
4. 输出优化方向（关停/加预算/换素材/调受众）。
5. 结论回流 score.csv（投放反馈维度）。

## 输出格式
- 文件：`YYYYMMDD_attribution_vX.md` → `09_Analytics/Reports/`
