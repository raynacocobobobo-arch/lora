# 《重庆时间》SCENE PROMPT TEMPLATE V3

- Updated: 2026-09-03
- Status: `ACTIVE / ATMOSPHERE-FIRST / IDENTITY-FIRST / SEEDANCE-READY`
- Supersedes: `SCENE-PROMPT-TEMPLATE-V2.md` for new major environment / atmosphere-image generation
- Canon basis: current user instruction + current Canon precedence + relevant Spatial patch + relevant episode outline/snapshot
- Visual basis: `VISUAL-CONSISTENCY-BIBLE-V2.md` + `VISUAL-STYLE-ROUTING-INDEX-V2.md` + **《重庆时间》押井守动画风格 V1**
- Default aspect: **2.35:1**

---

# 01｜Why V3 exists

Earlier failures were not mainly style failures. They came from the generation method collapsing a story-space into a generic visual object.

Observed failure modes:

1. **style-first drift** — old-white + rust-red + hard light looked correct, but the location itself became generic;
2. **label-first identity** — `302` text/signage was used to prove location instead of architecture/function doing the work;
3. **node = whole space error** — a technical node such as `old relay / Gravity Service` was enlarged into a sealed machine hall even when the episode's dominant action actually moved through a larger service route/spine;
4. **local-shot bias** — requests for a core environment were answered as one device / one room rather than an atmosphere master showing the whole spatial relationship;
5. **Seedance simplification too blunt** — detail was removed without distinguishing fragile micro-noise from scene-defining geometry;
6. **composition was under-specified** — prompts knew what objects existed but not what visual order should dominate the frame.

The successful direction is therefore:

> **先判断这张图是什么级别的图，再判断这一集真正持续承载动作的空间，再锁它的父空间和大结构，最后才套风格与 Seedance 压缩。**

---

# 02｜Natural-language trigger

When the user says any equivalent of:

- `重庆时间，按设定出图`
- `重庆时间，按设定出图，EPxx...`
- `按重庆时间设定出图`
- `按 GitHub 设定出这个场景`
- `做 EPxx 的核心空间`
- `做下一张环境母图 / 场景气氛图 / 大场景`
- `这个场景视觉化一下`

route through this V3 method automatically.

## Shot-mode trigger

If the user says:

- `核心空间`
- `场景气氛图`
- `环境母图`
- `大场景`
- `建立这个空间`

then default to:

> **ATMOSPHERE MASTER / WIDE ESTABLISHING ENVIRONMENT**

Do **not** default to a local device room, machine close-up or single functional node.

Only route to a local/partial view when the user explicitly asks for:

- `局部`
- `节点`
- `设备`
- `特写`
- `机房`
- `操作位`
- `桥头局部`

---

# 03｜Core-space interpretation rule

For episode requests such as `EP01 核心剧情空间`, do not choose the location merely because it is named most often or has the clearest noun.

Instead determine:

> **Which spatial geography carries the largest share of the episode's dominant physical action and must support the episode's main state change?**

Use three tests:

```yaml
runtime_coverage:
dominant_action_coverage:
state_change_coverage:
```

A small node may be important but still not be the core atmosphere space.

Example EP01:

- `old relay` = key handshake node;
- sealed Gravity Service room = possible local shot;
- **302 service/gravity path → outer-facing maintenance/interface route** = dominant action geography;
- therefore the atmosphere master should establish a larger **Gravity Service Spine / outer service void**, not a closed machine hall.

Rule:

> **核心剧情空间 = 承载主要动作变化的空间系统，不等于剧情里最醒目的设备名。**

---

# 04｜Generation order — hard lock

All major setting-art generation follows:

> **CANON → SHOT MODE → DOMINANT ACTION GEOGRAPHY → SCENE IDENTITY → PARENT SPACE → NARRATIVE AFFORDANCES → COMPOSITION → STYLE → SEEDANCE REDUCTION → PROMPT → GENERATE → QC**

Never begin from a style header.

Never begin from a cool object.

Never use signage to repair missing spatial identity.

---

# 05｜Scene truth block

Before prompt writing, resolve:

```yaml
episode_id:
shot_mode: atmosphere_master / local_functional_shot / action_keyframe
exact_story_phase:
scene_location:
dominant_action_geography:
scene_parent_asset:
entry_direction:
exit_or_next_space:
current_public_state:
current_gravity_state:
current_local_time_state:
reveals_allowed:
reveals_forbidden:
```

Then write one factual sentence:

> **This scene is [specific location/system], seen at [specific story phase], and the space must visibly support [dominant action/state change].**

If that sentence is generic, do not prompt yet.

---

# 06｜Scene identity gate

A scene must be identifiable without relying on text.

Define 2–4 **large semantic anchors**:

```yaml
anchor_1:
anchor_2:
anchor_3:
anchor_4_optional:
```

Good anchors are large physical facts:

- one dominant bridge span;
- a huge old freight/transfer frame;
- a broad Gravity Service engineering spine;
- exposed asteroid rock + dominant excavator;
- a shared thermal machine physically between two district interfaces;
- a compact two-bridgehead system around the same small lifeline.

Bad anchors are:

- lots of small signs;
- decorative pipe fields;
- random windows;
- generic people;
- generic sci-fi machinery.

Hard test:

> **If changing the sign can turn the image into another district, identity failed.**

---

# 07｜Parent-space continuity

Every atmosphere master must explain where it sits inside the city.

```yaml
parent_space:
position_inside_parent:
city_side_or_space_side:
visible_arrival_cue:
visible_departure_cue:
major_connector:
forbidden_old_geography:
```

The frame does not need to show every adjacent space, but it must preserve directional logic.

For route-based scenes, the viewer should feel a clear **toward**:

- toward city;
- toward Jialing;
- toward outer service edge;
- toward bridgehead;
- toward asteroid origin layer;
- toward retained city.

Avoid compositions that turn a directional route into a sealed box.

---

# 08｜Narrative affordance rule

Environment design should already contain the surfaces and structures that later action will use.

For each atmosphere master, define:

```yaml
future_action_affordance_1:
future_action_affordance_2:
future_action_affordance_3:
```

Example EP01 core geography should already contain:

- floor / wall / overhead surfaces that can change narrative meaning when gravity vector shifts;
- handrails / structural edges / securing points usable as handholds;
- temporary reinforcement that can later take abnormal load;
- a readable open void / lateral depth so gravity change creates real danger;
- a clear outward route toward the attached interface segment.

The environment should not look designed only for a still image.

> **母图不是背景板；它要预埋后面动作会用到的空间语法。**

---

# 09｜Atmosphere-master composition

For `核心空间 / 场景气氛图 / 环境母图`, default to a **wide spatial read**.

The frame should prioritize:

1. one dominant spatial relationship;
2. large void / mass relationship;
3. clear movement direction;
4. strong light-shadow organization;
5. tiny people / maintenance activity only as scale evidence.

Avoid:

- central hero machine taking most of the frame;
- one room filling the entire composition;
- close device detail;
- camera placed too near the subject;
- architecture cropped so tightly that parent-space relation disappears.

## Composition families

Choose one intentionally:

### A. Axial / center-symmetrical monumental

Use when the space is infrastructural, procedural, institutional or route-driven.

Characteristics:

- strong central vanishing axis;
- large bilateral structural masses;
- one central bridge / platform / route;
- tiny human scale;
- light source or bright depth centered / near-centered;
- calm severity rather than heroic spectacle.

This composition worked especially well for the 302 outer Gravity Service Spine exploration.

### B. Near-symmetrical with one controlled break

Use when the system looks ordered but the story contains asymmetry/damage.

- base geometry almost symmetrical;
- one repair scar, closed route, broken bridge, or unequal resource state interrupts it.

### C. Oblique structural panorama

Use when movement direction, bridge relationship or district-to-district geography matters more than institutional symmetry.

### D. Layered cross-space wide

Use for Jialing / shared infrastructure when two sides and one shared object must read simultaneously.

Do not use the same composition family for every environment.

---

# 10｜What the recent successful images got right

The recent 302 Gravity Service Spine atmosphere studies succeeded because they shared the following qualities:

- the frame showed a **whole spatial system**, not a local machine room;
- large off-white structural masses formed the image before details;
- deep open void gave the environment physical consequence;
- platforms and service spans established a clear route;
- human figures stayed very small and proved scale;
- rust-red operated as civic/repair structure, not decoration;
- directional warm light created large illuminated planes and large shadow blocks;
- center / near-center symmetry gave the infrastructure institutional order;
- the architecture felt capable of becoming dangerous when gravity changed;
- the image had atmosphere and story potential before any explanatory text.

These qualities are now part of the **generation method**, not a separate new art style.

---

# 11｜Style application

Only after scene truth and composition are locked, apply:

> **《重庆时间》押井守动画风格 V1**

Keep:

- aged off-white / warm off-white major structures;
- pale/cold gray secondary structures;
- charcoal/near-black deep structure and cast shadow;
- restrained muted rust-red repairs/civic bands;
- hand-drawn industrial structural linework;
- 2–3 hard-edged cel-shadow tiers;
- old / repaired / still-operational public infrastructure;
- quiet, severe, procedural mood;
- strong structural light.

Do not turn the style into one fixed color temperature.

---

# 12｜Seedance reduction V2 — preserve the essence, reduce the failure surface

The recent atmosphere studies are visually correct but still somewhat over-detailed for Seedance.

The fix is **structural compression**, not stylistic flattening.

## Preserve at full strength

- primary silhouette;
- central / dominant route;
- large structural frames;
- major open void;
- large wall planes;
- 1–3 main bridge/platform masses;
- major repair scar / rust-red band;
- light direction;
- large cast shadows;
- 1–3 scale figures.

## Simplify aggressively

- repeated side catwalks;
- dozens of small cross-bridges;
- dense background structural grids;
- repetitive tiny window/opening patterns;
- fine rails repeated across the whole frame;
- exposed micro-pipe networks;
- numerous small lamps;
- tiny signage;
- distant machinery that does not affect story.

## Depth compression

Use three readable depth bands:

> **foreground frame / main midground action architecture / simplified far mass**

Do not give every depth plane equal detail.

Far background should become:

- large vertical/horizontal masses;
- 2–4 key structural lines;
- one broad light value;
- very few lamps.

## Repetition rule

Repeated architecture must read as **rhythm**, not hundreds of individually resolved units.

Merge:

- rails into continuous edge bands;
- windows into larger dark openings;
- pipes into 1–3 thick service trunks;
- catwalk clusters into one clear service layer;
- tiny support modules into large dark structural blocks.

Core rule:

> **Seedance 优化不是少画世界，而是把很多小结构合并成少数稳定的大结构。**

---

# 13｜Text / signage

For atmosphere masters:

- default `0–2` large readable in-world markings;
- `302` may appear once when useful;
- one civic/functional marking is enough;
- duplicate giant labels on both sides only when architecture genuinely carries repeated system markings;
- no floating title;
- no text used to explain plot;
- no dense small Chinese signage.

If the scene identity disappears after deleting text, go back to Section 06.

---

# 14｜Prompt assembly — V3

Do not dump a long undifferentiated keyword list.

Assemble in this order:

```text
A. SCENE TRUTH
[exact episode phase + exact dominant action geography]

B. ATMOSPHERE / COMPOSITION
[wide atmosphere master + chosen composition family + dominant spatial relationship + camera distance + scale figures]

C. SEMANTIC ARCHITECTURE
[2–4 large identity anchors + parent-space direction + narrative affordances]

D. OSHII ANIMATION STYLE V1
[material / line / cel-shadow / repair / mood]

E. LIGHTING
[scene-specific light direction and local-time state]

F. SEEDANCE STRUCTURAL REDUCTION
[preserve big geometry + merge repeated structures + simplify far background]

G. NEGATIVE CONSTRAINTS
[scene-specific wrong interpretations + generic style exclusions]
```

---

# 15｜Reusable atmosphere prompt core

Use this as a production core, then replace the scene-specific blocks:

```text
A 2.35:1 wide cinematic environment atmosphere master for 《重庆时间》.
Show the whole spatial system rather than a local room or equipment close-up.
The frame must first read through large architecture, open void, movement direction and light-shadow structure.
Use tiny people or maintenance workers only as scale evidence.

Composition: [axial center-symmetrical / near-symmetrical with one break / oblique structural panorama / layered cross-space wide].
Keep one dominant spatial relationship and one clear depth axis.
Do not let a single machine become the entire subject unless the story explicitly requires it.

Scene identity must be readable without signage through these major physical anchors:
[anchor 1], [anchor 2], [anchor 3].
The space physically leads toward [adjacent space/system].
The architecture must already support later story action: [narrative affordance].

Apply 《重庆时间》押井守动画风格 V1:
aged off-white / warm off-white dominant structural planes,
pale gray secondary structure,
charcoal deep structure,
restrained muted rust-red civic/repair bands,
hand-drawn industrial linework,
2–3 hard-edged cel-shadow tiers,
strong directional structural lighting,
large illuminated planes,
large cast-shadow masses,
old but operational public infrastructure,
quiet and severe procedural atmosphere.

Seedance-ready structural compression:
keep the primary silhouette, dominant route, large frames, large wall planes, major void and main light-shadow masses;
merge repeated rails, windows, pipes, catwalks and small modules into a few stable structural groups;
foreground readable but restrained,
midground carries the main architecture,
far background simplified into large masses and a few major lines,
very few tiny lights,
very few signs,
low high-frequency detail.
```

---

# 16｜Scene-specific negative questions

Before generation, explicitly write 3–6 wrong interpretations to prohibit.

Examples EP01 core atmosphere:

- not a closed machine hall;
- not a giant central-machine shrine;
- not a public residential plaza;
- not the asteroid mining origin layer;
- not open outer space yet;
- not an infinite bottomless city canyon.

Negative constraints should prevent **semantic drift**, not merely aesthetic drift.

---

# 17｜QC — four tests

## A. Thumbnail test

At small size, can the viewer still read:

- main mass;
- main void;
- main route;
- main light direction?

If not, there is too much competing detail.

## B. Relabel test

Remove all signage mentally.

Can the image still only plausibly be this location?

If no, scene identity failed.

## C. Story-action test

Can the space support the episode's actual action without redesigning the architecture later?

If no, the atmosphere master is visually attractive but production-useless.

## D. Seedance motion test

Ask what will likely flicker/mutate when the camera moves:

- dense rails?
- tiny bridges?
- repeated windows?
- small lamps?
- background lattice?
- text?

If too many high-risk zones exist, merge them into larger stable masses before approval.

---

# 18｜Acceptance priority

For a major environment atmosphere master, acceptance priority is:

1. **Canon / episode truth**;
2. **dominant action geography**;
3. **scene identity without text**;
4. **whole-space atmosphere read**;
5. **composition strength**;
6. **Oshii V1 style consistency**;
7. **lighting structure**;
8. **Seedance stability**;
9. micro-detail last.

A beautiful local machine room that misses the episode's dominant geography is a fail.

A visually simpler wide atmosphere image that correctly establishes the space and can animate reliably is preferred.

---

# 19｜Short operating rule

When user says:

> **“重庆时间，按设定出图，EPxx 的核心空间。”**

Internally execute:

> **read EP → locate dominant action geography → choose atmosphere-master mode → lock parent-space direction → choose 2–4 large identity anchors → choose composition → apply Oshii V1 → compress repeated detail for Seedance → generate one 2.35:1 wide image.**

If a choice changes Canon/story facts, ask the user.

If it is only art direction, proceed without unnecessary clarification.
