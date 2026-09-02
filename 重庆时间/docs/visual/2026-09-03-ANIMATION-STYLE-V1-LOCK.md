# 《重庆时间》ANIMATION STYLE V1 — VISUAL LOCK

- Updated: 2026-09-03
- Status: `APPROVED / ACTIVE / DEFAULT FOR NEW SETTING ART + SEEDANCE ENVIRONMENT SOURCES`
- Internal name: **《重庆时间》Animation Style V1**
- Scope: environments, architecture, city spaces, bridges, facilities, public infrastructure, exterior city views, Seedance environment source images
- Canon status: **NON-CANON VISUAL EXECUTION LAYER** — this file controls how scenes are drawn, never what story/spatial facts are true.

---

# 01｜Core definition

《重庆时间》Animation Style V1 is the project's default environment rendering language.

Short definition:

> **漫画式建筑线稿 + 极简工业赛璐璐块面 + 大面积黑色负空间 + 旧白公共基础设施 + 少量锈红维修/识别系统 + 可见长期维修历史。**

It is designed from the start for stable image-to-video use.

The rule for all future setting art is:

> **剧本 / Spatial Canon 决定“画什么”；Animation Style V1 决定“怎么画”。**

Do not let the style master overwrite episode facts, bridge scale, district geography, gravity state or local-time state.

---

# 02｜Primary style master image

Persistent image:

> `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_ANIMATION_STYLE_MASTER_V1.png`

Image role:

> **APPROVED SPACE-STATION VISUAL MASTER + APPROVED PROJECT-WIDE ANIMATION STYLE MASTER**

Fingerprint:

- dimensions: `1918 × 820`
- SHA-256: `35f4f27601817f95a7bc7f1c5854aa8aaa0eba5afa613600f1d842edae15f80a`

The master locks two independent things:

1. **Second New Chongqing exterior macro appearance** — central engineered asteroid, complete ring city, limited radial links, old impact/repair sector, distant Earth relation;
2. **project-wide animation rendering grammar** — line, value, palette, repair language, signage behavior and detail density.

Future non-exterior scenes inherit item 2, not the station's literal ring geometry.

---

# 03｜Linework hierarchy

## Primary structural lines

Use stronger, stable, continuous outlines for:

- main architectural silhouette;
- bridge body;
- district mass;
- station hull;
- large columns / beams;
- asteroid silhouette;
- main machinery housing.

## Secondary structural lines

Use medium-weight simplified lines for:

- large panel divisions;
- doors / maintenance hatches;
- reinforcement frames;
- major repair boundaries;
- major railings / access structures.

## Micro-detail

Actively suppress:

- dense screw/bolt fields;
- hundreds of thin pipes;
- excessive antenna forests;
- tiny repeated panel lines;
- decorative hard-surface greeble;
- small lights used only to imply scale.

Rule:

> **Only draw micro-detail when it explains function, damage history or scale.**

---

# 04｜Value / cel-shading system

Default value structure:

1. **light** — aged off-white / pale gray public structural surfaces;
2. **midtone** — cold gray secondary planes;
3. **dark** — charcoal / near-black structural interior, deep shade and negative space.

Use primarily 2–3 hard-edged cel-shadow tiers.

Avoid:

- many soft gradient steps;
- heavy ambient-occlusion noise;
- glossy specular rendering;
- photoreal metallic reflections;
- lens-flare-driven depth.

Depth should primarily come from:

- overlap;
- perspective;
- silhouette separation;
- large black shapes;
- simple value hierarchy.

---

# 05｜Color system

## Dominant

- aged off-white;
- dirty ivory;
- cold gray;
- charcoal / black.

## Primary accent

> **muted rust red / oxide red**

Use rust red selectively for:

- repair plates;
- old structural reinforcement;
- industrial identification bands;
- civic / municipal lettering;
- older module markings;
- selected warning or maintenance areas.

Do not turn the project into a bright red-white spacecraft aesthetic.

The red should feel inherited from a long-used civic/industrial system.

---

# 06｜Material language

Materials are graphic, not PBR-first.

Metal should read through:

- flat structural plane;
- seam / edge;
- restrained scratches;
- patch / repair change;
- paint aging;
- large replacement panel.

Do not rely on:

- mirror reflection;
- micro roughness noise;
- metallic glitter;
- dense photo texture.

---

# 07｜Damage + maintenance DNA

A major identity of the project is:

> **original structure + historical damage + emergency repair + later reinforcement + newer replacement parts.**

Old infrastructure may show:

- large missing shell areas;
- exposed dark structural frame;
- rust-red reinforcement plates;
- mismatched replacement panels;
- old impact scars;
- simplified burn/ablation blocks;
- later maintenance frames;
- different generations of repair hardware.

Damage should remain visually legible at animation scale.

Avoid thousands of tiny fragments or hyper-detailed debris.

---

# 08｜Text / slogan behavior

Text is part of the architecture, never a floating poster title by default.

Approved behaviors:

- weathered painted hull lettering;
- old metal sign;
- large civic/industrial wall slogan;
- module identification marking;
- municipal name integrated into physical structure.

Approved examples:

- `团结协作 共同前进`
- `科学引领未来`
- `第二新重庆市`

Important distinction:

- `第二新重庆市` may appear as an **in-world municipal marking**;
- do **not** place a floating top-of-frame title `第二新重庆` / `SECOND NEW CHONGQING` unless the user explicitly requests poster typography;
- do not add infographic labels, leader lines or explanatory paragraphs to production visual masters.

Do not require slogans in every scene. Use them only when architecture and history justify them.

---

# 09｜Seedance-first design rule

All production environment source images should be designed for temporal stability from the start.

Prioritize:

1. stable large geometry;
2. readable silhouette;
3. clear structural hierarchy;
4. coherent large color blocks;
5. fixed major damage / repair landmarks;
6. low high-frequency noise.

Suppress:

- excessive tiny lights;
- fragile thin wires;
- dense panel seams;
- random micro machinery;
- high-frequency surface texture;
- repeated tiny reflective points.

If a scene becomes visually impressive but difficult to animate, simplify it.

---

# 10｜General style shorthand

Use this shorthand internally when a full prompt is unnecessary:

> **《重庆时间》Animation Style V1: serious graphic cel-animation; manga-inspired architectural linework; black/off-white/cold-gray large masses; large black negative space; 2–3 hard cel-shadow tiers; sparse muted rust-red civic/repair accents; old maintained public infrastructure; visible repair history; low micro-detail; Seedance-stable geometry.**

---

# 11｜Hard exclusions

Do not default to:

- photorealism;
- PBR concept-art finish;
- glossy sci-fi metal;
- cyberpunk neon;
- dense kitbash greeble;
- luxury-futurist design;
- bright multi-color lighting;
- tiny-light scale tricks;
- infographic sheets as production source images;
- floating movie-title typography;
- endless detail added merely to look expensive.

---

# 12｜Relationship to prior Dungeon Style naming

The previously named `DUNGEON STYLE` route is retained as visual-development provenance.

The user has now promoted the current approved visual language into the project's own production name:

> **《重庆时间》Animation Style V1**

Animation Style V1 becomes the default environment lane.

Do not require future prompts to reference an external work or the old `Dungeon Style` nickname.

The prior Dungeon documents remain useful historical/style-source records but no longer define the preferred user-facing production name.
