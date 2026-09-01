# 《北京市没有冬天》SCENE PROMPT TEMPLATE V1.1

- Updated: 2026-09-01
- Status: `LOCKED / ACTIVE NON-CANON SCENE GENERATION TEMPLATE`
- Supersedes for visual execution: `SCENE-PROMPT-TEMPLATE-V1.md`
- Depends on: `VISUAL-CONSISTENCY-BIBLE-V1.1.md`
- Scope: KV / teaser / storyboard keyframe / environment-scene generation
- Default output ratio: **2.35:1**

---

# 00｜Core Rule

Do NOT begin by writing an image prompt.

Every scene generation must complete:

> **READ → CANON HANDSHAKE → DRAMATIC HANDSHAKE → VISUAL HANDSHAKE → PROMPT ASSEMBLY → GENERATE → TWO-LAYER QC.**

The prompt is the final translation layer, not the source of truth.

---

# 01｜Required Reading

Before writing a scene prompt, read:

1. `CURRENT.md`
2. `ACTIVE-DOCS-INDEX.md`
3. `BEIJING-NO-WINTER-MASTER-CANON-V3.2.md`
4. any active narrow Canon patch affecting the scene
5. the highest active Episode Snapshot for the relevant episode
6. `TRAILER-TEASER-V2.md` if the image belongs to the current teaser
7. `VISUAL-CONSISTENCY-BIBLE-V1.1.md`
8. this template
9. approved KV visual anchors available in the working context

If the active Episode Snapshot leaves scene-space execution `TBD`, older detailed episode documents may be consulted for execution provenance, but only where they do not conflict with the active snapshot.

If user instructions in the current conversation are newer than the repository, record them as explicit current-turn overrides before prompt assembly.

If the relevant Episode Snapshot or execution document has not been read, do not generate.

---

# 02｜Canon Handshake — mandatory

Fill this before every scene.

```yaml
scene_id:
episode_id:
execution_layer: teaser | kv | storyboard | screenplay-concept | other

canon_sources_read:
  - CURRENT.md
  - ACTIVE-DOCS-INDEX.md
  - active Master
  - relevant patch(es)
  - relevant Episode Snapshot
  - current execution doc
  - optional older detailed source used only for non-conflicting execution detail

current_turn_overrides:
  - # later explicit user instructions, if any

scene_function:
  # What must this image communicate in story / teaser terms?

physical_location:
  # Where exactly inside/outside the orbital city?

city_state_at_this_time:
  # What has already happened? What has NOT happened yet?

core_physical_fact:
  # Concrete visible event / abnormality.

public_system_state:
  # What systems are still operating / degraded / duplicated / isolated?

allowed_reveals:

protected_reveals:

characters_required:

objects_required:

objects_forbidden:

signage_required:

naming_override:
  # Current visual execution uses 第二新重庆 where explicitly required.

time_or_season_state:

weather_state:
```

Before continuing, summarize the Canon fact in ONE factual sentence.

If that sentence sounds like a different story, stop and re-read Canon.

---

# 03｜Dramatic Handshake — NEW V1.1

This stage prevents a visually correct image from depicting the wrong scene.

```yaml
primary_readable_action:
  # What should the viewer read FIRST in the frame?

core_conflict_in_frame:
  # What two pressures / realities are colliding here?

continuing_operations_required:
  - # 1–3 visible public / life / maintenance actions that continue despite the abnormality

scene_uniqueness_vs_existing_KVs:
  # Why is this space / action NOT just KV01 / KV02 / KV03 / KV04 with different props?

background_suppression:
  # What visually impressive background element must stay subordinate?

spatial_closure_rule:
  # For orbital interiors: where does the engineered volume visibly terminate or close?

first_read:
  # What should the eye understand in <1 second?

second_read:
  # What deeper abnormality / consequence should become visible after the first read?
```

Required test:

> **If the scene were shown without its caption, could a viewer still identify the intended action rather than only “a cool sci-fi place”?**

If no, redesign before prompting.

---

# 04｜Visual Handshake — mandatory

```yaml
aspect_ratio: 2.35:1
visual_bible: VISUAL-CONSISTENCY-BIBLE-V1.1

approved_anchor_priority:
  - KV-01 station
  - KV-02 wedding observation hall
  - KV-03 checkpoint
  - KV-04 opening connector bridge / bounded internal chasm
  - later approved anchors when added

composition_mode:
  # stable frontal / central axis / elevated wide / controlled alternative justified by scene action

space_type:
  # enclosed / semi-enclosed municipal megastructure / internal chasm / approved exterior / etc.

material_family:
  # aged blue-gray steel / old white municipal equipment / rigid metal signage

palette:
  # cold gray-blue / deep steel blue / aged white / restrained muted red

lighting_logic:
  # practical municipal lighting / controlled exterior spill / plot-required split lighting

rendering_language:
  # serious cinematic cel animation / defined linework / 2–3 hard shadow steps

municipal_continuity:
  # What makes this obviously the same civilization and equipment procurement system?

orbital_scale_check:
  # Why does this still feel like a finite engineered space-city volume rather than infinite open space?

anti_drift_notes:
  # Most dangerous genre-default temptation for this shot.
```

Generic `cyberpunk`, `space dock`, `NASA`, `sleek sci-fi`, `photoreal 3D render`, `epic sunset cityscape`, `infinite megastructure abyss` must NOT be used as positive style drivers.

---

# 05｜Fixed Master Visual Prompt Block

Use this as the stable visual base. Append scene-specific facts after it.

## Chinese working block

> 中国式公共基础设施复古未来主义的轨道巨型城市“第二新重庆”当前视觉执行体系。场景属于一座成熟、长期居住、持续维修和改造中的轨道城市，而不是崭新的宇宙飞船。公共基础设施具有厚重旧化的工业粗野主义结构和明确的市政秩序，但不同场景必须保留各自真实空间功能，不为了统一风格重复同一种大厅或中轴构图。优先采用稳定、可读的建筑透视，人物与移动设备相对于巨型公共结构较小。深钢蓝、冷灰蓝、旧白为主，少量暗红用于公共警告、标识或仪式性重点；厚钢板、焊缝、螺栓、接缝、补焊板、维修补丁、外露管线、检修平台、护栏、实际工作灯和长期使用痕迹。公共导视为有厚度、有边框、有固定件、轻微磨损的硬质工业金属牌，中文主标题配克制的小号英文副标题。白色或浅灰色公共交通、维护、清洁、安全设备属于同一套长期服役的市政设备家族，略旧、有维修痕迹，不做崭新概念车。严肃电影级赛璐璐动画，明确手绘线条边界，机械背景细密但有结构，2–3档硬边 cel shading，少软渐变、少 bloom、无炫耀性 lens flare。城市公共生活和维护必须继续运行，让异常状态与正常系统行为同时存在。轨道城市内部空间即使巨大，也必须保留人工包覆感、结构边界和有限体积，不能默认形成无限开放的太空船坞或无尽深渊。外部宇宙、星球、天空只作为从属背景。2.35:1。

### Naming note

`第二新重庆` is a current visual-execution signage lock, not an automatic rewrite of series Canon.

If the scene should not visibly name the city, omit the city name rather than inventing another one.

---

# 06｜Scene Variable Block — V1.1

```text
【场景名称】
...

【场景功能】
...

【物理位置】
...

【本镜头一眼可读动作】
...

【核心冲突】
...

【空间结构】
...

【空间封闭度 / 远景上限】
...

【核心异常】
...

【仍在继续的公共行为】
1. ...
2. ...
3. ...

【必须出现的设备 / 人物】
...

【公共导视文字】
...

【时间 / 季节 / 天气】
...

【与已批准 KV 的共同视觉 DNA】
...

【与已批准 KV 的场景差异】
...

【背景压制】
...

【镜头】
2.35:1；超大全景 / 大全景 / 中景；本镜头有理由的稳定构图；...

【剧情限制】
...
```

Every positive element must exist for one of four reasons:

1. Canon fact;
2. dramatic / shot function;
3. visual continuity;
4. environmental storytelling.

Do not add decorative spectacle merely because it is impressive.

---

# 07｜Global Negative Block — V1.1

> 不要泛赛博朋克，不要霓虹商业街，不要普通地表未来都市天际线，不要山河日落成为主视觉，不要 NASA 白色洁净空间站，不要光滑崭新飞船内饰，不要开放式太空船坞成为默认场景，不要无限深远且没有结构包覆的城市内部空间，不要密集吊机脚手架取代可读公共建筑结构，不要无意义 kitbash 堆砌，不要机甲大战，不要机器人暴走，不要废土垃圾场，不要全城锈蚀废弃，不要巨型全息广告，不要过量 bloom / lens flare，不要摄影级 3D 游戏截图接管赛璐璐语言，不要默认爆炸火球，不要默认大雨，不要随意加入雪，不要让星球、天空或宇宙风景压过城市公共空间，不要为了“视觉统一”复制前一张 KV 的房间和构图，不要为了“科幻感”改变已锁定的公共设备、导视和材质体系。

---

# 08｜Prompt Assembly Order

Final prompt semantic order:

1. visual world identity;
2. factual scene function / location;
3. **primary readable action**;
4. core conflict;
5. space geometry + **closure limit**;
6. composition / camera;
7. architecture / material continuity;
8. required municipal equipment / people;
9. **continuing public operations**;
10. signage exact text;
11. time / season / lighting / weather;
12. rendering language;
13. **background suppression**;
14. negative constraints.

Do NOT start with mood words such as `epic`, `cyberpunk`, `majestic space station`, or `cinematic sci-fi`; they tend to overpower the locked project language.

---

# 09｜KV-04 Provenance Example — updated after approval

KV04 is now an approved visual anchor. Its final scene truth is:

> **Inside the orbital city, a long-maintained city-scale opening connector bridge spanning a bounded industrial chasm is reaching forced mechanical separation while evacuation / transport and municipal systems are still operating.**

## Scene-specific locks

```yaml
scene_id: KV-04
episode_id: EP02
primary_readable_action: opening bridge is mechanically separating
core_conflict_in_frame: continue evacuation vs stop transmitting structural risk
continuing_operations_required:
  - evacuation / pedestrian movement
  - old white municipal transit or evacuation vehicles
  - maintenance / guidance systems still operating
scene_uniqueness_vs_existing_KVs: internal opening bridge over structural chasm; not station, ceremony hall or checkpoint
spatial_closure_rule: deep but bounded city cavity; visible enclosing walls / decks / internal service layers; no infinite abyss
background_suppression: distant depth and architecture remain subordinate to the bridge action; no planet / cosmic vista hero image
first_read: the bridge is opening while people / vehicles are still using the two sides
second_read: this is controlled forced loss after prolonged rescue, not a sudden explosion
```

## Important correction history

Rejected directions included:

- terrestrial city bridge / skyline;
- generic orbital construction yard;
- maintenance hall with two broken pipe-like structures;
- internal chasm so vast that it no longer felt physically plausible inside the space-city.

Approved correction:

> **reduce distant spatial depth until the space still feels monumental but clearly finite and enclosed inside the orbital city.**

---

# 10｜Two-Layer Generation QC

Before presenting any generated image, answer YES to all required items.

```yaml
layer_A_visual:
  same_orbital_municipal_civilization: yes/no
  matches_approved_KV_family: yes/no
  same_material_age_and_signage_family: yes/no
  same_municipal_equipment_family: yes/no
  correct_cel_animation_language: yes/no
  aspect_ratio_2_35_1: yes/no
  orbital_space_has_plausible_finite_volume: yes/no
  background_does_not_overpower_subject: yes/no

layer_B_dramatic:
  current_and_episode_read: yes/no
  correct_timeline_state: yes/no
  primary_action_is_immediately_readable: yes/no
  scene_conflict_is_present: yes/no
  required_continuing_operations_visible: yes/no
  spatially_distinct_from_existing_KVs: yes/no
  no_protected_reveal_leak: yes/no
  not_generic_scifi_spectacle: yes/no
```

Any major `no` means revise / regenerate before advancing the asset set.

---

# 11｜Anchor Promotion Rule

```yaml
anchor_candidate_if_approved: yes/no
anchor_adds_new_space_family:
anchor_adds_new_equipment_rule:
anchor_adds_new_scale_rule:
```

A generated image becomes a visual anchor ONLY after explicit user approval.

Current approved set:

- KV01 station
- KV02 wedding observation hall
- KV03 checkpoint
- KV04 opening bridge / bounded internal chasm

---

# 12｜Decision Provenance

V1.1 incorporates the 2026-09-01 visual-consistency and KV04 iteration conversation recorded at:

- `decision-logs/2026-09-01-2137-VISUAL-V1.1-KV04-CONVERSATION.md`
