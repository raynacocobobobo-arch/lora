# 《北京市没有冬天》SCENE PROMPT TEMPLATE V1

- Updated: 2026-09-01
- Status: `LOCKED / ACTIVE NON-CANON SCENE GENERATION TEMPLATE`
- Depends on: `VISUAL-CONSISTENCY-BIBLE-V1.md`
- Scope: KV / teaser / storyboard keyframe / environment-scene generation
- Default output ratio: **2.35:1**

---

# 00｜Core rule

Do NOT begin by writing an image prompt.

Every scene generation must first complete a **Canon Handshake**, then a **Visual Handshake**, then assemble the final prompt.

Execution order:

> **READ → EXTRACT FACTS → LOCK VISUAL ANCHORS → ASSEMBLE PROMPT → GENERATE → QC.**

The prompt is the final translation layer, not the source of truth.

---

# 01｜Required Reading

Before writing the scene prompt, read:

1. `CURRENT.md`
2. `ACTIVE-DOCS-INDEX.md`
3. `BEIJING-NO-WINTER-MASTER-CANON-V3.2.md`
4. any active narrow Canon patch affecting the scene
5. the highest active Episode Snapshot for the relevant episode
6. `TRAILER-TEASER-V2.md` if the image is part of the current teaser
7. `VISUAL-CONSISTENCY-BIBLE-V1.md`
8. this template
9. approved KV visual anchors available in the working context

If the relevant Episode Snapshot or active execution document has not been read, do not generate.

If user instructions in the current conversation are newer than the repository, record them as explicit current-turn overrides before prompt assembly.

---

# 02｜Canon Handshake — mandatory extraction sheet

Fill this before every scene.

```yaml
scene_id:
episode_id:
execution_layer: teaser | kv | storyboard | screenplay-concept | other
canon_sources_read:
  - CURRENT.md
  - MASTER
  - relevant patch(es)
  - relevant Episode Snapshot
  - current execution doc

scene_function:
  # What must this image communicate in the story / teaser?

physical_location:
  # Where exactly in the orbital city is this?

city_state_at_this_time:
  # What has already happened? What has NOT happened yet?

core_physical_fact:
  # The concrete event / abnormality visible in this frame.

public_system_state:
  # What systems are still operating, degraded, duplicated, isolated, etc.?

ordinary_life_continuing:
  # 1–3 concrete daily-life / maintenance actions still happening.

allowed_reveals:
  # What may the image show clearly?

protected_reveals:
  # What must the image NOT accidentally reveal?

characters_required:
  # none / tiny crowd / named character / action-specific

objects_required:
  # trains, maintenance vehicle, checkpoint units, ring, etc.

objects_forbidden:
  # plot-specific forbidden items in addition to global visual negatives.

signage_required:
  # exact Chinese wording if needed.

naming_override:
  # current visual execution uses 第二新重庆 where explicitly locked.

time_or_season_state:
  # e.g. left dusk / right night; winter / non-winter; neutral industrial interior.

weather_state:
  # explicit; do not invent rain/snow/fog without reason.

continuity_with_previous_approved_KV:
  # Which approved KV(s) carry the strongest style / equipment / signage reference?
```

The executing model must be able to summarize the scene in one factual sentence before continuing.

Example:

> **A long-maintained inter-district connection inside the orbital city is reaching irreversible structural separation while both sides and the maintenance system remain operational.**

If the sentence sounds like a different story world, stop and re-read Canon.

---

# 03｜Visual Handshake — mandatory style lock

Before prompt assembly, explicitly lock:

```yaml
aspect_ratio: 2.35:1
visual_bible: VISUAL-CONSISTENCY-BIBLE-V1
approved_anchor_priority:
  - KV-01 station
  - KV-02 wedding observation hall
  - KV-03 checkpoint
  - later approved anchors when added

composition_mode:
  # strict central axis / stable frontal / controlled alternative required by shot

space_type:
  # enclosed / semi-enclosed municipal megastructure / approved exterior

material_family:
  # aged blue-gray steel / old white municipal equipment / rigid metal signage

palette:
  # cold gray-blue / deep steel blue / aged white / restrained muted red

lighting_logic:
  # practical municipal lighting / controlled exterior spill / plot-required split lighting

rendering_language:
  # serious cinematic cel animation / defined linework / 2–3 hard shadow steps

municipal_continuity:
  # what makes this obviously the same public-system civilization?

anti-drift_notes:
  # what genre-default temptation is most dangerous for this shot?
```

For current work, generic `cyberpunk`, `space dock`, `NASA`, `sleek sci-fi`, `photoreal 3D render`, or `epic sunset cityscape` must NOT be used as positive style drivers.

---

# 04｜Fixed Master Visual Prompt Block

Use this as the stable visual base. Scene-specific facts are appended after it.

## Chinese working block

> 中国式公共基础设施复古未来主义的轨道巨型城市“第二新重庆”当前视觉执行体系。场景属于一座成熟、长期居住、持续维修和改造中的轨道城市，而不是崭新的宇宙飞船。超大型封闭或半封闭公共基础设施空间，厚重旧化的工业粗野主义结构，明确的城市公共系统秩序，严格正面或稳定建筑透视，优先中轴构图，人物与移动设备相对于空间尺度较小。深钢蓝、冷灰蓝、旧白为主，少量暗红作为公共标识、警告或仪式性色彩；厚钢板、焊缝、铆接/螺栓、接缝、补焊板、维修补丁、外露管线、检修平台、护栏、实际工作灯、长期使用痕迹。公共导视为有厚度、有边框、有固定件、轻微磨损的硬质工业金属牌，中文主标题配克制的小号英文副标题。白色或浅灰色公共交通、维护、清洁、安全设备属于同一套长期服役的市政设备家族，略旧、有维修痕迹，不做崭新概念车。严肃电影级赛璐璐动画，明确手绘线条边界，机械背景细密但有结构，2–3档硬边 cel shading，少软渐变、少 bloom、无炫耀性 lens flare。城市公共生活与维护必须仍在继续，让异常状态与正常系统行为同时存在。2.35:1。

### Important

The term `第二新重庆` in this block is the **current visual-execution signage lock**, not an automatic rewrite of all Canon documents.

If a scene should not visibly name the city, omit the signage rather than inventing another name.

---

# 05｜Scene Variable Block

After the fixed master block, add only facts required for the current scene.

```text
【场景名称】
...

【场景功能】
...

【空间结构】
...

【核心异常】
...

【仍在正常运行的细节】
1. ...
2. ...
3. ...

【必须出现的设备/人物】
...

【公共导视文字】
...

【时间 / 季节 / 天气】
...

【镜头】
2.35:1；超大全景 / 大全景 / 中景；正面中轴或本镜头批准的稳定构图；...

【剧情限制】
...
```

Do not add decorative elements merely because they are visually impressive.

Every positive element should have one of four reasons:

1. Canon fact;
2. shot function;
3. visual continuity;
4. environmental storytelling.

---

# 06｜Global Negative Block

Append the following negative logic unless a specific approved scene requires an exception.

> 不要泛赛博朋克，不要霓虹商业街，不要普通地表未来都市天际线，不要山河日落成为主视觉，不要 NASA 白色洁净空间站，不要光滑崭新飞船内饰，不要开放式太空船坞成为默认场景，不要密集吊机脚手架取代可读的公共建筑结构，不要无意义 kitbash 堆砌，不要机甲大战，不要机器人暴走，不要废土垃圾场，不要全城锈蚀废弃，不要巨型全息广告，不要过量 bloom / lens flare，不要摄影级 3D 游戏截图质感，不要默认爆炸火球，不要默认大雨，不要随意加入雪，不要让星球、天空或宇宙风景压过城市公共空间，不要为了“科幻感”改变已锁定的公共设备、导视和材质体系。

---

# 07｜Prompt Assembly Order

Final generation prompt must follow this semantic order:

1. **visual world identity** — fixed master block;
2. **scene function / location**;
3. **core physical fact**;
4. **composition and camera**;
5. **architecture and material continuity**;
6. **required public equipment / people**;
7. **ordinary life still continuing**;
8. **signage exact text**;
9. **time / season / lighting / weather**;
10. **rendering language**;
11. **negative constraints**.

Do NOT start with mood adjectives such as “epic”, “cyberpunk”, “cinematic sci-fi”, “majestic space station”, because they tend to overpower the locked project language.

---

# 08｜Scene Prompt Example — KV-04

This example is an execution translation of current Canon and the Visual Bible; it is not a new Canon definition.

## Canon facts

- EP02 occurs after the meteor impact, during prolonged rescue / support / repair;
- everyone is still trying to save and reconnect as much as possible;
- a long-maintained inter-district structure is nearing the point where continued support threatens larger stability;
- the final structural form remains execution-level design, but the frame must show prolonged repair, real connection function, and approaching irreversible loss;
- no explosion;
- both sides continue operating.

## KV-04 prompt block

> 使用《VISUAL-CONSISTENCY-BIBLE-V1》固定视觉体系：第二新重庆当前视觉执行中的轨道巨型城市公共基础设施，2.35:1，严肃手绘赛璐璐电影感，正面中轴超大全景。场景是封闭/半封闭的“跨区连接大厅”：左右不是两座独立城市，也不是裸露太空船坞，而是同一座轨道巨城内部两侧巨大的公共城区结构体。中央是一条长期承担人员通行、城市轨道、物流与大型公共管线的重型复合连接脊柱。陨石灾后它已经被连续支撑和维修很久：能看到多代补焊钢板、液压临时支撑、加固桁架、外接粗电缆与管线、局部气密结构、检修平台和少量维修机器人，但整体结构仍清晰、厚重、可读，不要脚手架堆满画面。
>
> 核心异常只发生在中央连接处：两端结构和公共照明仍然正常，部分维护设备仍工作，但中央连接脊柱已经产生明显、缓慢、不可逆的几米级错位；两段轨道轴线开始对不上，粗管线被拉伸，临时支撑承受异常载荷。它还没有爆炸，也不是刚刚被撞断；第一眼应读到“已经被救和撑了很久”，第二眼才发现“这条连接正在真正失去”。
>
> 画面保留日常仍在运行：少量巡检人员继续检查，小型白色旧式维护车停在仍可使用的轨道段，一台维护机器人继续工作，远处公共指示灯和局部物流系统仍亮。人物非常小，空间压倒人物。
>
> 公共导视使用前三张 KV 同一材质体系的蓝色硬质工业金属牌，可写“第二新重庆市 / 跨区结构维护段”，下方小字“临时支撑运行中 / 通行能力 37%”；文字作为真实公共设施信息，不做巨型装饰口号。
>
> 色彩以冷灰蓝、深钢蓝、旧白和暖白工作灯为主，只允许少量暗红告警灯。不需要左右黄昏/夜晚切分，不下雨。若远处存在宇宙或轨道外部，只作为很小的空间背景提示，并由建筑结构框住，绝不能成为星球奇观主视觉。
>
> 不要赛博朋克，不要地表重庆高楼天际线，不要山、河、太阳主视觉，不要开放太空船坞，不要泛 NASA / 航天基地，不要写实 3D 概念设计，不要机甲，不要大型吊机群，不要爆炸，不要随机断裂，不要让维修结构比公共建筑本体更抢画面。

---

# 09｜Generation QC Checklist

Before presenting a generated image, answer YES to all required items:

```yaml
canon:
  current_and_episode_read: yes/no
  correct_timeline_state: yes/no
  no_protected_reveal_leak: yes/no

world:
  same_orbital_municipal_civilization: yes/no
  not_generic_spacecraft_or_cyberpunk: yes/no

visual:
  matches_approved_KV_family: yes/no
  2_35_1: yes/no
  stable_architectural_composition: yes/no
  aged_heavy_material_family: yes/no
  signage_family_consistent: yes/no
  equipment_family_consistent: yes/no
  serious_cel_animation_not_photoreal_3d: yes/no

storytelling:
  core_abnormality_readable: yes/no
  public_system_still_operating: yes/no
  ordinary_life_or_maintenance_continues: yes/no
  no_generic_explosion_shortcut: yes/no
```

Any `no` on a scene-critical item means the image should be revised / regenerated before it is treated as an approved asset.

---

# 10｜Approval and Anchor Promotion

A generated image is NOT a new visual anchor merely because it was generated.

Only explicit user approval promotes it into the working anchor set.

Workflow:

> **generate → self-QC → user review → explicit approval → anchor promotion.**

Rejected, superseded, or style-drift generations must never become reference sources for later prompts.

This prevents visual drift from compounding across generations.

---

# 11｜Current Next Action

Use this template and `VISUAL-CONSISTENCY-BIBLE-V1.md` to regenerate:

> **KV-04 / EP02 slow inter-district structural separation.**

Once KV-04 is explicitly approved, use KV-01 + KV-02 + KV-03 + KV-04 as the active visual anchor set for subsequent scene generation.