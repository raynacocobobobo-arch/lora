# 《重庆时间》押井守动画风格 V1 — PROMPT PACKAGE

- Updated: 2026-09-03
- Status: `ACTIVE / SEEDANCE-NATIVE PRODUCTION PROMPT`
- Style lock: `2026-09-03-OSHII-ANIMATION-STYLE-V1-LOCK.md`
- Primary visual master: `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_OSHII_ANIMATION_STYLE_MASTER_V1.png`
- Lighting calibration anchor: `/重庆时间/visual/style-masters/OSHII_STYLE_V1_LIGHTING_CALIBRATION_HALL_V1.png`

---

# 01｜Universal style header

```text
《重庆时间》押井守动画风格 V1。

serious cinematic anime environment,
mature cel-animation background art,
hand-drawn architectural and industrial linework,
large readable geometric masses,
clear structural perspective,
2–3 hard-edged cel-shading tiers,
strong readable light-shadow structure,
large illuminated planes,
large cast-shadow masses,
aged off-white and warm off-white as the dominant visible structural colors,
pale gray secondary surfaces,
charcoal and near-black only in deep shadow, void and exposed engineering interiors,
small restrained muted rust-red / oxide-red accents for repair plates, functional bands, civic markings and selected signage,
old but operational public infrastructure,
visible long-term maintenance and repair history.

SEEDANCE-NATIVE VISUAL DESIGN:
stable large geometry,
stable silhouette,
clear visual hierarchy,
foreground readable but restrained,
midground simplified into major structures and functional objects,
background strongly reduced into large masses, major light-shadow planes and only a few key structural lines,
minimal repeated small windows,
minimal dense railings,
minimal tiny pipes,
minimal small lights,
minimal distant crowd detail,
minimal noisy panel seams,
few large in-world signs only,
large coherent color blocks,
low high-frequency visual noise,
animation-friendly scene design.
```

---

# 02｜Lighting rule

```text
Lighting color may change with the scene and Local Public Time:
neutral or cool daylight,
restrained warm dusk light,
cold night ambience with limited warm practical lights,
or controlled warm/cool coexistence at time-boundary spaces.

But the lighting structure must remain consistent:
clear light / midtone / deep-shadow hierarchy,
large readable illuminated surfaces,
hard-edged architectural cast shadows when the scene allows,
light must explain the architecture,
never flat lighting,
never evenly lit gray exposure,
never a whole-frame warm filter,
never a whole-frame blue filter.
```

统一的是光影组织，不是统一色温。

---

# 03｜Seedance production rule

Major environment source frames default to **2.35:1** unless another ratio is explicitly required.

```text
2.35:1 cinematic wide frame,
stable architecture,
stable major landmarks,
stable lighting direction,
stable cast-shadow masses,
stable large color blocks,
clear foreground-midground-background separation,
reduce detail progressively with distance,
preserve main geometry and key damage / repair landmarks,
no fragile micro-detail dependency,
no structural mutation,
no random new machinery appearing,
no disappearing major components,
no flickering dense signage,
no dense star-like light fields.
```

Priority:

> **major geometry → light/shadow → color blocks → key functional objects → repair landmarks → micro-detail last.**

---

# 04｜Text behavior

Production frames use world-internal text only.

```yaml
floating_title: false
infographic_callout: false
technical_explanation_panel: false
in_world_municipal_marking: allowed
in_world_civic_slogan: allowed_when_contextual
small_dense_signage: avoid
```

Prefer a few large stable signs over many small labels.

---

# 05｜Universal negative block

```text
no flat lighting,
no evenly lit gray scene,
no weak structural shadows,
no black-dominant manga poster look,
no photoreal PBR render,
no glossy hard-surface sci-fi,
no cyberpunk neon,
no dense micro-greeble,
no excessive panel lines,
no tiny pipes everywhere,
no dense railing patterns,
no endless repeated windows,
no excessive antennas,
no excessive tiny lights,
no dense distant crowds,
no high-frequency texture noise,
no cluttered background detail,
no photobash look,
no luxury futuristic design,
no floating movie title,
no infographic labels
```

---

# 06｜Prompt assembly order

```text
[current scene facts from screenplay / Spatial Canon]
+
[parent asset geometry / existing visual anchor]
+
[Oshii Animation Style V1 universal style header]
+
[scene-specific time-of-day / lighting / damage / signage]
+
[Seedance production rule]
+
[negative block]
```

Never let the visual style invent or overwrite Canon.

If a missing decision would change spatial facts, world mechanics, meaningful time-of-day, orientation or story blocking, ask the user before generating. Otherwise proceed from the established master style and current Canon.

---

# 07｜Second New Chongqing exterior reference prompt

```text
第二新重庆市巨型环形轨道城市完整外景，2.35:1。

保持已批准母版的大结构：完整闭合环形城市、中央工程化小行星核心、少量粗壮径向结构、外围模块化主环、固定的历史撞击/维修区和远处小地球。

使用《重庆时间》押井守动画风格 V1：旧白和灰白为主要可见结构色，冷灰/炭黑用于深阴影和暴露结构，少量锈红用于维修补强、功能识别带和城市标识。2–3档硬边赛璐璐明暗，清楚的大轮廓和大光影。

Seedance-native：保留主环轮廓、中央小行星、主要径向连接、撞击旧伤和大色块；压低小灯、密集 panel line、细管道、细栏杆、小型外挂机械和远景噪声。远景只保留大结构与少量关键线条。
```
