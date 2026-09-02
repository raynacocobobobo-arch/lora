# 第二新重庆｜Seedance 2.5 图生视频 Prompt B

- Updated: 2026-09-02
- Project: **《重庆时间》**
- City: **第二新重庆市**
- Status: `ACTIVE PRODUCTION PROMPT / B MASTER ONLY`
- Source master: `2026-09-02-SECOND-NEW-CHONGQING-SEEDANCE-MASTER-B.md`
- Source image: `../../assets/visual/second-new-chongqing/SECOND_NEW_CHONGQING_SEEDANCE_MASTER_B.webp`

---

# 00｜Core production principle

User production intent:

> **Seedance receives the approved B source image + prompt.**

Therefore the prompt should not reconstruct the city from scratch.

Use this rule:

> **SOURCE IMAGE = geometry authority**
>
> **PROMPT = camera / motion / continuity / atmospheric authority**

The more architecture is re-described as “new”, the greater the risk Seedance will redesign the station across frames.

---

# 01｜Base image-to-video prompt

Use this as the default exterior prompt when the station itself is not undergoing a story-state change.

```text
Use the provided source image as the exact visual and structural ground truth for Second New Chongqing.

Preserve the same complete asteroid-centered ring city throughout the shot: same outer ring silhouette, same central engineered asteroid core, same general radial structural-link layout, same major old off-white district masses, same historical T0 impact/repair sector, same distant-Earth relationship and the same mature cel-animation industrial visual language.

Do not redesign, add, remove, multiply or reshape major station structures.

The station remains an old but operational orbital city. Very subtle practical lights and tiny maintenance activity may continue, but the architecture itself stays stable.

Keep the central asteroid visually stable as an irregular natural rock mass integrated into the central industrial collar. Keep the main radial links rigid and structurally consistent. Keep the outer ring continuous and recognizable.

Historical T0 damage remains old and reinforced: no active explosion, no spreading destruction, no new breakage.

Earth stays far away and small. Deep space remains calm and subordinate.

Motion should be cinematic, restrained and slow. Prioritize temporal consistency of the station over visual spectacle. Preserve the cel-shaded large-form rendering, simplified panel density and low micro-detail noise. No flickering window fields, no multiplying antennas, no crawling panel seams, no pipe growth, no truss mutation, no changing ring thickness.
```

---

# 02｜Chinese compact version

```text
严格以输入原图作为第二新重庆的结构母版，不重新设计空间站。整个镜头始终保持同一座完整环形轨道城市：外环轮廓不变、中央工程化小行星核心不变、主要径向结构总体位置不变、T0历史撞击/长期修复区位置不变、旧白/冷灰蓝/工业红配色不变、远处小地球关系不变。

空间站本身结构稳定，只允许极少量维护灯、微小工程活动和环境变化。不要新增环层，不要让主环忽粗忽细，不要让中央小行星变成金属球，不要增加密集辐条，不要新增大片建筑，不要让撞击区继续爆炸或扩散。

镜头运动缓慢、电影化、克制，优先保证时序一致性和大轮廓稳定。保持成熟赛璐璐科幻环境画风：大块面、2–3档硬边明暗、低微细节噪声、非写实3D硬表面。地球保持遥远且很小。
```

---

# 03｜Hard continuity phrases

When a shot tends to drift, append several of these rather than adding more descriptive detail:

```text
same exact station design
same ring silhouette
same central asteroid core
same radial-link layout
same impact-scar sector
same district massing
same camera-space orientation
no structural redesign
no new architecture
preserve source-image geometry
preserve source-image proportions
temporal structural consistency
stable macro silhouette
```

---

# 04｜Seedance anti-drift negative block

```text
no station redesign,
no shape mutation,
no extra ring,
no disappearing ring section,
no changing ring thickness,
no hollow center,
no asteroid transformation,
no metal-sphere asteroid,
no new giant structure,
no dense new spokes,
no multiplying docking arms,
no antenna growth,
no pipe growth,
no crawling panel seams,
no flickering window grid,
no new explosion,
no spreading damage,
no huge Earth,
no low Earth orbit,
no photoreal style shift,
no cyberpunk neon shift,
no mecha transformation
```

---

# 05｜Recommended camera modes

## A｜Safe establishing hover — safest

Prompt suffix:

```text
Wide establishing shot. The entire station remains inside frame. Camera performs a very slow stable hover with minimal lateral parallax. No roll. No rapid perspective change. The station remains structurally rigid and unchanged.
```

Use for:

- first reveal of Second New Chongqing;
- episode exterior punctuation;
- before/after state comparison;
- establishing EP10 intact-city state.

## B｜Slow cinematic push-in — safe

```text
Very slow cinematic push-in toward the complete station, keeping the entire ring readable for most of the shot. Minimal yaw, no roll, no aggressive zoom. Preserve all source geometry and landmark positions.
```

Use for:

- transition from cosmic scale toward city;
- opening narration / city-state montage;
- calm dread before crisis.

## C｜Slow lateral drift — safe/moderate

```text
Slow lateral camera drift with gentle parallax. Keep the station orientation almost fixed, with only subtle three-dimensional reveal. No fast orbit and no major rotation of the station.
```

Use for:

- showing ring thickness;
- showing outer service attachments;
- holding the T0 repair landmark in frame.

## D｜Gentle orbital move — moderate risk

```text
Gentle partial orbital camera move around the station, limited angle change, slow and smooth. Preserve the same ring geometry, asteroid core and radial structures. Do not reveal newly invented structures on the far side.
```

Only use when a slight additional 3D read is necessary.

---

# 06｜Avoid these motions from a single B source frame

High drift risk:

- fast 180°/360° orbit;
- aggressive camera roll;
- diving through a radial structure;
- moving from full-station view directly into a tiny docking hatch;
- rapid crash zoom;
- dramatic station rotation;
- complex multi-axis camera flight;
- asking the hidden far side to become fully visible;
- asking a major ring sector to move when no separate target state image exists.

If the screenplay requires one of these, create a dedicated source keyframe first.

---

# 07｜Motion hierarchy by shot scale

## Level 1 — full city exterior

Goal:

> recognition and structural stability.

Keep:

- entire ring;
- asteroid core;
- major radial links;
- T0 landmark;
- distant Earth.

Detail budget: LOW.

Best motion: hover / push-in / lateral drift.

## Level 2 — outer-ring sector medium-wide

Do not ask Seedance to crop B and simultaneously invent detailed architecture.

Recommended workflow:

1. derive a dedicated still from B / approved sector geometry;
2. simplify it for motion;
3. feed that image to Seedance.

## Level 3 — external engineering close shot

Use a dedicated close asset for:

- impact repair scar;
- docking hub;
- 302 outer edge;
- mechanical release locks;
- service-module detachment.

B remains the macro identity reference, not the direct close-up source.

---

# 08｜Lighting / atmosphere variations allowed without redesign

Safe changes:

- slow sunlight / rim-light movement;
- slight shadow travel over ring modules;
- very subtle maintenance lights;
- tiny distant maintenance craft;
- extremely subtle star parallax;
- slow Earth drift due to camera framing;
- limited warning lights in an active crisis sector.

Unsafe from the base master alone:

- whole-city lighting switching randomly;
- hundreds of windows turning on/off;
- massive thruster firing everywhere;
- asteroid surface breaking;
- damage spreading;
- ring opening/separating without target-state reference.

---

# 09｜T0 impact-sector continuity

Prompt block when the damage sector is visible:

```text
Preserve the same old T0 impact and long-term repair sector from the source image. It remains structurally damaged but stabilized and operational. Exposed deep structure, reinforced frames and red-brown repair modules stay in the same location. No active fireball, no new debris burst, no expanding crack and no additional catastrophic failure.
```

---

# 10｜Earth / orbital-distance continuity

Prompt block:

```text
Earth remains very distant and small, only a quiet scale reference. Do not enlarge Earth or make the station appear in low Earth orbit. Preserve the deep-space distance relationship from the source image.
```

---

# 11｜Style continuity block

```text
Maintain the exact visual language of the source image: mature cinematic cel-animation environment, simplified monumental industrial forms, illustrated architectural edges, broad hard-edged shadow groups, restrained aged off-white / blue-gray / industrial-red palette, low glossy reflection and controlled micro-detail. Do not transition toward photoreal NASA CGI, glossy game-cinematic hard surface, cyberpunk neon or anime character illustration.
```

---

# 12｜Reproduction fallback order

If a generated shot is unstable, simplify in this order:

1. reduce camera angle change;
2. remove new environmental activity;
3. remove tiny craft;
4. remove descriptive micro-details from prompt;
5. explicitly add `preserve source-image geometry`;
6. shorten the shot / split it into two source-keyframe shots;
7. create a dedicated new motion master for the required angle.

Do NOT fix instability by adding more architectural prose.

---

# 13｜Seedance handoff template

For each exterior shot, store:

```yaml
source_master: SECOND_NEW_CHONGQING_SEEDANCE_MASTER_B
source_asset: 重庆时间/assets/visual/second-new-chongqing/SECOND_NEW_CHONGQING_SEEDANCE_MASTER_B.webp
shot_id: TBD
shot_purpose: TBD
camera_mode: hover | push_in | lateral_drift | gentle_orbit
camera_speed: slow
major_state_change: false
must_preserve:
  - ring silhouette
  - asteroid core
  - radial links
  - impact-scar location
  - distant Earth relationship
allowed_motion:
  - subtle lighting shift
  - tiny maintenance activity
negative_drift:
  - no redesign
  - no ring mutation
  - no asteroid mutation
  - no new damage
prompt: |
  [base prompt]
  [shot-specific action]
```

If `major_state_change: true`, B alone is not sufficient; create/approve the target-state keyframe first.

---

# 14｜EP10 provisional note

The currently approved B master is an intact-city production baseline.

A possible future EP10 macro split / Legacy Sector release has been discussed but is **not automatically Canon merely because it is visually attractive**.

If approved later:

> prepare a dedicated `B-EP10-SEPARATION` keyframe pair (before / after or start / end) and animate between controlled state references rather than asking one B frame to invent the entire structural separation.

This is the preferred way to keep the station recognizable through a season-finale macro event.
