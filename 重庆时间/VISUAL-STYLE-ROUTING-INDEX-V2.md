# 《重庆时间》VISUAL STYLE ROUTING INDEX V2

- Updated: 2026-09-03
- Status: `ACTIVE / OSHII ANIMATION STYLE V1 DEFAULT / ATMOSPHERE-FIRST / SEEDANCE-NATIVE`

---

# 01｜Default route

All new environment / setting art defaults to:

> **《重庆时间》押井守动画风格 V1 / OSHII ANIMATION STYLE V1**

There is no separate “normal V1” and “Seedance simplified V1”.

> **Oshii Animation Style V1 itself is the Seedance production style.**

But style routing happens only after the scene-generation method has resolved what the image actually is.

> **Canon + episode action geography define the place; Scene Prompt V3 defines the image mode/composition; Oshii V1 defines how it is drawn.**

---

# 02｜Active references

Active scene-generation method for new environment / atmosphere work:

> `SCENE-PROMPT-TEMPLATE-V3.md`

Legacy lower-level method:

> `SCENE-PROMPT-TEMPLATE-V2.md`

Use V2 only as provenance / fallback for older scene-generation decisions. New major environment images route through V3.

Style lock:

> `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-LOCK.md`

Prompt package:

> `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-PROMPT.md`

Primary style master:

> `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_OSHII_ANIMATION_STYLE_MASTER_V1.png`

Lighting / color calibration anchor:

> `/重庆时间/visual/style-masters/OSHII_STYLE_V1_LIGHTING_CALIBRATION_HALL_V1.png`

---

# 03｜Natural-language routing

The following user phrasing automatically triggers `SCENE-PROMPT-TEMPLATE-V3.md`:

- `重庆时间，按设定出图`
- `重庆时间，按设定出图，EPxx...`
- `按重庆时间设定出图`
- `按 GitHub 设定出这个场景`
- `EPxx 的核心空间`
- `场景气氛图`
- `环境母图`
- `大场景`
- `这个场景视觉化一下`

If the request contains `核心空间 / 场景气氛图 / 环境母图 / 大场景`, default output mode is:

> **2.35:1 wide atmosphere master / establishing environment**

Do not answer those requests with a local machine room or equipment close-up unless the user explicitly asks for `局部 / 节点 / 设备 / 特写 / 机房`.

---

# 04｜Core-space routing

For an episode `核心剧情空间`, choose the **dominant action geography**, not the most memorable named node.

Evaluate:

1. runtime coverage;
2. dominant physical action coverage;
3. state-change coverage.

Example EP01:

- old relay = key node;
- Gravity Service machine room = local functional shot;
- **302 service/gravity path → outer-facing maintenance/interface route** = dominant action geography;
- atmosphere master therefore establishes the larger Gravity Service Spine / outer service void.

---

# 05｜Scene identity gate

Before routing into Oshii V1, establish:

1. exact location/system;
2. parent space;
3. dominant action geography;
4. 2–4 large physical identity anchors;
5. adjacent space/system it leads toward;
6. narrative affordances required by later action.

Hard rule:

> **If changing the sign can turn the image into another generic district, scene identity has failed.**

For 302, read `SPATIAL-ENVIRONMENT-CANON-PATCH-V2.2-302-ORIGIN-LAYER.md`.

---

# 06｜Composition routing

Major atmosphere masters must select a composition family intentionally:

- **axial / center-symmetrical monumental** — procedural infrastructure, long service routes, institutional order;
- **near-symmetrical with one controlled break** — ordered system with one meaningful scar/asymmetry;
- **oblique structural panorama** — movement direction or bridge geography dominates;
- **layered cross-space wide** — two sides + one shared object must read together.

Center symmetry is a strong project tool, not a universal default for every scene.

The recent 302 Gravity Service Spine studies validated axial / near-symmetrical atmosphere composition as a useful family for EP01 infrastructure.

---

# 07｜Current style shorthand

> **mature cinematic cel-animation environment + dominant aged off-white structural planes + strong readable structural lighting + 2–3 hard cel-shadow tiers + sparse rust-red civic/repair accents + visible maintenance history + large atmosphere-first spatial read + progressive detail reduction with distance + stable Seedance-ready geometry.**

Important:

- do not interpret the style as flat black-and-white manga poster art;
- do not interpret Seedance optimization as flat lighting;
- do not make every scene the same color temperature;
- day / dusk / night / Local Public Time variation is allowed when story and space support it;
- unify the light-shadow language, not the time-of-day color;
- wide environment masters prioritize whole-space relationship before local object detail.

---

# 08｜Seedance structural compression

Seedance optimization is now defined as **structural compression**, not simple detail deletion.

Preserve:

- primary silhouette;
- dominant route;
- large structural frames;
- major open void;
- large wall planes;
- 1–3 main bridge/platform masses;
- major repair landmark;
- main light direction and cast-shadow masses;
- minimal scale figures.

Merge/simplify:

- repeated catwalks;
- dense cross-bridges;
- background structural grids;
- window/opening repetition;
- fine rails;
- micro-pipe networks;
- tiny lamps;
- small signs;
- distant decorative machinery.

Use three readable depth bands:

> **foreground frame → main midground architecture → simplified far mass.**

Core rule:

> **删噪声，不删身份；合并结构，不削平空间。**

---

# 09｜Default output priority

For major environment masters:

> **single 2.35:1 production frame**, unless the scene explicitly requires another ratio.

Priority:

1. current Canon / episode facts;
2. shot mode;
3. dominant action geography;
4. scene identity;
5. parent-space relationship;
6. narrative affordances;
7. composition strength;
8. Oshii V1 style;
9. lighting structure;
10. Seedance stability;
11. micro-detail last.

---

# 10｜Simple workflow

```text
read current Canon / episode facts
→ determine shot mode
→ locate dominant action geography
→ lock scene identity and parent-space direction
→ identify 2–4 large semantic anchors
→ identify later-action affordances
→ choose composition family
→ route into Oshii Animation Style V1
→ decide meaningful day/night/dusk lighting state
→ apply Seedance structural compression
→ generate one 2.35:1 image
→ run thumbnail / relabel / story-action / Seedance-motion QC
```

Ask the user only when the unresolved choice materially changes:

- story facts;
- spatial Canon;
- important orientation;
- meaningful day/night/dusk state;
- major object/function definition;
- scene blocking;
- reveal timing.

For ordinary art-direction details, proceed from the established method and style master without unnecessary clarification.

---

# 11｜Naming

- `Animation Style V1` = legacy alias;
- `Dungeon Style` = development provenance only;
- `押井守风格`, `押井守风格 V1`, `现在的动画风格` all route to **OSHII ANIMATION STYLE V1**;
- new major environment-generation method = **SCENE PROMPT TEMPLATE V3 / atmosphere-first method**.
