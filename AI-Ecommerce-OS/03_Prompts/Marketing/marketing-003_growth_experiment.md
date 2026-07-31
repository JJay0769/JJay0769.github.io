# 增长实验设计

- id: marketing-003
- version: v1
- owner_agent: Marketing_Agent
- status: active
- updated: 2026-07-31
- inputs: hypothesis, metric, duration
- outputs: 09_Analytics/Reports

## 目标
把假设转为可执行、可判定的增长实验。

## 上下文注入
- 假设：{{hypothesis}}
- 主指标：{{metric}}
- 周期：{{duration}}

## 指令
1. 明确假设、变量、对照组/实验组。
2. 定义主指标与护栏指标（防止副效应）。
3. 给样本量与显著性要求。
4. 给执行步骤与判定规则。
5. 实验后产出结论与是否全量。

## 输出格式
- 文件：`YYYYMMDD_experiment_主题_vX.md` → `09_Analytics/Reports/`
