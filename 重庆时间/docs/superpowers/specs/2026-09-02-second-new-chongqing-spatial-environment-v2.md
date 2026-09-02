# 第二新重庆空间环境架构 V2 — Design Spec

- Updated: 2026-09-02
- Branch: `chongqing-time-story-causal-repair`
- Status: `APPROVED DIRECTION / IMPLEMENTATION AUTHORITY FOR SPATIAL CLEANUP`
- Scope: city macro-topology, visual geography, bridge scale hierarchy, 302 position, EP01 detachment geometry, EP01–EP10 location continuity
- Purpose: provide one spatial model that both screenplay and visual development can use without reintroducing over-engineered or contradictory city geometry.

---

## 1. Core design objective

第二新重庆必须让创作者和观众都能稳定回答：

1. 人现在在哪；
2. 怎么去下一个地方；
3. 为什么这一处连接会成为剧情问题；
4. 哪些空间会在多集重复出现；
5. 哪些空间状态改变，而地点本身没有改变。

任何不能帮助这五件事的工程细节都不进入第一季 active canon。

---

## 2. Macro-form

> **第二新重庆是一座建立在永久环形船坞骨架上的模块化太空城市。**

Design-direction dimensions:

- 主环半径约 `1 km`；
- 主要城市内部最大有效净空约 `200 m`；
- 外形近似不规则甜甜圈 / 环形船坞；
- 环形只是建筑拓扑，不是人工重力产生机制。

主环骨架长期存在，第一季的“城市变小”不通过剪断主环承重主体实现。

城市通过减少、迁移、隔离附属城区舱段及其连接来收缩。

---

## 3. Only three physical scales

### A. Permanent Ring Backbone

- 长期承力 / 船坞骨架；
- 支持城市扩建和模块接驳；
- 不作为日常剧情场景；
- EP01–EP10 不以破坏主环为主要冲突。

### B. District Modules

观众理解中的“城区”。

一个大型城区舱段内部可以拥有：

- 街道；
- 住宅；
- 医院；
- 商业；
- 车站；
- 影院；
- 公共空间；
- 工业/服务区。

居民日常应首先感到自己生活在城市，而不是生活在一个设备舱里。

### C. Attached Service / Maintenance Modules

小尺度附属设施：

- 维护平台；
- EVA 接口；
- 重力服务节点；
- 小型设备舱；
- 可隔离或可释放的接口段。

EP01 最终脱离的是此等级，不是 302 区城体本身。

---

## 4. Jialing spatial definition

`嘉陵江` 不等于环形结构中心的大孔洞。

> **嘉陵江是环形城市内部的一条连续、有限、百米级开放公共空间带。**

它沿城市弯曲延伸，把不同城市带、公共设施和桥网组织在一起。

其空间特征：

- 一眼可看到多座不同尺度的桥；
- 两侧是可生活的城区体量；
- 中间包含共享公共/工程设施；
- 有明确结构边界，不是无限深渊；
- 居民自然使用“过江 / 江桥 / 江这边 / 江对面 / 临江”等城市语言。

甜甜圈中央大空域只是总体船坞/结构空域，不承担“嘉陵江”剧情地理。

---

## 5. Bridge scale hierarchy

桥是模块间的可识别连接，但必须区分**物理尺度**与**叙事重要性**。

### Level 1 — Trunk Bridge

大型公共复合连接，可承载：

- 轨道；
- 大规模人员；
- 物流；
- 服务；
- 环境；
- 数据；
- Gravity Handoff；
- public/reference connection。

EP02 的嘉陵江主干桥属于此级。

### Level 2 — Regional Bridge

中等区域交通/服务连接。

第一季不要求某一条 Level 2 成为核心角色资产。

### Level 3 — Utility Bridge

以能源、环境、数据和工程服务为主。

### Level 4 — Maintenance Bridge

小型维护连接：

- 维修人员；
- 小型运输架；
- 工业机器人；
- 应急少量人员通过。

**EP03→EP04→EP08→EP10 的 Familiar Lifeline 物理上始终保持 Level 4 / small maintenance bridge。**

它后来获得公共价值和制度意义，但不因此升级成大型 Regional Bridge。

核心定义：

> **生命线物理尺度很小，叙事尺度很大。**

---

## 6. Trunk Bridge and Lifeline relation

EP02 主干桥与 EP03 生命线应位于同一较大的跨区连接带附近，但结构独立。

Recommended topology:

```text
DISTRICT A                              DISTRICT B
████████                              ████████
   │                                     │
   ╞══════════ TRUNK BRIDGE ═════════════╡
   │                X EP02                │
   │                                     │
   ├──────── SMALL MAINTENANCE ──────────┤
                    ↑
               FAMILIAR LIFELINE
```

EP02 主桥退出后：

- 其他远距离正常绕行仍存在；
- 但医疗时限下绕行来不及；
- 同区附近的小维护桥因此成为唯一及时路径。

这样 EP03 不需要“全城只剩一座桥”的不可信前提。

---

## 7. 302 spatial lock

> **302 是挂接在主环外缘的一组旧城区舱段。**

它有两个方向：

- 朝城一侧：正常生活 / 公共空间 / 区域交通；
- 朝外一侧：服务、重力维护、附属工程接口，最终邻接太空。

空间类比：

> **一面朝城，一面临空。**

302 内部可以包含：

- ordinary lived district；
- old public/cinema space；
- Gravity Service / legacy relay；
- outer maintenance interface。

但这些是一个城区集群的不同子空间，不是角色要穿越多层城市。

---

## 8. EP01 spatial mechanism

EP01 行动路径：

> **normal city → 302 → 302 service/gravity area → attached outer maintenance module → space**

不是：

> normal city → many stacked districts → shell layers → space。

EP01 保留现有剧情因果：

1. routine Gravity Reference Reset；
2. partial handshake exposes trusted `+08:00`；
3. gravity instability has already begun；
4. full control becomes available；
5. AI refuses lethal immediate restore；
6. safe-reset Plan B genuinely begins working；
7. new physical fact defeats the plan。

Spatial V2 locks the final physical fact as:

> **男主所在的 302 外缘小型附属维护/接口段，在 T0 潜在旧伤与异常方向载荷共同作用下失去有效结构连接并意外断接。**

It is visually analogous to a reverse bridge operation, but is not a deliberate system ejection.

302 itself remains attached, inhabited and available for EP04/09/10.

---

## 9. Gravity simplification

Local Gravity Frames remain active canon, but spatial orientation is simplified.

> **绝大多数可居住城区的 nominal down 在视觉上大体一致。**

Local Gravity Frame differences are primarily felt at:

- bridge transitions；
- old interfaces；
- damaged service areas；
- abnormal event windows。

First-season visual severity:

- normal districts: stable；
- EP03/04/08: Level 1–2 embodied transition；
- EP06/07: gravity low-weight/background；
- EP01: only major Extreme vector-instability set piece。

Do not use “every district is rotated 90 degrees relative to the next” as default city geography.

---

## 10. Shared infrastructure / EP06–EP07

Do not create a separate giant central city district only for EP06/07.

Shared infrastructure exists inside / below the Jialing bridge-and-utility geography.

EP06:

> shared thermal/environment node between two local regions.

EP07:

> Shared Hub within the same infrastructure family, controlling shared physical resources that span both local states.

The audience should understand these as **things both sides physically depend on**, not as another new megacity zone.

---

## 11. EP08 bridge staging

The Familiar Lifeline remains small.

The main public-order confrontation should stage around the two **bridgehead maintenance platforms**, not as two armies facing across a giant bridge deck.

Degraded-side industrial humanoids must remain in their normal bridgehead maintenance area because removing them closes the bridge.

The better-resourced quadruped security platform approaches from the opposite bridgehead.

The narrow connection and constrained bridgeheads increase legitimacy pressure without turning the episode into military spectacle.

---

## 12. EP10 capacity rule

EP10 must not imply that the entire 302 population evacuates through a 3–5 m maintenance bridge in one episode.

Locked interpretation:

- migration starts after EP09 and continues before EP10 opening；
- earlier routes / temporary transit / longer detours carry the majority of residents during the broader contraction；
- those routes progressively retire；
- by EP10, the Familiar Lifeline is the **last active legacy connection**, carrying only final residents, maintenance staff and last service/cutover actions；
- its small physical scale remains believable.

“Last bridge” means **last active connection**, not “the only route ever used for migration.”

---

## 13. EP01–EP10 spatial map

| EP | Main spatial asset | Spatial state/change |
|---|---|---|
| EP01 | 302 + small outer attached module | small accidental detachment |
| EP02 | Jialing Trunk Bridge | large forced connection loss |
| EP03 | small maintenance bridge near former trunk route | one emergency shared action succeeds |
| EP04 | same small bridge + ordinary old-district public space | temporary route becomes daily life |
| EP05 | ordinary district / wedding space | no topology change |
| EP06 | Jialing shared thermal/environment node | one shared physical transaction succeeds |
| EP07 | Shared Hub in same infrastructure family | healthy shared-control role retires |
| EP08 | same small lifeline, mainly bridgeheads | local public orders collide |
| EP09 | 302 as complete lived district | current reality acknowledged; migration planned |
| EP10 | retained city ↔ same small lifeline ↔ 302 | last active legacy connection exits |

---

## 14. Season spatial arc

```text
EP01  small accidental detachment
   ↓
EP02  large trunk connection forced out
   ↓
EP03  insignificant maintenance bridge becomes useful
   ↓
EP04  useful bridge becomes ordinary life
   ↓
EP08  ordinary bridge becomes institutional boundary
   ↓
EP10  small familiar healthy bridge becomes final active connection and is deliberately retired
```

The season does not need a new spectacular bridge every episode.

Spatial meaning accumulates by reusing the same places.

---

## 15. Visual-environment design authority

This spatial architecture must be read before future:

- environment concept art；
- key visual development；
- storyboard / shot planning；
- screenplay blocking；
- location naming；
- Seedance/other scene generation prompts。

Required first visual assets:

1. ring-city overall exterior / orientation；
2. ring-city unrolled topology diagram；
3. ordinary district interior；
4. Jialing wide space with multiple bridge scales；
5. 302 whole-district orientation / city-facing vs space-facing relation；
6. EP02 Trunk Bridge；
7. EP03/04/08/10 small Familiar Lifeline + both bridgeheads；
8. EP06/07 shared infrastructure family；
9. EP01 outer attached maintenance segment and detachment geometry。

Sub-scenes such as hospital, cinema and wedding venue are downstream within these established spatial families.

---

## 16. Superseded spatial interpretations

The following are no longer active spatial canon:

- infinite / effectively bottomless internal megacity canyon；
- characters routinely traversing many stacked districts to reach an outer hull；
- citywide absence of a dominant ordinary spatial orientation；
- default image of entire districts rotated dramatically relative to each other；
- `嘉陵江 = torus central hole`；
- Familiar Lifeline physically upgraded into a large regional bridge because it becomes socially important；
- EP01 whole-302 ejection / deliberate module expulsion；
- EP10 entire 302 population funneling through the small lifeline during the episode；
- cutting the permanent ring backbone as the season-finale contraction mechanism。

Git history remains provenance; active docs must not repeat these as current facts.

---

## 17. Canon maintenance requirements

Implementation must reconcile, not merely overlay, the following active documents:

- `CURRENT.md`；
- `WORLD-ARCHITECTURE-CANON-V4.md`；
- `CHONGQING-TIME-MASTER-CANON-V4.md`；
- `Pilot-EP01-LATEST-CANON-SNAPSHOT-V4.md`；
- `Pilot-EP02-LATEST-CANON-SNAPSHOT-V4.md`；
- `Pilot-EP03-LATEST-CANON-SNAPSHOT-V4.md`；
- `Pilot-EP04-LATEST-CANON-SNAPSHOT-V4.md`；
- `Pilot-EP05-LATEST-CANON-SNAPSHOT-V5.md`；
- `Pilot-EP06-LATEST-CANON-SNAPSHOT-V4.md`；
- `Pilot-EP07-LATEST-CANON-SNAPSHOT-V4.md`；
- `Pilot-EP08-LATEST-CANON-SNAPSHOT-V3.md`；
- `Pilot-EP09-LATEST-CANON-SNAPSHOT-V4.md`；
- `Pilot-EP10-LATEST-CANON-SNAPSHOT-V4.md`；
- spatial scene-map document；
- any active causal patch that explicitly carries superseded spatial wording。

Old spatial patch/map documents should not remain active competitors after V2 consolidation.

---

## 18. Verification conditions

Spatial V2 passes only if all are true:

1. no active doc describes EP03 lifeline as a large/Level-2 bridge;
2. no active doc uses `EP01 remap 302` or stale-occupancy engine;
3. no active doc requires multi-layer city traversal for EP01;
4. no active doc treats Jialing as the torus central hole or infinite canyon;
5. EP01 explicitly loses only a small 302 outer attached segment;
6. EP10 explicitly preserves small-lifeline capacity plausibility through pre-episode migration;
7. Master season matrix reflects the repaired EP01 story;
8. Local Gravity Frames remain, but ordinary district orientation is visually stabilized;
9. `CURRENT.md` points future story and visual work to the same V2 spatial authority;
10. V1 spatial patch/map are removed or explicitly non-active so downstream agents cannot treat them as competing canon.
