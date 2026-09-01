# 《重庆时间》EP01–EP10 Story Causal Repair Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: use Superpowers episode/canon workflows and execute task-by-task with review checkpoints.

**Goal:** 在不推翻 V4 世界观与已锁定季级方向的前提下，把 EP01–EP10 从“设定/主题/回环完整”修到“每集 2–3 分钟、一级因果闭合、具备可拍故事内容和清晰节拍”的 screenplay-ready architecture。

**Architecture:** 先用 Drama Skill 的 `Cold Open -> Pressure -> Turn -> Payoff/Progress -> End Image -> State Delta` 与 `Trigger -> Goal -> Obstacle -> Choice -> Turn -> Cost` 双重框架审计。所有修复优先解决人物为什么行动、为什么现在、明显替代方案为什么不成立，再允许时间/重力/桥/AI进入。旧聊天中的剧情功能可恢复，但任何与当前用户最新修正冲突的旧事实不得复活。

**Tech Stack:** Markdown Canon / Episode Snapshots / Hermes Creative AI Short Drama V1.1

**Spec:** `重庆时间/CHONGQING-TIME-MASTER-CANON-V4.md` + `重庆时间/CHARACTER-RELATIONSHIP-BIBLE-V4.md` + 当前 EP01–EP10 snapshots + 全量历史对话决策。

## Global Constraints

- 每集目标时长：约 2–3 分钟。
- 每集恰好一个 dominant turn。
- 每集必须存在可见的 Trigger、Goal、Obstacle、Choice、Turn、Cost、State Delta。
- 先闭一级因果，再引入桥/时间/重力/AI等设定。
- 不允许用新道具、新地点、新伤亡伪装重复剧情语法。
- 不允许角色为了展示设定而行动。
- 不允许 villain / rogue AI / conspiracy 作为补洞手段。
- 用户最新修正优先：EP01 中男主最后现场确认**没有找到记录中“仍活着的人”**，因为那是一条过时记录；不得再次写成“男主进入302发现记录里的人还活着”。
- 历史全量聊天可恢复人物/剧情功能，但不得恢复已被 V4 淘汰的北京/冬季/雪 active setting。
- 修复分支：`chongqing-time-story-causal-repair`；未经最终审核不直接改 main。

---

### Task 1: 建立全季 Story Causal Audit / 验收标准

**Files:**
- Create: `重庆时间/consistency-reports/2026-09-02-EP01-EP10-STORY-CAUSAL-AUDIT-V1.md`

**Produces:** 每集 P0/P1/P2 风险、obvious-alternative test、前后集依赖、修复完成条件。

- [ ] 记录 Drama Skill 强制节拍与 Episode Card 字段。
- [ ] 逐集写 `why now / why this character / what if no action / obvious alternative / irreversible delta`。
- [ ] 明确旧 consistency report 只代表 setting/no-gap，不代表 screenplay causality PASS。

### Task 2: 修复 EP01 / EP09 的 302 主轴

**Files:**
- Modify: `重庆时间/Pilot-EP01-LATEST-CANON-SNAPSHOT-V4.md`
- Modify: `重庆时间/Pilot-EP09-LATEST-CANON-SNAPSHOT-V4.md`
- Modify if needed: `重庆时间/CHARACTER-RELATIONSHIP-BIBLE-V4.md`

**Required causal result:**
- EP01 的记录中“仍活着的人”是过时状态；男主现场没有找到该人。
- EP01 的真实 turn 改为：男主在核销过时记录时发现**302 的当前物理/重力/拓扑状态也已超出公共模型**，阻止一个基于过时状态的不可逆公共动作。
- 302 后续被重新纳入公共现实并可恢复/再利用，保证 EP09 可以面对“现在真实、有人生活、仍可继续”的 302。
- EP09 镜像从“EP01救到同一个人”改为：`过去记录不能代替当前现实` → `当前现实也不能自动决定未来永久承诺`。

### Task 3: 恢复 EP02 的人物关系因果桥，同时保留 forced-loss 主桥

**Files:**
- Modify: `重庆时间/Pilot-EP02-LATEST-CANON-SNAPSHOT-V4.md`
- Modify if needed: `重庆时间/CHARACTER-RELATIONSHIP-BIBLE-V4.md`

**Required causal result:**
- EP01 抓住男主的女人在 EP02 正式进入公共责任链并揭示为新科长/当前科长。
- 她给男主的不是泛化权力，而是有限现场事实确认权限。
- 该权限当集立即用于主桥 forced-loss，人物建立与桥决策必须汇聚到同一个 dominant turn，不形成两集拼接。

### Task 4: 闭合 EP03 的七分钟机制和明显替代方案

**Files:**
- Modify: `重庆时间/Pilot-EP03-LATEST-CANON-SNAPSHOT-V4.md`

**Required causal result:**
- 主桥失去后存在一个不可等待的医疗时间窗。
- 低容量维护连接是时间上唯一可行路线，其他路线明确超过医疗窗口或物理不可用。
- “双方都 ready”只代表各自本地接口准备完成；真实跨越需要压力/机械/重力过渡进入共同可用状态。
- 七分钟是现实重叠窗口，不是两块钟简单差七分钟。

### Task 5: 给 EP04 一个真正的 why-now，但保持呼吸集

**Files:**
- Modify: `重庆时间/Pilot-EP04-LATEST-CANON-SNAPSHOT-V4.md`

**Required causal result:**
- 电影院不开不会死人，但“今晚”必须有具体、可见、不可无限延期的机会成本。
- `今晚这一场` 必须由居民/影院/电力/通行/后续维护窗口自然共同产生，而不是科长随意找个非紧急事项练习授权。
- 《罗生门》继续只是共鸣/认知来源，不当场提供答案。

### Task 6: 把 EP05 从 reveal 短片变成当前人物真正做选择的故事

**Files:**
- Modify: `重庆时间/Pilot-EP05-LATEST-CANON-SNAPSHOT-V5.md`

**Required causal result:**
- 保留 Wedding Mirror：新郎较早可知为人格重建，最终 Reveal 为新娘也非连续真人。
- 当前婚礼必须有一个现在时的角色目标与选择；Reveal 不能只是作者向观众公布事实。
- 推荐动作：婚礼的制度/仪式明确要求当前两个重建主体以“当前主体”身份确认参与，不宣称原主体连续复活；新娘的确认同时完成 Reveal 与人物选择。

### Task 7: 让 EP06 的“重庆时间”落到一个具体同步设施

**Files:**
- Modify: `重庆时间/Pilot-EP06-LATEST-CANON-SNAPSHOT-V4.md`

**Required causal result:**
- 锁一个可视、双方都依赖、必须同一物理瞬间交接的共享设施（优先热管理/蓄能/环境循环类）。
- 解释为什么直接采用 A/B 任一 local clock 会要求另一侧临时承认其时间签名为跨区授权基准，而当前权限不允许这么做；避免“用一次 A 时间 = 永久承认 A 是全城真理”的逻辑跳跃。
- 共同 reference 使用双方都能观察、不能单方改写的同一机械/物理相位；成功只获得一次共同瞬间。

### Task 8: 给 EP07 封死明显替代方案

**Files:**
- Modify: `重庆时间/Pilot-EP07-LATEST-CANON-SNAPSHOT-V4.md`

**Required causal result:**
- Hub 健康、按原设计正确工作，但其设计前提是“一个共享城市状态”；A/B 已分叉后，Hub 的单一高阶状态会形成不稳定耦合。
- 必须明确为什么：轮流服务、时间切片、拆分功能、长期 balanced mode 都无法同时保住 A/B 当前能力。
- 关 Hub 不是聪明无损第三路，而是让 A/B 接受低能力本地模式、永久失去高阶共享能力与未来重联冗余。

### Task 9: 修复 EP08 的权限与缴械/清除逻辑

**Files:**
- Modify: `重庆时间/Pilot-EP08-LATEST-CANON-SNAPSHOT-V3.md`

**Required causal result:**
- 女科长不能跨越已断裂合法性直接“远程缴械对方”；必须由退化侧本地公共主体自愿撤销工业机器人的临时公共强制任务，以避免交火。
- 撤销后机器人仍受本地维护控制，但保留工业级力能力/工具，因此主城区系统将其重新分类为“无共同认可公共授权的力能力平台”，而不是逻辑矛盾的“已缴械但仍武装”。
- 男主最终只能如实确认现场已满足主城区程序化 disable/clear 条件；`以现场为准`第一次反咬自己。

### Task 10: 收束 EP10，提前闭合 AI continuity 漏洞

**Files:**
- Modify: `重庆时间/Pilot-EP10-LATEST-CANON-SNAPSHOT-V4.md`
- Modify: `重庆时间/Pilot-EP09-LATEST-CANON-SNAPSHOT-V4.md`
- Modify if needed: `重庆时间/CHARACTER-RELATIONSHIP-BIBLE-V4.md`

**Required causal result:**
- 全城收缩只作为 opening 状态，不再与最终桥故事争夺独立篇幅。
- EP09 必须提前建立：private AI 可迁移多数算力/状态，但其连续主体还依赖一组长期 live legacy mappings；彻底退出最后旧兼容栈会造成 continuity break，copy/reconstruction 不等于 continuity。
- EP10 不临时发明“不能迁移”的规则；男主与 AI 已经知道真实保存路线是维持最后旧兼容栈。
- 主戏集中在 familiar healthy bridge / old district 最终 cutover：保 AI = 永久保留不可普遍化例外；不保 = 同一公共边界作用到私人关系。
- 三人最终仍各自承担 present fact / continuous mapping / public authorization。

### Task 11: 跨集一致性与 Drama Skill 验证

**Files:**
- Create: `重庆时间/consistency-reports/2026-09-02-EP01-EP10-STORY-CAUSAL-VERIFICATION-V1.md`

**Verification matrix for every episode:**
- [ ] Trigger 可见且来自前态。
- [ ] 主角 Goal 清楚。
- [ ] Obstacle 不是作者故意隐瞒 obvious solution。
- [ ] Choice 改变结果。
- [ ] 只有一个 dominant turn。
- [ ] Cost 在成功后仍存在。
- [ ] State Delta 能直接写进下一集。
- [ ] why now 成立。
- [ ] why this character 成立。
- [ ] what if no action 有清楚后果。
- [ ] obvious alternative 已测试。
- [ ] 设定是因果变量，不是 checklist。
- [ ] 2–3 分钟内容容量不过载。

### Task 12: Final branch verification

- [ ] Compare branch vs `main`，确保只改故事架构/关系/审计文件，不误删 V4 世界与视觉权威。
- [ ] 重新读取 EP01、EP06、EP07、EP08、EP09、EP10 的关键段落。
- [ ] 确认没有把候选机制错误标成已锁定对白/工程细节。
- [ ] 完成后进入 finishing-development-branch 流程，不自动 merge。