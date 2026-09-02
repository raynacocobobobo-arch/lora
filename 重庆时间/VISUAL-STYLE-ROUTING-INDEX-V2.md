# 《重庆时间》VISUAL STYLE ROUTING INDEX V2

- Updated: 2026-09-03
- Status: `ACTIVE VISUAL STYLE ROUTER / OSHII ANIMATION STYLE V1 DEFAULT / LIGHTING-CALIBRATED`
- Supersedes routing defaults in: `VISUAL-STYLE-ROUTING-INDEX-V1.md`

---

# 01｜Routing principle

Visual style is not Canon.

Resolve story / spatial facts first, then select the visual lane.

Default order:

1. current explicit user instruction;
2. scene/asset-specific approved style lock;
3. this routing index;
4. general Visual Bible / legacy anchors.

---

# 02｜OSHII ANIMATION STYLE V1 / 押井守动画风格 V1

Status:

> **ACTIVE / DEFAULT FOR ALL NEW ENVIRONMENT + SETTING ART**
>
> **ACTIVE / DEFAULT FOR SEEDANCE ENVIRONMENT SOURCE IMAGES**

Official Chinese name:

> **《重庆时间》押井守动画风格 V1**

Internal English name:

> **CHONGQING TIME — OSHII ANIMATION STYLE V1**

Style master:

> `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_OSHII_ANIMATION_STYLE_MASTER_V1.png`

Lighting / color calibration anchor:

> `/重庆时间/visual/style-masters/OSHII_STYLE_V1_LIGHTING_CALIBRATION_HALL_V1.png`

Style lock:

> `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-LOCK.md`

Prompt package:

> `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-PROMPT.md`

Corrected shorthand:

> **mature cinematic cel-animation environment + dominant aged off-white structural planes + strong directional architectural lighting + large hard-edged light/shadow blocks + manga-inspired structural linework + 2–3 cel-shadow tiers + cold gray/charcoal deep structure + sparse muted rust-red civic/repair accents + visible repair history + low micro-detail + Seedance-stable geometry.**

Hard correction:

- do **not** interpret this route as flat black-and-white manga poster art;
- do **not** default to flat/even lighting;
- old off-white / warm off-white must usually remain the dominant visible architectural material;
- black is reserved for deep shadow, exposed structure, void and selected negative space;
- strong structural cast shadows are part of the style;
- Seedance simplification removes micro-detail before it removes lighting hierarchy.

---

# 03｜Naming migration

Current meaning:

- `Animation Style V1` = legacy alias for **Oshii Animation Style V1**;
- old separate `Oshii Style lane` = merged into the current production lane;
- `Dungeon Style` = visual-development provenance only;
- there is no production decision between `Animation Style V1` and `Oshii Style`.

If the user says `押井守风格`, `押井守风格 V1`, `现在的动画风格` or `Animation Style V1`, route to **OSHII ANIMATION STYLE V1**.

---

# 04｜Default decision table

| Request | Default route |
|---|---|
| New city / environment setting image | **OSHII ANIMATION STYLE V1** |
| New architecture / bridge / facility setting art | **OSHII ANIMATION STYLE V1** |
| Seedance environment source | **OSHII ANIMATION STYLE V1** |
| Major Seedance environment master | **OSHII ANIMATION STYLE V1 / default 2.35:1 unless otherwise locked** |
| Second New Chongqing exterior | **OSHII ANIMATION STYLE V1 + current station master geometry** |
| User explicitly says 押井守 | **OSHII ANIMATION STYLE V1** |
| User explicitly requests another style | follow explicit request |
| Character with separate locked character style | follow character lock; do not force environment style |

---

# 05｜Mandatory workflow

```text
READ SCRIPT / CANON
→ identify parent spatial asset
→ identify valid geometry anchor
→ route style
→ read Oshii Animation Style V1 lock + corrected prompt
→ identify scene light source / lighting logic
→ generate one production reference image
→ story/spatial QC
→ lighting/color/style QC
→ Seedance QC
```

Default lane:

```yaml
style_route: oshii_animation_style_v1
style_lock: docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-LOCK.md
prompt_package: docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-PROMPT.md
lighting_default: strong_directional_structural_light_when_scene_allows
visible_structure_color_default: aged_off_white
seedance_major_environment_aspect_default: 2.35:1
flat_lighting_default: false
```

---

# 06｜Text routing

Default production source frames:

- no floating film title;
- no infographic explanation;
- in-world civic slogans allowed when contextually justified;
- municipal markings allowed;
- `第二新重庆市` is an in-world municipal marking, not a default poster title.

---

# 07｜Seedance priority

Prioritize:

1. large silhouette;
2. main structural geometry;
3. stable directional lighting and major cast-shadow shapes;
4. off-white / gray / charcoal value-block stability;
5. major damage / repair landmarks;
6. restrained rust-red distribution;
7. signage placement if visible;
8. micro-detail last.

If detail threatens temporal stability, simplify detail first — **do not flatten the lighting**.
