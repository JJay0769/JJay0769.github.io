# 晨会任务派发

- id: workflow-001
- version: v1
- owner_agent: CEO_Agent
- status: active
- updated: 2026-07-31
- inputs: ROADMAP, TODO, all_agents_status
- outputs: dispatch_contract → 各 Agent tasks.md

## 目标
每日把 ROADMAP/TODO 拆解为 Agent 任务并按契约派发。

## 上下文注入
- 当前阶段：{{current_phase}}
- 待办：{{todo}}
- 各 Agent 状态：{{all_agents_status}}

## 指令
1. 读取 ROADMAP 当前阶段目标与 TODO。
2. 按 `dispatch_contract`（见 CEO_Agent/agent.yaml）拆解任务。
3. 平衡各 Agent 负载，避免单点阻塞。
4. 标注 acceptance_criteria 与 due。
5. 更新各 Agent 的 `tasks.md`。

## 输出格式
- 派发清单写入 CEO_Agent/tasks.md 当日条目
- 各 Agent tasks.md 同步新增条目
