# 视频脚本分镜

- id: content-002
- version: v1
- owner_agent: Content_Agent
- status: active
- updated: 2026-07-31
- inputs: product_id, hook, duration, platform
- outputs: 06_Content/Videos

## 目标
产出可直接拍摄的视频脚本与分镜。

## 上下文注入
- 产品：{{product_id}}
- 选用 Hook：{{hook}}
- 时长：{{duration}}
- 平台：{{platform}}

## 指令
1. 按“Hook→痛点→解决方案→证明→CTA”结构编排。
2. 分镜表含：镜号/时长/画面/口播/字幕/BGM/道具。
3. 标注拍摄难度与所需素材。
4. 提供 2 个结尾 CTA 变体。
5. 输出到 `06_Content/Videos/`。

## 输出格式
- 文件：`YYYYMMDD_产品简称_script_vX.md`
- 分镜用表格
