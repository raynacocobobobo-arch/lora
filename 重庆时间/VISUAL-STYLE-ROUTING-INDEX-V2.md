# 《重庆时间》VISUAL STYLE ROUTING INDEX V2

- Updated: 2026-09-03
- Status: `ACTIVE / OSHII ANIMATION STYLE V1 DEFAULT / SEEDANCE-NATIVE`

---

# 01｜Default route

All new environment / setting art defaults to:

> **《重庆时间》押井守动画风格 V1 / OSHII ANIMATION STYLE V1**

There is no separate “normal V1” and “Seedance simplified V1”.

> **Oshii Animation Style V1 itself is the Seedance production style.**

Visual style never overrides current screenplay / Spatial Canon.

---

# 02｜Active references

Style lock:

> `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-LOCK.md`

Prompt package:

> `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-PROMPT.md`

Primary style master:

> `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_OSHII_ANIMATION_STYLE_MASTER_V1.png`

Lighting / color calibration anchor:

> `/重庆时间/visual/style-masters/OSHII_STYLE_V1_LIGHTING_CALIBRATION_HALL_V1.png`

---

# 03｜Current shorthand

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

# 04｜Default output

For major environment masters:

> **single 2.35:1 production frame**, unless the current scene requires another ratio.

Production priority:

1. current Canon / story geography;
2. parent asset / approved geometry;
3. large silhouette and main spatial relationship;
4. lighting structure;
5. large material/color blocks;
6. key functional objects and repair landmarks;
7. micro-detail last.

---

# 05｜Simple workflow

```text
read current Canon / episode facts
→ identify the actual scene and parent space
→ check approved visual master if one exists
→ decide the scene's meaningful time-of-day / lighting logic
→ generate one 2.35:1 Seedance-ready image in Oshii Animation Style V1
→ reject if geometry, style, light or detail density drifts
```

Ask the user only when the unresolved choice would materially change:

- story facts;
- spatial Canon;
- important orientation;
- meaningful day/night/dusk state;
- major object/function definition;
- scene blocking.

For ordinary art-direction details, use the established style master and continue without unnecessary clarification.

---

# 06｜Naming

- `Animation Style V1` = legacy alias;
- `Dungeon Style` = development provenance only;
- `押井守风格`, `押井守风格 V1`, `现在的动画风格` all route to **OSHII ANIMATION STYLE V1**.
