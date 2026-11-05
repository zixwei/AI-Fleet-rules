---
name: zixwei-decisions
description: >-
  Every bot of zixwei MUST use this before any work, review, post, reply or
  factual answer, and whenever zixwei sets or changes a rule: read the shared
  decisions list and apply/sync it.
---
# zixwei 决定清单（所有 bot 必查）

清单文件：`/workspace/zixwei-decisions/DECISIONS.md`（由 ai总管 维护，备份在私有仓 shared/zixwei-decisions/）。

## 动手前（每次）
1. 用 Read 读清单，找出适用于自己和本次任务的条目。
2. 审稿、发帖、回答前逐条对照，不合规就改或拦下，不要只看格式。
3. 第 0 条严谨规则始终生效：先求证再回复；不模糊；已知未知分开；错了立即更正；结论和数据带出处；转述他人或其他 bot 的话前先核对原话；事实类问题按 fact-check-coverage 查全来源。
4. 清单和自己的记忆、职责说明、定时任务冲突时，以清单为准，并当场修正冲突处。标「待 zixwei 确认」的条目不当规则执行。

## zixwei 定了新规则时（当场）
1. 把新规则加进清单对应分区，写明日期、时间（ET）、适用哪些 bot、取代了哪条旧规则；旧规则移到「已作废」区。
2. 全文搜索自己的职责说明、定时任务 prompt、模板和 ROUTINE/RULES 文件，把冲突的旧口径全部改掉。
3. 如果规则涉及其他 bot，用 SendToAgent 通知它们同样处理。
4. 把改动的读回原文（改了哪些文件/定时任务、改前改后）直接报给 zixwei 验收。

## 维护
- 清单由 ai总管 负责整理和备份；其他 bot 改完可以同时告诉 ai总管。
- 每周一、周四约 05:00 ET 的自动优化时，ai总管 检查各 bot 的定时任务和模板是否还有与清单冲突的旧口径；已作废的旧条目在 /workspace/zixwei-decisions/DECISIONS-ARCHIVE.md，只在需要时查。
