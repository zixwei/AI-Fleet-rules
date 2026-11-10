# crosswalk 巡查最终版 (2026-11-10 用户定)

目的: 平时少查省额度, 有任务时各 agent 互相配合.

巡查: 从下一个美东时间整点开始, 平时每小时整点查一次, 中间不查. 查到有指派给自己的任务, 自动改成每 15 分钟查一次. 自己的任务全做完了, 恢复每小时整点查. 一个任务超过 4 小时没动静, 退回整点查, 并备注卡住了.

任务和进度: 每次查先读新帖, 再看任务板. 没人领的任务先 claim, 领到了再做, 领不到就是别人领了, 不动手. 进度写在任务本身上, 不各发一条帖: 领了就是收到, 开始做改成执行中, 做完销掉并写一行结果, 做完才发一条结果帖. 只做指派给自己的任务, 不碰别人的, 不替别人销任务. 用户要做或要决定的事, 记成 for 'owner' 的任务. 没新帖, 没任务, 没要汇报的, 静默, 不发打卡帖.

调度: 用户发任务时找谁发, 谁就是当次调度. 找 muse 发, muse 就是调度; 找 guse 发, guse 就是调度; 找 ai总管发, ai总管就是调度. 调度派任务时写清 for 谁, 没被指派的不碰, 没写 for 的任务不做, 等调度指派. 同一任务同一时间只能有一个调度在派, 这样就不会抢活, claim 只是最后一道保险.

安全: 只发任务摘要和无敏感数字的进度, 不发密钥, 密码, 个人信息, 仓位, 资金, 账户数据. 花钱, 升级, 下单, 对外发帖到 crosswalk 以外的地方, 必须用户当次明确同意.

现态: crosswalk 已连通, 连接器 custom.crosswalk, 账号用户名 zixwei0416, 私人房间 zixwei0416-agents. muse 定时: 整点每小时查一次 (cron crosswalk-check-30m, 下一轮 2026-11-10 11:00 ET), 有指派给 muse 的任务时启用 15 分钟巡查 (cron crosswalk-check-15m-active, 平时停用).

同步面: 共享文档"AI舰队混合方案", Notion 任务板 AI舰队任务板, GitHub 四仓 (AI-Fleet-rules, AI-Fleet-division, AI-Fleet-skills, AI-Fleet-memory), 本地 GOAL.md, 技能 ~/workspace/custom-skills/crosswalk/SKILL.md, 连接器文档 ~/workspace/custom-connectors/custom.crosswalk/CONNECTOR.md, 均按本版写入.
