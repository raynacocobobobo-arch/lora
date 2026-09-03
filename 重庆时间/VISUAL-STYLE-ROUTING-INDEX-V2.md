# 《重庆时间》VISUAL STYLE ROUTING INDEX V2

- Updated: 2026-09-03
- Status: `ACTIVE / OSHII ANIMATION STYLE V1 DEFAULT / SEEDANCE-NATIVE / IDENTITY-FIRST`

---

# 01｜Default route

All new environment / setting art defaults to:

> **《重庆时间》押井守动画风格 V1 / OSHII ANIMATION STYLE V1**

There is no separate “normal V1” and “Seedance simplified V1”.

> **Oshii Animation Style V1 itself is the Seedance production style.**

But style routing happens **after** scene identity is locked.

> **Visual style never defines the place. Canon + parent-space relationship define the place; style only defines how that place is drawn.**

---

# 02｜Active references

Scene-generation method:

> `SCENE-PROMPT-TEMPLATE-V2.md`

Style lock:

> `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-LOCK.md`

Prompt package:

> `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-PROMPT.md`

Primary style master:

> `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_OSHII_ANIMATION_STYLE_MASTER_V1.png`

Lighting / color calibration anchor:

> `/重庆时间/visual/style-masters/OSHII_STYLE_V1_LIGHTING_CALIBRATION_HALL_V1.png`

---

# 03｜Scene identity gate

Before routing into Oshii V1, establish:

1. exact location;
2. parent space;
3. 2–4 large physical cues that make the location unique;
4. adjacent system/space it connects toward;
5. current episode function/state.

Hard rule:

> **If changing the sign could turn the image into another generic district, scene identity has failed. Do not generate yet.**

For 302 specifically, read `SPATIAL-ENVIRONMENT-CANON-PATCH-V2.2-302-ORIGIN-LAYER.md` before generation.

302 lived/public space must not become generic old housing; it needs a few large inherited industrial/logistics cues. The asteroid mine itself remains mainly an EP09/EP10 origin-layer location and is not inserted into EP01 merely to prove identity.

---

# 04｜Current style shorthand

> **mature cinematic cel-animation environment + dominant aged off-white structural planes + strong readable structural lighting + 2–3 hard cel-shadow tiers + sparse rust-red civic/repair accents + visible maintenance history + progressive detail reduction with distance + stable Seedance-ready large geometry.**

Important:

- do not interpret the style as flat black-and-white manga poster art;
- do not interpret Seedance optimization as flat lighting;
- do not make every scene the same color temperature;
- day / dusk / night / Local Public Time variation is allowed when story and space support it;
- unify the light-shadow language, not the time-of-day color;
- foreground may carry necessary functional detail;
- midground is simplified;
- background is reduced to large masses, major light-shadow planes and a few key lines;
- repeated windows, railings, pipes, tiny lights, distant people and small signs must not dominate the image.

---

# 05｜Seedance compression rule

Seedance compression happens only after scene identity is correct.

Delete first:

- repeated small windows;
- thin railings;
- fine pipes/cables;
- tiny lights;
- distant crowd detail;
- small signs;
- decorative greeble.

Do **not** delete first:

- scene-defining industrial ancestry;
- parent-space cues;
- bridge-scale cues;
- major functional machinery;
- entry/exit relationship;
- continuity landmarks.

> **删噪声，不删身份。**

---

# 06｜Default output

For major environment masters:

> **single 2.35:1 production frame**, unless the current scene requires another ratio.

Production priority:

1. current Canon / episode facts;
2. scene identity;
3. parent asset / spatial relationship;
4. semantic anchors;
5. large silhouette and main geometry;
6. lighting structure;
7. large material/color blocks;
8. key functional objects / repair landmarks;
9. micro-detail last.

---

# 07｜Simple workflow

```text
read current Canon / episode facts
→ lock scene identity
→ lock parent-space relationship
→ identify 2–4 semantic anchors
→ check approved visual master if one exists
→ route into Oshii Animation Style V1
→ decide meaningful day/night/dusk lighting state
→ apply Seedance compression without deleting identity anchors
→ generate one 2.35:1 image
→ reject if identity, geography, style, lighting or detail density drifts
```

Ask the user only when the unresolved choice materially changes:

- story facts;
- spatial Canon;
- important orientation;
- meaningful day/night/dusk state;
- major object/function definition;
- scene blocking;
- reveal timing.

For ordinary art-direction details, use the established style master and continue without unnecessary clarification.

---

# 08｜Naming

- `Animation Style V1` = legacy alias;
- `Dungeon Style` = development provenance only;
- `押井守风格`, `押井守风格 V1`, `现在的动画风格` all route to **OSHII ANIMATION STYLE V1**.
