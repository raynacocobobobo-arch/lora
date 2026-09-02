# 《重庆时间》SPATIAL ENVIRONMENT CANON V2

- Updated: 2026-09-02
- Status: `LOCKED / ACTIVE SPATIAL + ENVIRONMENT CANON ON REPAIR BRANCH`
- Project: **《重庆时间》**
- City: **第二新重庆市**
- Scope: macro topology, environment geography, bridge scale, 302 position, EP01 detachment geometry, spatial blocking, visual-development reference
- Design basis: `docs/superpowers/specs/2026-09-02-second-new-chongqing-spatial-environment-v2.md`

---

# 00｜Core rule

> **第二新重庆是一座建立在永久环形船坞骨架上的模块化太空城市。**

整体近似不规则甜甜圈 / 环形船坞。

设计尺度方向：

- 主环半径约 `1 km`；
- 主要城市内部最大有效净空约 `200 m`。

这些是视觉/剧作尺度，不是施工级工程数字。

环形只定义城市拓扑，不定义人工重力来源。

---

# 01｜Three physical scales only

## A｜Permanent Ring Backbone

永久船坞/承力骨架。

- 支撑长期扩建；
- 允许城区舱段接入、替换、隔离；
- 第一季不通过切断主环骨架来表现“城市变小”。

## B｜District Modules

观众理解中的城区。

一个城区舱段可拥有：

- 街道；
- 住宅；
- 医院；
- 学校；
- 商业；
- 车站；
- 影院；
- 公共空间；
- 工业 / 服务区。

居民首先感到自己生活在城市，不是生活在设备舱。

## C｜Attached Service / Maintenance Modules

小型附属工程结构：

- 维修平台；
- EVA接口；
- 重力服务节点；
- 设备舱；
- 可隔离 / 可释放的接口段。

EP01最终意外脱离的是这一等级。

---

# 02｜Spatial readability rule

> **城市可以视觉多层，但角色行动不默认穿越多层城市。**

每集主动作原则上只需要：

> **一个主区域 + 一个明确连接 / 接口 + 必要时一个子空间。**

跨区域必须通过观众能理解的：

- 桥；
- 轨道；
- 舱门 / 接口；
- 维护连接。

禁止用“继续往上/下很多层”把角色抽象送到另一个城区。

---

# 03｜嘉陵江

`嘉陵江` 不是环形结构中央大孔洞。

> **嘉陵江是环形城市内部一条连续、有限、百米级的开放公共城市带。**

它沿城市弯曲延伸，两侧是可生活城区，中间/附近分布大量桥、轨道和共享设施。

居民自然使用：

- 过江；
- 江桥；
- 江这边 / 江对面；
- 临江；
- 上游 / 下游。

视觉铁律：

- 一眼能看到多种尺度连接；
- 空间大但有边界；
- 不是无限深渊；
- 不是“甜甜圈中央洞”；
- 不要求上方/下方无限叠城。

中央船坞大空域可存在，但不承担“嘉陵江”剧情地理。

---

# 04｜Bridge hierarchy — physical scale is not narrative importance

## Level 1｜Trunk Bridge

大型城市级复合连接：

- 重型轨道；
- 大规模人员；
- 物流；
- 能源 / 环境；
- 数据；
- Gravity Handoff；
- public/reference connection。

EP02嘉陵江主干桥属于此级。

## Level 2｜Regional Bridge

中等区域交通/服务连接。

## Level 3｜Utility Bridge

以能源、环境、数据和市政工程为主。

## Level 4｜Maintenance Bridge

小型维护连接：

- 技术人员；
- 小型运输架；
- 工业机器人；
- 应急少量人员/物资。

**EP03→EP04→EP08→EP10 的 Familiar Lifeline 物理上始终是 Level 4。**

它后来获得公共价值、排班、安保和终局意义，但不因此物理升级成大型区域桥。

> **生命线物理尺度很小，叙事尺度很大。**

---

# 05｜Trunk Bridge ↔ Lifeline topology

两者位于同一较大的跨区连接地理附近，但结构独立。

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

EP02主桥退出后：

- 远处仍可能有正常绕行；
- 绕行时间对EP03医疗需求来不及；
- 附近小维护桥因此成为唯一及时路径。

不是“全城只剩一座桥”。

---

# 06｜302 spatial lock

> **302 是挂接在主环外缘的一组旧城区舱段。**

空间关系：

- 朝城：正常生活 / 公共空间 / 区域交通；
- 朝外：旧服务、重力维护、附属工程接口；
- 最外侧邻接真空环境。

核心视觉类比：

> **一面朝城，一面临空。**

302内可包含：

- lived district；
- old public/cinema space；
- Gravity Service / legacy relay；
- outer maintenance interface。

这些是一个城区集群的子空间，不是多层城市穿越。

---

# 07｜EP01 — small accidental reverse-connection event

EP01空间动线：

> **normal city → 302 → 302 service/gravity area → small attached outer maintenance/interface segment → space**

现有故事因果保持：

- routine reset；
- partial handshake reveals trusted `+08:00`；
- gravity instability already active；
- full control succeeds；
- AI refuses lethal immediate restore；
- safe-reset Plan B genuinely begins working；
- new physical fact defeats the plan。

空间上的新物理事实锁定为：

> **男主所在的302外缘小型附属维护/接口段，在T0潜在旧伤与异常方向载荷共同作用下失去有效结构连接并意外断接。**

它视觉上类似“反向接桥 / 小尺度断接”，但不是系统主动把有人舱室弹射出去。

**302本体没有脱离。**

---

# 08｜Local Gravity Frames — visually simplified

Local Gravity Frames 保留。

但：

> **绝大多数可居住城区的 nominal down 在视觉上大体一致。**

观众不需要默认理解每个城区都旋转90度。

重力差主要在：

- 桥 / Gravity Handoff；
- 旧接口；
- 损伤服务区；
- 特定异常窗口。

第一季：

- ordinary district = stable；
- EP03/04/08 = Level 1–2 embodied transition；
- EP06/07 = gravity background / low weight；
- EP01 = primary Extreme vector-instability event。

时间与重力仍是独立故障轴。

---

# 09｜Shared infrastructure family

EP06/07 不新增一个独立“超级中央城区”。

共享基础设施存在于嘉陵江桥网/公共工程地理内。

EP06：

> shared thermal/environment node。

EP07：

> Shared Hub，属于同一共享工程家族，并控制跨区共享物理资源。

空间递进：

> 同一个城市连接体系里，EP06证明一次共同动作还能完成；EP07证明持续的单一共同高阶状态已经不能继续。

---

# 10｜Familiar Lifeline bridgehead staging

生命线本体保持狭窄低容量。

EP08主要冲突空间应落在：

- degraded-side bridgehead maintenance platform；
- better-resourced-side bridgehead；
- 两端之间的小维护桥；
- 小型 Gravity Handoff / interface。

退化侧工业人形机器人本来就在桥头负责维护，撤掉 public-force role 后仍不能无成本离开。

主城区中型四足公共安全平台从另一端接近。

不要把EP08画成巨型军事桥面会战。

---

# 11｜EP10 small-bridge capacity lock

EP09之后迁移已经开始，并在EP10开场前持续一段时间。

大部分居民通过当时仍开放的：

- 其他临时连接；
- 更远绕行；
- 低频公共转运；
- 分批迁移安排

完成离开。

随着城市收缩，这些连接逐步退出。

到EP10：

> **Familiar Lifeline 是最后仍 active 的旧兼容连接。**

它只承担：

- 最后一批人员；
- 维护/服务人员；
- 最后服务迁移；
- Gravity / time / protocol cutover。

“最后一座桥”指最后 active connection，不意味着整区人口在一集中全部挤过这条小桥。

---

# 12｜First-season spatial asset map

| EP | Main spatial asset | Change |
|---|---|---|
| EP01 | 302 + small attached outer segment | small accidental detachment |
| EP02 | Jialing Trunk Bridge | large forced connection loss |
| EP03 | small maintenance bridge near former trunk route | emergency public use begins |
| EP04 | same small bridge + ordinary legacy public space | temporary connection becomes life |
| EP05 | ordinary district / wedding space | no topology change |
| EP06 | Jialing shared thermal/environment node | one shared transaction |
| EP07 | Shared Hub in same infrastructure family | healthy shared-control role retires |
| EP08 | same small lifeline + bridgeheads | institutional conflict surface |
| EP09 | 302 as a complete lived district | current reality acknowledged; migration planned |
| EP10 | retained city ↔ same small lifeline ↔ 302 | last active legacy connection retired |

---

# 13｜Spatial character arc

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
EP10  small familiar healthy bridge becomes final active legacy connection and is deliberately retired
```

核心：

> **不是每集发明一座更大的桥，而是同一条小桥不断获得更多生活和公共意义。**

---

# 14｜Visual environment rules

1. 城市先读成一个有限环形整体，再读成工程细节。
2. 普通生活区必须像真实城市生活空间。
3. 200m是最大空间尺度感，不是多层穿越任务。
4. 嘉陵江大但有限，一眼可见桥梁尺度差。
5. 主干桥与小维护桥在体量上必须明显区分。
6. 302必须一眼读出“朝城 / 临空”双面关系。
7. 外部太空是稀有视觉状态，EP01因此有重量。
8. Local Time通过照明、班次、商店、医院、交通和行为节律显现，不靠多个太阳。
9. 普通城区 nominal down 大体统一；接口处再表现重力差。
10. 未来KV、环境概念图、分镜、剧本调度、场景生成提示词必须先读本文件。

---

# 15｜Priority visual-development assets

1. 环形城市整体外观 / orientation；
2. 环形城市“剪开拉直”的文字/视觉拓扑图；
3. 普通城区内部；
4. 嘉陵江宽景，多桥尺度同时出现；
5. 302整体：朝城面 vs 临空面；
6. EP02大型主干桥；
7. EP03/04/08/10小型生命线 + 两端桥头；
8. EP06/07共享基础设施家族；
9. EP01外缘附属维护段 + 意外断接几何。

医院、电影院、婚礼厅等属于这些母空间里的子场景，不升级成新的一级城市区域。

---

# 16｜Superseded spatial interpretations

以下不再是 active canon：

- 无限 / 近乎无底的内部巨构峡谷；
- 角色为到外壳而日常穿越许多叠层城区；
- 整座城市没有任何主导普通空间方向；
- 默认不同居住区彼此大角度翻转；
- `嘉陵江 = 环形结构中央大孔洞`；
- 生命线因社会重要而物理升级成大型Regional Bridge；
- EP01整个302被排出 / 系统主动弹射有人模块；
- EP10整区人口在正片中全部通过小生命线完成迁移；
- 通过切断永久主环骨架完成终局城市收缩。

这些只保留在Git历史作为创作过程，不得覆盖V2。
