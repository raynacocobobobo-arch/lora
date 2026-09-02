# 《重庆时间》VISUAL STYLE ROUTING INDEX V2

- Updated: 2026-09-03
- Status: `ACTIVE VISUAL STYLE ROUTER / OSHII ANIMATION STYLE V1 DEFAULT`
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

Short name:

> **押井守风格 V1 / OSHII STYLE V1**

Style master:

> `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_OSHII_ANIMATION_STYLE_MASTER_V1.png`

Style lock:

> `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-LOCK.md`

Prompt package:

> `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-PROMPT.md`

Current station geometry/master document may continue to use the older `ANIMATION` filename as provenance until separately renamed; its rendering route is now Oshii Animation Style V1.

Style shorthand:

> **serious graphic cel-animation + manga architectural linework + black/off-white/cold-gray large masses + large black negative space + 2–3 hard shadow tiers + sparse rust-red civic/repair accents + old maintained public infrastructure + visible repair history + Seedance-stable low micro-detail.**

---

# 03｜Naming migration

The user explicitly merged the previously separate names.

Current meaning:

- `Animation Style V1` = **legacy alias** for the current Oshii Animation Style V1;
- old separate `Oshii Style lane` = **merged into the current production lane**;
- `Dungeon Style` = **visual-development provenance only**;
- there is no longer a production decision between `Animation Style V1` and `Oshii Style`.

If the user says any of the following:

- `押井守风格`
- `押井守风格 V1`
- `现在的动画风格`
- `Animation Style V1`

route to:

> **OSHII ANIMATION STYLE V1**

---

# 04｜Default decision table

| Request | Default route |
|---|---|
| New city / environment setting image | **OSHII ANIMATION STYLE V1** |
| New architecture / bridge / facility setting art | **OSHII ANIMATION STYLE V1** |
| Seedance environment source | **OSHII ANIMATION STYLE V1** |
| Second New Chongqing exterior | **OSHII ANIMATION STYLE V1 + current station master geometry** |
| User explicitly says 押井守 | **OSHII ANIMATION STYLE V1** |
| User says 现在这个动画风格 | **OSHII ANIMATION STYLE V1** |
| User explicitly requests another style | follow explicit request |
| Character with separate locked character style | follow character lock; do not force environment style |

---

# 05｜Mandatory workflow

```text
READ SCRIPT / CANON
→ identify parent spatial asset
→ identify valid geometry anchor
→ route style
→ read Oshii Animation Style V1 lock + prompt
→ generate one production reference image
→ story/spatial QC
→ style/Seedance QC
```

Default lane:

```yaml
style_route: oshii_animation_style_v1
style_lock: docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-LOCK.md
prompt_package: docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-PROMPT.md
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
3. value-block stability;
4. major damage / repair landmarks;
5. large color distribution;
6. signage placement if visible;
7. micro-detail last.

If detail threatens temporal stability, simplify it.
