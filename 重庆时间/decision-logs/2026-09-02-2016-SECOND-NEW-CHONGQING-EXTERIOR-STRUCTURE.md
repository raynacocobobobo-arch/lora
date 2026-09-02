# 2026-09-02｜第二新重庆外部结构设定记录

- Project: **《重庆时间》**
- Topic: **RING-ORIENT-01 / CITY-03 外部结构设计**
- Status: `RECORDED / EXECUTION DIRECTION LOCKED`
- Related execution spec: `../docs/visual/2026-09-02-SECOND-NEW-CHONGQING-EXTERIOR-STRUCTURE-V1.md`

---

# 01｜Why this decision was needed

在 Spatial Environment V2 合并后，项目重新评估了此前的环境/KV出图层级。

确认：

- 旧 KV 可以继续提供画风、材质、灯光和赛璐璐渲染 DNA；
- 旧图不能再反向定义城市宏观地理；
- 应先建立一级城市资产，再回到剧情子场景；
- `RING-ORIENT-01 / CITY-03` 属于一级城市结构资产。

随后生成的第一版外部结构图出现明显问题：

- 把中央空域处理成巨大悬浮城市/核心圆盘；
- 使用了错误的 `22 km` 量级；
- 把环形结构解释成旋转/向心 1G 重力来源；
- 与 Spatial V2 的“主环半径约 1 km、环只定义拓扑、不定义人工重力来源”冲突。

因此用户要求：

> 完整读取设定，外部结构必须符合物理学和材料学逻辑。

之后进一步锁定：

> 沿用此前已确认的赛璐璐画风，同时加入陨石撞击历史与长期维护痕迹。

---

# 02｜Locked external-city reading

第二新重庆外观不得再读成“一整块厚重甜甜圈飞船”。

正确读取：

> **永久环形船坞骨架 + 大型城区舱段 + 小型附属工程模块 + 多尺度交通/服务/对接接口。**

尺度方向：

- 主环中心线半径约 `1 km`；
- 整体直径视觉量级约 `2 km`；
- 主要城市内部最大有效净空约 `200 m`。

这些是视觉/剧作尺度，不是施工级精确尺寸。

Hard lock:

> **环形只定义城市结构拓扑，不通过旋转产生人工重力。**

永久禁止恢复：

- `22 km diameter`；
- Stanford torus；
- centrifugal / inward gravity 1G arrows；
- 旋转环重力解释。

---

# 03｜Central void decision

环中央主要保持：

> **central shipyard / structural open volume**

允许：

- 少量跨空域运输连接；
- 维护桁架；
- 对接结构；
- 小型工程飞行器。

禁止：

- 中央悬浮城区；
- 巨型中央圆盘；
- 中央花园世界；
- 嘉陵江 = 环中央洞；
- 嘉陵江 = 中央自然河流/湖泊。

嘉陵江必须继续服从 Spatial V2：

> **位于环形城市内部城区体系中的连续、有限、百米级开放公共城市带。**

---

# 04｜Structural engineering direction

外部结构绘制优先建立受力逻辑，而不是装饰性硬表面细节。

Permanent Ring Backbone 推荐视觉语言：

- 分段箱梁；
- 空间桁架；
- 环向主承力梁；
- 大型节点框架；
- 冗余载荷路径；
- 模块接口；
- 位移/热胀补偿；
- 隔振和检修空间；
- 外部维护路线。

城市模块必须表现为：

- 不同年代；
- 不同尺寸；
- 不同接口代际；
- 可替换/可维护挂接；
- 长期扩建、翻修和维修形成的非均质城市。

---

# 05｜Materials decision

以下材料逻辑属于**工程可视化执行假设**，不自动升级为硬 Canon：

- 高载节点：钛合金/高强钢类结构语言；
- 大型轻质舱体/骨架：铝合金/铝锂合金类结构语言；
- 局部长跨加强：碳纤维复合材料类结构语言；
- 外壳：压力壳 + 隔热 + 辐射/微流星防护 + 可更换外板；
- 微流星/碎片防护可参考 Whipple-shield-like layered protection；
- 散热器：薄型热辐射工程面，不是厚装甲；
- 模块接口必须考虑位移容差、密封、振动、热胀和维护可达性。

核心视觉规则：

> **真正承力骨架在内部/节点，外部大面积白色面板主要表达气密、防护、热控和可维护蒙皮，而不是“每块板都是装甲主梁”。**

---

# 06｜Meteor impact + maintenance history

外观必须明确携带 T0 历史，但不表现正在撞击。

Locked chronology:

> **impact → emergency initial sealing → structural reinforcement → long-term maintenance**

撞击区必须同时读出多个时间层：

- 原始受损；
- 应急封堵；
- 后装结构加固；
- 后续长期维修与再次老化。

视觉元素：

- 不规则撕裂撞击坑；
- 多层外壳破坏；
- 外板翻卷；
- 暴露桁架；
- 烧蚀/黑化；
- 后装加强框；
- 异色替换板；
- 焊接/铆接/夹持式维修；
- 维护管线；
- 检测接口；
- 新旧维修件并存；
- 应急修补自身也已经老化。

城市整体状态：

> **受过重伤，但没有停止运行；不是修回崭新，而是在不断维修中继续生活。**

---

# 07｜Art-style lock

用户明确要求继续继承此前已确定的赛璐璐画风。

有效风格 DNA：

- serious cinematic cel-animation background art；
- hand-drawn architectural linework；
- 2–3 hard-edged cel-shading tiers；
- large shapes first, micro-detail second；
- simplified monumental industrial forms；
- restrained signage；
- low glossy reflection；
- low micro-greeble density；
- cold gray-blue / deep steel blue / aged off-white；
- 少量褪色工业红与安全黄；
- 成熟中国公共基础设施复古未来主义。

Primary render lesson continues from KV05:

> **large shapes first; micro-detail second.**

禁止把外部城市重新做成 photoreal 3D / dense hard-SF kitbash。

---

# 08｜Generated draft status

Associated generation:

- `gen_id: 20c61a92-d3d0-4d86-b9eb-e9e3ce9a76e4`

This image is retained only as discussion/provenance reference.

Status:

> **NOT an approved visual anchor.**

Reason:

- generated text/labels can be accidental;
- exact geometry still needs a cleaner redraw under the locked structural rules;
- textual engineering direction is now more authoritative than accidental image details.

---

# 09｜Next use

Future `CITY-03 / RING-ORIENT-01` generation must first read:

1. `SPATIAL-ENVIRONMENT-CANON-V2.md`;
2. `WORLD-ARCHITECTURE-CANON-V4.md`;
3. `VISUAL-ANCHOR-INDEX-V2.md`;
4. `docs/visual/2026-09-02-SECOND-NEW-CHONGQING-EXTERIOR-STRUCTURE-V1.md`.

Then inherit the approved cel-shaded style anchors without copying obsolete geometry.

The full reusable positive prompt and negative prompt are stored in the execution spec above.
