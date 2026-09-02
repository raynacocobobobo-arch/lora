# 《重庆时间》VISUAL ANCHOR INDEX V4

- Updated: 2026-09-03
- Status: `ACTIVE VISUAL ANCHOR OVERLAY / OSHII ANIMATION STYLE V1 ROUTED / LIGHTING-CALIBRATED`
- Detailed legacy registry: `VISUAL-ANCHOR-INDEX-V2.md`
- Previous overlay: `VISUAL-ANCHOR-INDEX-V3.md`
- Active style router: `VISUAL-STYLE-ROUTING-INDEX-V2.md`

---

# 01｜Authority order

For new setting art:

1. current user instruction;
2. current story / episode / screenplay facts;
3. active Spatial Canon / patch;
4. parent spatial asset / valid geometry anchor;
5. `VISUAL-STYLE-ROUTING-INDEX-V2.md`;
6. selected style master + lighting calibration anchor;
7. scene-specific Seedance constraints.

Short form:

> **Canon 决定画什么；geometry anchor 决定空间资产怎么长；押井守动画风格 V1 决定怎么画；lighting calibration 决定白色、亮度和光影结构怎么落。**

---

# 02｜Primary project-wide Oshii animation style anchor

## CHONGQING-TIME-OSHII-ANIMATION-STYLE-V1

Status:

> **APPROVED / ACTIVE / DEFAULT FOR NEW SETTING ART**
>
> **APPROVED / ACTIVE / DEFAULT FOR SEEDANCE ENVIRONMENT SOURCES**

Primary style master:

> `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_OSHII_ANIMATION_STYLE_MASTER_V1.png`

Fingerprint:

- `1918 × 820`
- SHA-256 `35f4f27601817f95a7bc7f1c5854aa8aaa0eba5afa613600f1d842edae15f80a`

Lighting / white-material calibration anchor:

> `/重庆时间/visual/style-masters/OSHII_STYLE_V1_LIGHTING_CALIBRATION_HALL_V1.png`

Fingerprint:

- `1915 × 821`
- SHA-256 `a991c49eecf481dd2785e7c38587499ea71ff059fed06141b4760a34ff005c31`

Style lock:

> `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-LOCK.md`

Prompt:

> `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-PROMPT.md`

Locked style DNA:

- mature cinematic anime / cel-animation environment;
- hand-drawn architectural / industrial structural linework;
- **aged off-white / warm off-white as dominant visible architectural material**;
- pale / cold gray secondary structure;
- charcoal / near-black reserved for deep shadows, void and exposed structure;
- **strong directional architectural lighting**;
- large readable illuminated planes;
- large hard-edged cast-shadow shapes;
- clear light / midtone / deep-shadow hierarchy;
- 2–3 hard cel-shadow tiers;
- sparse muted rust-red accents;
- selected red-white functional identification / repair bands;
- visible repair / maintenance history expressed as large readable shapes;
- low micro-detail density;
- Seedance-stable silhouettes and lighting blocks;
- in-world municipal/civic lettering allowed;
- no floating title text by default;
- quiet, procedural, lived-in public-system mood rather than spectacle.

Hard anti-drift:

> **Do not reduce Oshii Style V1 to a flat black-and-white manga poster. Do not flatten the light to make Seedance easier. Simplify micro-detail first.**

---

# 03｜RING-ORIENT-01 / Second New Chongqing exterior

Status:

> **APPROVED / CURRENT SPACE-STATION VISUAL MASTER**
>
> **APPROVED / ACTIVE OSHII-ANIMATION SEEDANCE SOURCE REFERENCE**

Current master image:

> `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_OSHII_ANIMATION_STYLE_MASTER_V1.png`

Preserve:

- full closed ring-city silhouette;
- central engineered asteroid core;
- limited heavy radial links;
- modular outer city ring;
- recognizable historical impact / repair sector;
- old-white dominant structural body;
- sparse rust-red identification / repair distribution;
- red-white functional striping only where compositionally useful;
- small distant Earth;
- simplified cel-animation rendering with readable form lighting.

Text behavior:

- `第二新重庆市` may appear as in-world municipal text;
- `团结协作 共同前进` and `科学引领未来` are approved examples of contextual civic lettering;
- no floating `第二新重庆` / `SECOND NEW CHONGQING` title in ordinary production frames.

---

# 04｜LIGHT-CAL-01 / Public observation hall lighting anchor

Status:

> **APPROVED / LIGHTING + COLOR + CONTRAST CALIBRATION ANCHOR**

Use this anchor to correct future interiors and lit public spaces.

It locks:

- dominant old-white wall / frame / column surfaces;
- strong exterior directional light when a large opening is present;
- clear hard-edged cast shadows from architecture;
- bright structural planes against dark audience / deep-shadow zones;
- restrained rust-red signage / ceremonial / civic accents;
- 2.35:1 wide production-source composition for major Seedance environment masters when no other ratio is specified;
- no unnecessary exterior architecture if the canonical view is directly toward Earth / deep space.

It does **not** lock the observation hall's literal geometry for unrelated scenes.

---

# 05｜Naming migration

The active production name is:

> **《重庆时间》押井守动画风格 V1 / OSHII ANIMATION STYLE V1**

Therefore:

- `Animation Style V1` = legacy alias;
- separate old `Oshii lane` is no longer a competing route;
- `Dungeon Style` remains visual-development provenance only.

---

# 06｜Legacy KV and spatial anchors

All detailed KV01–KV06 / EP08 / bridge-scale / geometry statuses remain in `VISUAL-ANCHOR-INDEX-V2.md` unless explicitly superseded by current Canon.

When regenerating those settings:

> keep valid story/spatial function and geometry, but render the new setting asset in **Oshii Animation Style V1** unless another style is explicitly requested.

Style must never enlarge or distort scene scale.

---

# 07｜Mandatory anti-drift rules

- approved style never overrides Canon;
- Second New Chongqing remains asteroid-centered, not hollow-centered;
- central asteroid ≠ T0 impactor;
- ring topology ≠ centrifugal gravity;
- Jialing ≠ torus center hole;
- EP02 Trunk Bridge remains much larger than Familiar Lifeline;
- Familiar Lifeline remains small under current Canon;
- no generic 3D hard-SF drift;
- no photoreal PBR default;
- no cyberpunk neon default;
- no floating movie-title text in ordinary production sources;
- **no flat-light default**;
- **off-white remains the main visible structural color in applicable public/industrial architecture**;
- black remains deep shadow / exposed structure / void, not default wall color;
- strong cast-shadow geometry is part of the style when the scene has a directional light source;
- prefer large stable structures over micro-detail;
- visible repair history is part of the visual DNA;
- Seedance continuity outranks decorative detail, but not major lighting hierarchy.

---

# 08｜Current default generation gate

```yaml
script_or_canon_read: yes
parent_spatial_asset_identified: yes
valid_geometry_anchor_identified: yes
style_route: oshii_animation_style_v1
style_lock_read: yes
lighting_logic_identified: yes
visible_structure_color_default: aged_off_white
flat_lighting_default: no
seedance_source_required: yes/no
major_environment_aspect_default: 2.35:1
floating_title_default: no
in_world_signage: contextual
```

For major structural changes such as a possible later EP10 macro separation:

> **lock story geometry first → approve target-state keyframe → then animate.**
