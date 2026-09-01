# 《北京市没有冬天》VISUAL PATCH V1.1.1 — KV05 / CEL SIMPLIFICATION

- Updated: 2026-09-01
- Status: `LOCKED / ACTIVE NON-CANON VISUAL EXECUTION PATCH`
- Parent standards: `VISUAL-CONSISTENCY-BIBLE-V1.1.md`, `SCENE-PROMPT-TEMPLATE-V1.1.md`
- Scope: large environment/KV setting images; first locked by approved KV05
- Canon impact: NONE

---

# 00｜Why this patch exists

KV05 first drifted toward a dense photoreal / premium-3D concept-art look: too many pipes, micro-lights, small screens, tiny panels, windows, labels and reflective metal details competed at once.

The corrected KV05 became successful only after aggressively simplifying visual density while preserving the same municipal world.

Therefore this patch locks the following production rule:

> **少一点设计炫技，多一点空间逻辑；少一点写实复杂度，多一点赛璐璐结构感。**

For current large-setting KVs, visual richness must come primarily from **large structural relationships, functional spatial hierarchy, hard cel-shadow masses and municipal continuity**, not from micro-detail accumulation.

---

# 01｜KV05 approved visual anchor

KV05 is now an **APPROVED VISUAL ANCHOR**.

Scene family:

> **EP07 A / B / shared public Hub — large orbital-city interior public-infrastructure setting.**

Core readable structure:

- central shared Hub is the dominant mass;
- A-side and B-side public infrastructure connect visibly to it;
- one side may operate at higher capability while the other is visibly degraded;
- the relation is understood from architecture, light, activity and service state before signage is read;
- people / municipal vehicles remain scale references rather than image subjects;
- the space is huge but remains a finite engineered orbital-city interior.

KV05 joins current approved anchor set:

1. KV01 — dual-time / dual-state station;
2. KV02 — wedding public observation hall;
3. KV03 — public-security checkpoint;
4. KV04 — opening inter-district connector bridge over bounded internal chasm;
5. **KV05 — A/B/shared-Hub large public-infrastructure interior, simplified cel-megastructure language.**

---

# 02｜Large-setting Cel Simplification Rule — HARD

For large environment/KV setting images, default detail density must be lower than a realistic high-end sci-fi concept painting.

Prefer:

- large steel wall planes;
- large beams / columns / bridge decks;
- a few thick readable pipe groups instead of dozens of thin pipes;
- large equipment silhouettes;
- clear negative space between structural systems;
- 2–3 major cel-shadow tiers;
- large light/dark masses;
- restrained material highlights;
- a small number of meaningful signs;
- few but legible municipal vehicles / workers for scale.

Reduce or remove:

- decorative micro-panels;
- tiny blinking lights everywhere;
- dense window grids;
- excessive screens;
- excessive labels;
- hundreds of thin conduits;
- random kitbash layers;
- photoreal metal reflection noise;
- high-frequency greeble covering every surface;
- atmospheric depth used only to make the space look infinitely huge.

Working target:

> **When an image starts to feel like premium 3D hard-SF concept art, reduce micro-detail roughly 40–50% before adding anything else.**

This percentage is an execution heuristic, not a Canon number.

---

# 03｜Readability hierarchy

A large-setting frame should normally read in this order:

1. **major space relationship**;
2. **one dominant functional / dramatic state**;
3. **large equipment / circulation system**;
4. **municipal signage / status cues**;
5. **small people / vehicles / maintenance details**.

If the eye reads tiny pipes, lamps, screens or labels before it understands the scene, the image is too dense.

Rule:

> **One frame = one dominant spatial relationship + one dominant state.**

---

# 04｜Cel-animation rendering lock

Current successful large-setting rendering should prioritize:

- clear drawn edge hierarchy;
- simplified but confident mechanical contour;
- 2–3 hard-edged shadow bands;
- broad shadow shapes across walls / Hub / platforms;
- restrained gradients;
- minimal glossy reflection;
- minimal volumetric bloom;
- no ray-traced showroom material feel;
- no tiny light-field sparkle used as substitute for detail.

The frame should remain credible as a **serious hand-drawn / cel-animation production background**, not merely a 3D render with an anime filter.

---

# 05｜Material and equipment simplification

Keep the established city family:

- deep steel blue / cold blue-gray;
- aged white municipal shells;
- muted warning red;
- warm-white practical lighting;
- rigid blue public signage;
- used / maintained / repaired surfaces.

But simplify presentation:

- use fewer repair seams, each larger and clearer;
- use fewer exposed pipe bundles, each thicker and functionally grouped;
- show municipal vehicles as simple readable silhouettes;
- avoid designing every vehicle as a unique hero object;
- avoid covering every structural face with equal detail.

---

# 06｜State contrast should be structural, not textual

KV05 locks an important rule for A/B capability-state scenes:

> **Do not rely on a wall of explanatory signage to communicate state.**

Prefer state differences through:

- overall illumination level;
- number of active service lanes;
- transit frequency;
- open / closed service zones;
- visible operating machinery;
- partial darkness / reduced activity;
- large-scale power / service routing cues.

Signs may confirm what the image already communicates, but should not be required to understand it.

---

# 07｜Prompt patch for future large-setting KVs

Append this logic when generating major environment setting images:

> **大场景设定图采用简化赛璐璐巨构语言：优先巨大清晰的建筑块面、钢板、梁柱、桥面和少量粗管线，以2–3档硬边阴影建立体积；机械细节密度控制在可读范围，不用微小灯光、密集窗口、细管、屏幕、文字和高频金属反射堆“科幻感”。先让观众一眼读懂空间关系和核心状态，再看到车辆、人员、导视和维护细节。保持第二新重庆既有冷灰蓝/深钢蓝/旧白/少量暗红、市政设备和蓝色硬质导视体系。画面应像严肃手绘赛璐璐动画背景，而不是高密度写实3D概念图。太空城内部保持巨大但有限的人工体积。**

Negative addendum:

> **不要高频 greeble，不要每个表面都塞细节，不要密集小灯，不要大面积镜面金属反射，不要无数细管，不要用屏幕和标牌解释所有信息，不要无限层叠城市背景。**

---

# 08｜QC additions

For every future large-setting KV, add these checks:

```yaml
large_setting_cel_qc:
  major_shape_reads_before_micro_detail: yes/no
  one_dominant_spatial_relationship: yes/no
  one_dominant_scene_state: yes/no
  micro_detail_not_competing: yes/no
  hard_cel_shadow_masses_clear: yes/no
  photoreal_metal_reflection_suppressed: yes/no
  signage_confirms_instead_of_explains: yes/no
  finite_orbital_city_volume: yes/no
```

Any `no` in the first six items should trigger simplification before adding new content.

---

# 09｜Current working rule

For the present KV phase:

> **Only large scene / environment-setting KVs are being developed first. Character-action shots such as the EP01 fall-and-catch beat remain for later Shot Asset / Character Action development.**

This keeps the current asset phase focused on establishing reusable world spaces before character-action coverage.