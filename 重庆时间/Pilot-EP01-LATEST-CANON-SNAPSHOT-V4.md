# 《重庆时间》EP01 — TASK RECORD / GRAVITY CHOICE SNAPSHOT

- Updated: 2026-09-02
- Status: `LOCKED_DIRECTION / STORY + SPATIAL V2 RECONCILED / SCREENPLAY TBD`
- Project basis: `CHONGQING-TIME-MASTER-CANON-V4.md`
- World basis: `WORLD-ARCHITECTURE-CANON-V4.md`
- Spatial basis: `SPATIAL-ENVIRONMENT-CANON-V2.md`
- Character basis: `CHARACTER-RELATIONSHIP-BIBLE-V4.md`
- Outline basis: `EP01-STORY-OUTLINE-V1.md`
- Design spec: `docs/superpowers/specs/2026-09-02-ep01-task-record-gravity-redesign.md`
- Supersedes: **stale occupancy record → physical clearance → wrong cutover** as EP01 engine.

---

# 01｜Episode function

EP01 is the audience's first complete contact with **第二新重庆市**.

It must simultaneously:

1. show a damaged but functioning post-T0 city;
2. prove through one ordinary maintenance task that **local systems can all be working while the shared city reference is no longer whole**.

The episode is not about discovering a hidden resident and is not about proving 302 exists.

> **男主与私人 AI 进入 302 执行例行 Gravity Reference Reset。partial handshake 首次给出可信 302 本地时间，显示 `302 LOCAL = CHONGQING PUBLIC +08:00`；他们这才知道安全重置窗口早已过去，gravity re-lock / vector instability 已经开始。full handshake 最终成功，Gravity Control 可用，但 AI 判断此刻恢复 nominal gravity 会直接杀死已经被异常向量带离原位的男主，因此拒绝立即 restore，改为先利用错误重力把他送到外缘安全重置位置固定，再恢复完成原任务。Plan B 真的开始成功；随后 T0 潜在旧伤在异常方向载荷下扩展，使男主所在的 302 外缘小型附属维护/接口段失去有效结构连接并意外断接。302 本体没有脱离。任务由“完成工单”转为“让男主活下来”。AI 最终为维生关闭 local core；男主失去意识前，一只真实的人手抓住他。**

Episode-level dramatic question:

> **当“恢复正常”已经不再等于“现在最安全”，你是否仍然机械完成正确流程？**

---

# 02｜Opening — task record is the world-entry device

Target direction: first `0:00–0:45`.

观众从开场就知道这里是一座仍然正常生活的人工太空城市，但不做历史旁白。

## Ordinary city visuals

男主前往302时只需要自然看到：

- 环形船坞城市中的普通街区；
- 不同尺度的城市桥 / 轨道 / 服务连接；
- 正常通勤居民；
- 运行中的列车和公共服务；
- 桥侧日常维护；
- 不同城区略有差异的公共照明 / 服务节律；
- 已工程化处理、仍可见的 T0 修补痕迹。

不要求：

- 穿越多层城区；
- 上下无穷叠城；
- 大角度翻转城区。

城市不是末日废墟。

> **大灾难已经发生过；人们把城市救回来，并继续在里面生活。**

## Task record

任务纪录只给今天必须知道的信息：

> `SECOND NEW CHONGQING / CITY MAINTENANCE`
>
> `T0 AFTERMATH MAINTENANCE`
>
> `TARGET: 302 OUTER LEGACY DISTRICT / GRAVITY SERVICE`
>
> `LOCAL OPERATION: ACTIVE`
>
> `COMMON REFERENCE: DEGRADED`
>
> `LOCAL PUBLIC TIME: MAINTAINED`
>
> `LOCAL GRAVITY FRAME: MAINTAINED`
>
> `PUBLIC / LOCAL HANDSHAKE: REQUIRED`
>
> `TASK: GRAVITY REFERENCE RESET`
>
> `SAFE RESET WINDOW: ACTIVE`

Exact UI wording remains execution-level `TBD`; functions above are locked.

Audience understands normal ending:

> **握手 → 重置重力 → 窗口结束前撤离。**

## Male + private AI baseline

私人 AI 从第一场就在。

两人已经长期协作；不开“AI介绍场”。

开场通过熟练、生活化配合证明：

- 她参与他的工作；
- 她知道他的习惯；
- 两人熟悉此类维护；
- 彼此关系不以今天任务成功为条件。

可埋 `早安` 母题，给结尾回收。

---

# 03｜302 spatial lock / why male must enter

302 是：

> **挂接在第二新重庆主环外缘的一组旧城区舱段，一面朝城，一面临空。**

它不是一栋楼，也不是必须经过许多城市层才能到达的“地下区”。

302 内部有：

- 正常生活 / 公共空间；
- 旧 service / relay；
- Gravity Service；
- 外缘附属维护接口。

T0 后：

- 结构/接口曾受损；
- 一部分区域长期维修；
- Local Gravity Frame 为继续生活而本地维持；
- public/local time 依赖灾后 mapping；
- old relay / service 仍承担 legacy compatibility。

今天处理的是一个**已知、周期性、可维护**的重力 reference 问题。

Normal procedure:

> trusted public/local handshake
> → confirm current reference
> → reset / re-lock gravity reference
> → exit before hazardous re-lock window.

远程 handshake 无法通过最终 trusted-reference validation。

因此男主必须进入：

> **同一302城区内部的 old relay / Gravity Service area，建立当前真实物理节点到系统之间的可信桥接。**

私人 AI = protocol / historical mapping / model / control。

男主 = current physical node access / execution。

不是“AI不会按按钮”。

---

# 04｜Pressure 1 — routine job mostly works

进入302后不要立即灾难化。

前几个步骤顺利：

- access nodes pass；
- hardware alive；
- Gravity Controller responsive；
- identity / local service usable；
- only final trusted public/local handshake invalid。

Expectation:

> **再处理最后一个节点，任务就结束。**

Small drift evidence:

- condensation略有角度；
- 悬挂工具不完全垂直；
- 小物件缓慢向非预期方向偏；
- 男主体感到轻微 frame bias。

这只是已知问题的早期表现。

AI 的安全窗口仍依据最后可信的 `CHONGQING PUBLIC + last trusted mapping`。

> **她知道 302 time-domain mapping 不可信，但 handshake 完成前不能把未认证 local timestamp 当危险动作依据。**

AI 不是算错。

---

# 05｜Pressure 2 — partial handshake reveals +08:00

男主在旧 relay 建立当前 physical bridge。

AI 重启 handshake。

第一阶段只是 partial：

> enough local bus / safety / time authority becomes trusted;
> gravity actuation authority still unavailable.

302 local safety layer fragmented warning:

> `GRAVITY RE-LOCK...`
>
> `SAFE / EVACUATION WINDOW... EXPIRED...`
>
> `LOCAL GRAVITY VECTOR... UNSTABLE...`

然后首次可信比较：

> `CHONGQING PUBLIC  14:xx`
>
> `302 LOCAL         14:xx + 08:00`

`+08:00` direction locked.

Meaning:

> **不是还有几分钟；已经晚了八分钟。**

Correct causality:

> T0 leaves known gravity re-lock/reset vulnerability
> → 302 local time remains valid locally
> → trusted public/local mapping becomes stale
> → crew misjudges where the gravity cycle already is
> → partial handshake restores enough trusted local authority to reveal the hazard window is already active.

Time does not cause gravity failure.

---

# 06｜Pressure 3 — maintenance becomes evacuation

一旦 local warning 可信，男主立即撤离。

空间仍然是：

> **302 service/gravity path → 302 outer attached interface direction。**

不是穿越其他城区。

Gravity grammar:

> **vector instability / re-lock cascade**

Progression:

> subtle lean
> → strong lateral pull
> → previous floor unusable
> → debris/equipment change load direction
> → wall/ceiling becomes fall direction
> → outer-facing side becomes dominant “down”.

早期环境回收：

- temporary supports become hazards；
- loose equipment moves；
- exposed structure becomes handholds；
- pressure boundary requires visor seal。

每次成功动作只买到几秒，随后当前几何再次改变。

男主的 physical bridge 仍 live，所以 AI 在背景继续完成 handshake。

Two-front action:

- male = current physical survival；
- AI = reference/protocol/control path。

---

# 07｜Dominant Turn — full control succeeds, restore is lethal

男主已进入 302 外缘 Gravity Service / attached-interface direction。

Then:

> `HANDSHAKE COMPLETE`
>
> `GRAVITY CONTROL AVAILABLE`

False victory:

> handshake complete → restore → finish.

男主要求恢复 nominal gravity。

AI 不执行。

Reason:

- male displaced under abnormal vector；
- debris/equipment redistributed；
- temporary structures carry abnormal-direction loads；
- immediate nominal restore reverses load direction and drives male/debris back through the maintenance volume。

The one dominant turn:

> **目标从“现在恢复重力”改为“先把男主送到安全重置位置固定，再恢复完成任务”。**

AI不是选择永久异常重力。

Plan B 仍然是完整的 task-ending plan。

这同时锁定她的 independent agency：

> 当前安全状态使命令致命时，她可以拒绝男主的立即指令。

---

# 08｜Payoff — use bad gravity to reach safe reset

AI identifies one singular target:

> **302 outer attached interface / emergency reset securing position**

Exact hardware/name remains `TBD`.

Function:

- structurally intended to secure a worker during emergency Gravity Frame restoration；
- located on the small outer attached maintenance/interface segment；
- once male is secured, AI can restore nominal gravity and complete task。

Bad gravity becomes the route.

AI helps with route/timing/attitude/minimal EVA support。

男主 continuously supplies current physical geometry。

They reach the point.

Crucial lock:

> **He genuinely gets secured/caught by the emergency recovery system.**

The mechanism works.

Recovery genuinely begins.

AI prepares `RESTORE`.

Characters/audience believe original work order is about to complete.

A quiet work-like line such as `好了。` remains candidate dialogue, not locked.

---

# 09｜Cost after solution — attached segment loses connection

This is the episode's one true unexpected physical intervention.

Not:

- AI miscalculation；
- male error；
- tether simply breaks；
- battery failure；
- another protocol problem；
- system deliberately ejects an occupied module。

Locked function:

> **T0 left a latent fracture / interface scar inside the load path that attaches this small outer maintenance segment to 302. Prolonged abnormal-direction loading propagates it after Plan B has already started working. The attached segment itself then loses its valid structural connection and accidentally detaches.**

Chain:

> recovery mechanism worked
> → male secured
> → recovery began
> → current physical support/interface changed
> → attached segment disconnects.

This seeds:

> **方案正确 ≠ 结果保证。**
>
> **现场新事实有最后一票。**

AI still has `RESTORE NOMINAL` and reassesses.

Answer remains:

> **DO NOT RESTORE.**

Meaning differs:

- first no-restore = wait until secured；
- second no-restore = the safe reference itself is no longer connected to the city; restoring still reverses local loads without returning male。

This is Cost, not a second dominant turn.

---

# 10｜Outer-space transition

The small detached segment + male continue outward with acquired motion.

Once beyond 302 Local Gravity Frame's effective acceleration region:

> artificial acceleration falls away;
> acquired velocity remains;
> “向上坠落” becomes inertial drift.

No vacuum suction.

No explosion required.

External reveal should show a **readable ring-shipyard city**, not the superseded infinite layered megacity:

- curved ring-city mass；
- distinct district-module clusters；
- multiple bridge scales around the Jialing urban corridor；
- the visible scar / repaired surfaces of a long-used city；
- distant Earth only as subordinate external reference。

The reveal is not “surprise, they were in space.”

> **the ordinary city from the opening is seen from outside after one small connection has failed around one person.**

---

# 11｜Deceleration — AI can still help, cannot return him

After space transition, do not start a second action movie.

AI uses simple EVA capability:

1. stop/reduce uncontrolled rotation；
2. reduce outbound relative velocity。

Both genuinely succeed.

But the suit is not a return vehicle; remaining delta-v is insufficient.

Emotional state:

> **everything still possible is working; it is simply not enough.**

AI searches briefly for viable return/rescue path.

No drone/hoist/device failure cascade.

First AI wound:

> **correct reasoning can improve survival and still fail to guarantee a good outcome.**

---

# 12｜Power descent

Suit damage/increased life-support load makes shared power critical.

Exact medical/power numbers remain `VALIDATE_LATER`.

Plausible contributors:

- impact/concussion；
- degraded CO2 scrubbing/circulation；
- stabilized partial pressure loss；
- increased life-support draw；
- exhaustion/stress。

AI first shuts high-compute functions:

- external search；
- gravity modeling；
- high-rate trajectory simulation；
- nonessential sensing/reasoning。

She remains present after these go dark.

> **first she loses the ability to keep finding answers; only later does she choose to stop running at all.**

If male asks for another way, candidate direction remains:

> **“我不知道。” / “没有我能确认的。”**

Exact line `TBD`.

Final power trade:

> keeping `AI LOCAL CORE` alive measurably reduces remaining life-support time;
> shutdown maximizes `LIFE SUPPORT + MINIMUM RESCUE BEACON`.

AI is not converted into battery power; she stops consuming shared suit power.

This is local operational shutdown, not permanent continuity death.

---

# 13｜AI shutdown / dialogue

男主看见她准备关机，不希望她停。

No long optimality explanation.

Approved final direction:

> **“我很抱歉。”**
>
> **“祝你早安……晚安。”**

Then:

> `AI LOCAL CORE: SHUTDOWN`
>
> `LIFE SUPPORT: PRIORITY`
>
> `RESCUE BEACON: MINIMUM ACTIVE`

No dialogue after this point.

---

# 14｜End Image — physical hand

男主缓慢漂移，意识因伤势/维生下降而收窄。

Near black:

> **a real EVA-gloved human hand catches his wrist.**

Relative motion changes.

Second hand reaches chest rescue ring/tether.

Do not identify rescuer in EP01.

No early chief POV.

No line like “有人抓住你了。”

CUT TO BLACK.

EP02 reveals rescuer = current/new female chief.

> **all higher systems have fallen away; one person physically catches another.**

---

# 15｜Episode architecture audit

## Cold Open

> task record + ordinary ring city establishes world / relationship / normal task ending.

## Pressure

> routine mostly works → trusted handshake fails → partial handshake reveals +08 and expired window → evacuation through worsening gravity instability.

## Dominant Turn

> full control succeeds, but AI refuses lethal immediate restore; target becomes safe-reset first, restore second.

## Payoff

> bad gravity is exploited; male reaches the securing point; recovery genuinely begins.

## Cost

> latent T0 interface damage propagates; the small attached segment loses structural connection after success begins.

## End

> task completion impossible → AI prioritizes survival → EVA aid helps but cannot return him → compute descends → AI local core shuts down → human hand catches him.

Exactly one dominant turn.

`+08:00` = Pressure.

Detachment = Cost.

Final hand = Cliffhanger / relationship handoff.

---

# 16｜State Delta

1. Second New Chongqing is already in long-term post-T0 recovery; Local Operation is ordinary survival infrastructure.
2. 302 is an outer legacy district with a real time/gravity/protocol/interface scar.
3. Trusted public/local time mapping can fail while public and local systems keep functioning; `302 LOCAL = PUBLIC +08:00` becomes the first concrete trusted split.
4. Time mismatch does not cause gravity failure; it causes hazard-window misjudgment.
5. Male + AI are complementary: current physical bridge/execution vs protocol/model/reference/control.
6. AI independently refuses lethal immediate restore and proposes a complete safe-reset Plan B.
7. Plan B genuinely begins succeeding.
8. A new physical fact — the small attached outer segment losing connection — defeats task completion without making AI stupid or wrong.
9. 302 itself remains connected and available for EP04/09/10.
10. Male survives the space event only because AI repeatedly improves survival state and finally frees shared suit power.
11. AI local session shuts down; this is not permanent continuity death.
12. Unidentified human rescuer catches male; EP02 reveals her identity.
13. `DEBT_MALE_VALUE` remains open: field presence was genuinely necessary.
14. `DEBT_AI_KNOWLEDGE` opens: correct judgment can be defeated by newly revealed reality.
15. `DEBT_HAND_CONNECTION` opens.

---

# 17｜EP01 handoffs

## EP02

EP02 begins from rescue completion + incident review.

Chief reveal occurs there, not earlier.

Relationship split:

> male = present physical execute/abort fact;
> chief = public authorization/responsibility.

## EP09

Callback:

> **EP01: current physical reality can invalidate nominally correct procedure.**
>
> **EP09: after current reality is honestly acknowledged, it still does not automatically create permanent future public obligation.**

## EP10

302 chain:

> T0 time/gravity/protocol/interface scars
> → EP01 +08 / gravity / small outer detachment incident
> → continued repair / limited reuse
> → EP09 future-boundary trial
> → EP10 migration + legacy compatibility exit.

No stale occupancy/remap chain.

---

# 18｜Episode Card

```yaml
episode_id: EP01
target_duration: "3m30s–4m00s direction; exact screenplay runtime TBD"
episode_function: "普通302 Gravity Reference Reset工单暴露可信+08:00 public/local split；gravity instability已开始。full control成功后AI拒绝致命的立即restore，改走safe-reset-first Plan B。Plan B真实开始成功后，T0潜在旧伤使男主所在的302外缘小型附属维护/接口段意外断接；302本体仍在。任务让位于男主生存，AI最终关闭local core，未知人手完成救援。"
opening_hook: "仍正常生活的环形船坞城市里，男主与私人AI前往外缘旧城区302执行一张普通重力参考重置工单。"
dominant_turn: "HANDSHAKE COMPLETE / GRAVITY CONTROL AVAILABLE之后，AI判断立即恢复会杀死男主，拒绝restore并把目标改成先到安全重置位置固定。"
core_conflict: "正常流程终于重新可执行时，当前物理现实已经改变到继续执行正常流程反而更危险。"
conflict_grammar: "restored control authority vs changed present physical state"
progression:
  reveal_or_knowledge: "local systems can remain functional while shared public/local reference is stale; +08:00 is the first concrete crack"
  pressure_or_public_action: "routine maintenance becomes evacuation; task completion is ultimately abandoned"
  relationship_or_capability: "male=current physical execution; AI=protocol/model/control; AI proves independent judgment then loses capability layer by layer"
callback_or_debt: "302 legacy compatibility -> EP09/10; correct-judgment wound -> AI arc; physical hand -> EP02 chief reveal"
cost_after_solution: "safe-reset recovery truly begins, then the small outer attached segment loses structural connection; male is stranded outside and AI must shut down local operation for life support"
payoff_or_progress: "world premise and male/AI dependency are proven through one causal job"
ending_cliffhanger_or_image: "after '我很抱歉 / 祝你早安……晚安' and AI shutdown, an unidentified EVA-gloved hand catches the male's wrist"
mechanism_status: "LOCKED_DIRECTION / exact gravity hardware, interface engineering and suit power figures VALIDATE_LATER"
dialogue_status: "TBD except final apology/greeting direction locked"
state_delta:
  - "302 trusted local/public split +08 exposed"
  - "time and gravity remain independent"
  - "AI refuses immediate nominal gravity restore"
  - "safe-reset Plan B genuinely begins succeeding"
  - "small 302 outer attached segment accidentally detaches; 302 itself remains"
  - "male survives space drift"
  - "AI local session shuts down for life support/beacon"
  - "unidentified human rescuer catches male"
continuation_capsule: "EP02 opens after rescue. Incident review shows shared reference can fail while local systems continue. The rescuer is revealed as the current/new chief; AI shutdown was temporary/local, not permanent continuity death."
```

---

# 19｜Hard prohibitions

- no stale occupancy / hidden resident engine；
- no early chief reveal；
- no detached lore prologue；
- no multi-layer-city traversal to reach the exterior；
- no infinite internal canyon requirement；
- no time error directly causing gravity failure；
- no one-shot magical gravity flip as full escape grammar；
- no AI stupidity required for +08 reveal；
- no full handshake = automatic safe restore；
- no AI choosing permanent abnormal gravity as Plan A；
- no male simply slips from safe point；
- no recovery equipment failing before genuine success begins；
- no AI miscalculation as detachment cause；
- no deliberate system ejection of occupied segment；
- no whole-302 detachment；
- no vacuum suction；
- no post-space device-rescue cascade；
- no AI-as-battery language；
- no permanent AI death implication；
- no explanatory dialogue after final hand.
