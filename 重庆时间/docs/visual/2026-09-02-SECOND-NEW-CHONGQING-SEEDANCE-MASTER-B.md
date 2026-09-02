# 第二新重庆｜Seedance 生产母版 B

- Updated: 2026-09-02
- Project: **《重庆时间》**
- City: **第二新重庆市**
- Status: `APPROVED / ACTIVE PRODUCTION VISUAL MASTER / SEEDANCE 2.5`
- Role: **第二新重庆外景图生视频唯一生产主母版**
- Canon basis: `SPATIAL-ENVIRONMENT-CANON-PATCH-V2.1-ASTEROID-CORE.md` + `SPATIAL-ENVIRONMENT-CANON-V2.md`
- Rendering basis: approved simplified cel-animation environment language, especially KV05 `large shapes first; micro-detail second`
- Repository image asset: `../../assets/visual/second-new-chongqing/SECOND_NEW_CHONGQING_SEEDANCE_MASTER_B.webp`

---

# 00｜Production decision

User explicitly approved the Seedance-optimized B image and chose it as the direct production source.

From this document forward:

> **B is the sole production master for exterior image-to-video work.**

A separate high-detail A master is **not required** for production.

Older high-detail exterior concepts remain provenance/style/engineering references only when useful; they are not mandatory inputs for Seedance.

The production logic is:

> **approved source image B + stable reproduction prompt + shot-specific motion instruction + anti-drift constraints**

---

# 01｜Asset identity

## Human-readable name

> **第二新重庆_Seedance优化母版**

## Repository-safe name

> `SECOND_NEW_CHONGQING_SEEDANCE_MASTER_B.webp`

## Source image used in the approved conversation

- source display name: `第二新重庆_Seedance优化母版.png`
- source dimensions: `1919 × 820`
- source SHA-256: `945c168efd56322ecf129124c2190e922fcd6a8f337e17c88a3720ce55d8e183`

## Repository derivative

For stable Git storage and retrieval, a visually equivalent WebP derivative is stored in-repo:

- path: `重庆时间/assets/visual/second-new-chongqing/SECOND_NEW_CHONGQING_SEEDANCE_MASTER_B.webp`
- dimensions: `1600 × 684`
- WebP quality target: `92`
- SHA-256 of prepared derivative: `982fbd84a24863aa37e87a1fc4d39439b9bb721dce39cb4a61025c81770026b9`

When the original approved PNG is available to the production operator, prefer supplying the original PNG to Seedance. The Git WebP exists as the durable project reference / fallback asset.

---

# 02｜Why B is the production master

The project downstream is explicitly Seedance 2.5 image-to-video.

Therefore the primary production problem is not maximum static concept-art density. It is:

- stable macro silhouette;
- stable geometry across frames;
- low high-frequency flicker risk;
- readable large structures;
- predictable camera motion;
- recoverable/repeatable prompt language;
- same-station recognition across multiple shots.

High-frequency elements that commonly destabilize image-to-video generation include:

- hundreds of tiny windows/lights;
- dense panel seams;
- tiny exposed pipe bundles;
- repeated miniature antennae;
- dense narrow trusses;
- fine star noise;
- excessive hard-surface greeble;
- local photo-texture that has no strong large-form support.

B deliberately keeps the world identity while reducing these sources of temporal noise.

Production priority:

> **structure continuity > silhouette continuity > material/color continuity > hero damage landmarks > micro-detail fidelity.**

---

# 03｜What the approved B image actually locks

## 03.1 Complete station silhouette

The entire Second New Chongqing station is visible in one establishing view.

Primary read:

> a huge, finite, closed ring-city structure centered around an engineered asteroid core.

The main outer ring must remain one recognizable continuous urban/mechanical body.

Do not mutate it into:

- multiple concentric rings;
- an open horseshoe;
- a flat disk;
- a spacecraft fleet;
- a conventional Stanford torus;
- an empty-center ring.

## 03.2 Central engineered asteroid core

The center is occupied by a large irregular asteroid.

The asteroid has:

- natural rock silhouette;
- large hard cel-shaded rock planes;
- visible engineered attachment/containment structures;
- a lower/around-core industrial collar;
- several main structural/service links toward the ring.

The asteroid must remain visibly rock, not turn into a metal sphere or glowing reactor.

## 03.3 Radial structural/service links

A small number of strong radial structures connect the central engineering core toward the outer ring.

They read as:

- heavy;
- broad;
- slow/industrial;
- serviceable;
- structurally important.

They are not dense bicycle spokes and are not ordinary public pedestrian bridges.

For Seedance, preserving their **general position and count impression** is more important than preserving every panel detail.

## 03.4 Outer ring-city body

The surrounding ring is thick because it combines:

- permanent structural spine;
- district modules;
- public/civic city compartments;
- service and industry layers;
- docking/maintenance attachments.

But it must still visually read as modular, not as one seamless tube.

Large module breaks and generational differences may remain visible.

## 03.5 T0 historical impact / repair landmark

One ring sector contains the strong recognizable old T0 damage/repair region.

This is a **visual landmark** and should not wander randomly between shots.

It should read as:

- old structural damage;
- torn/absent exterior shell;
- exposed deeper structure;
- burned/darkened material;
- red-brown repair / older industrial module language;
- later structural reinforcement;
- long-term maintenance rather than active destruction.

The impact region is not currently exploding.

The central asteroid is not the T0 impactor.

## 03.6 Distant Earth relation

Earth appears small and distant.

The station must not read as an ISS-like low-Earth-orbit object.

Earth is:

> **context / home / scale reference**

not the dominant background spectacle.

---

# 04｜B visual style lock

The approved B image belongs to the same visual family already established for 《重庆时间》.

Locked rendering language:

- serious cinematic cel-animation environment;
- hand-drawn / illustrated architectural edges;
- 2–3 dominant hard-edged shading tiers;
- large shape grouping;
- simplified industrial mega-forms;
- controlled mechanical detail;
- low glossy reflection;
- low cyberpunk/neon dependence;
- old municipal / industrial atmosphere;
- mature Chinese retro-futurist orbital-city identity.

## Palette

Primary:

- `aged off-white`
- `dirty ivory`
- `cold blue-gray`
- `deep steel blue`
- `charcoal asteroid gray`

Accent:

- `faded industrial red`
- `muted rust / repair brown`
- small amounts of `muted safety yellow`
- sparse warm practical lights

No saturated rainbow lighting.

---

# 05｜Seedance optimization rules baked into B

The B master intentionally favors:

1. **one strong complete outline** rather than thousands of small silhouette interruptions;
2. **large white/gray district masses** rather than tiny modular tile noise;
3. **broad asteroid planes** rather than photographic rock microtexture;
4. **few strong radial links** rather than dense truss webs;
5. **one readable impact/repair landmark** rather than scattered destruction everywhere;
6. **limited small lights** rather than window grids;
7. **simple distant Earth** rather than detailed planetary motion pressure;
8. **clean deep-space negative area** so camera motion does not constantly hallucinate infrastructure.

---

# 06｜Still-image reproduction contract

If the production team ever needs to regenerate a still approximately matching B, preserve the following in this order:

### Tier 1 — non-negotiable

- entire station visible;
- single closed outer ring silhouette;
- engineered asteroid in center;
- small number of major radial links;
- same broad three-quarter elevated viewing angle;
- T0 repair/damage landmark on a consistent ring sector;
- distant small Earth;
- cel-animation / simplified large-shape rendering.

### Tier 2 — strongly preferred

- old off-white dominant outer modules;
- red-brown legacy/repair region;
- exposed outer maintenance/service attachments;
- central industrial collar around asteroid;
- cold deep-space background.

### Tier 3 — expendable micro detail

- exact number of tiny docking arms;
- individual antenna position;
- individual panel seams;
- tiny lamps;
- tiny maintenance craft;
- small surface text/numbering.

---

# 07｜Master still reproduction prompt

```text
SECOND NEW CHONGQING — SEEDANCE PRODUCTION MASTER B.

Create a complete wide exterior establishing view of the same asteroid-centered modular orbital city. The entire station must fit clearly inside frame, seen from a stable distant three-quarter elevated angle.

Second New Chongqing is one massive closed ring-city built around one engineered asteroid core. The center is not hollow. The asteroid is a large irregular natural rock body with simplified broad charcoal-gray cel-shaded planes, partially integrated into a heavy central industrial dock/collar system. The asteroid remains visibly natural rock and must never become a smooth metal sphere, planet, garden world or glowing reactor.

A limited number of large, thick radial structural/service links connect the central engineered core toward the surrounding ring. Keep them broad and easy to read, with low micro-detail density. Do not create a dense bicycle-wheel spoke pattern.

The surrounding ring is the main city body: one continuous closed circular/elliptical ring silhouette with modular district masses, permanent structural spine, service/industry layers, docking and maintenance attachments. The ring should feel old, repaired, inhabited and operational. Large modules are aged off-white and dirty ivory over cold gray-blue and deep steel structure, with selected faded industrial-red / rust-brown older modules and repair areas.

Keep one strong historical T0 meteor-impact / long-term-repair landmark on one sector of the outer ring. The damage is severe enough to expose deeper structural layers and break the clean hull silhouette locally, with dark burn/ablation areas, reinforcement frames, mismatched replacement plates and older red-brown repair structure. It is historical damage under continued maintenance, not an active explosion. The central asteroid is not the T0 impactor.

Earth is very far away and small in the background. The station must not look like a low-Earth-orbit station. Deep space occupies generous negative space around the city.

Rendering style: serious cinematic cel-animation environment, hand-drawn architectural line feeling, simplified monumental industrial forms, strong large silhouettes, 2–3 hard-edged shading tiers, large shapes first, micro-detail second, restrained practical lights, low glossy reflection, low hard-surface greeble density, mature Chinese civic-industrial retro-futurism.

Seedance-friendly simplification: suppress excessive panel seams, tiny windows, dense pipe bundles, tiny antennas, dense star noise and miniature truss clutter. Preserve the macro geometry and recognizable landmarks instead of adding detail.

Aspect ratio approximately 2.34:1 to 2.35:1. Entire station fully visible.
```

---

# 08｜Still-image negative prompt

```text
no hollow center,
no empty donut hole,
no second central city,
no giant central reactor,
no smooth metal asteroid,
no asteroid as T0 impactor,
no Stanford torus gravity diagram,
no centrifugal gravity visual,
no multiple concentric rings,
no open horseshoe ring,
no dense bicycle spokes,
no giant nearby Earth,
no low Earth orbit appearance,
no active explosion,
no abandoned dead station,
no pristine luxury station,
no cyberpunk neon,
no glossy photoreal NASA render,
no dense hard-surface kitbash,
no excessive tiny lights,
no excessive panel seams,
no tiny pipe noise,
no high-frequency star noise
```

---

# 09｜Production use rule

When generating video, do **not** ask Seedance to redesign the station from text.

Always treat the approved B image as ground truth:

> **image supplies geometry; prompt supplies motion, emphasis, continuity and anti-drift constraints.**

Do not overload the motion prompt with new architecture.

If text and source image conflict, preserve the source image unless the current shot explicitly calls for a state change.

---

# 10｜Relationship to future EP10 state change

B represents the recognizable **pre-major-separation base city state**.

If EP10 later receives a Canon-approved macro separation / Legacy Sector release:

- derive the separation-state asset FROM B;
- keep asteroid core, retained ring identity, main landmark locations and visual style consistent;
- do not ask Seedance to invent a completely new station during the separation shot;
- prepare a dedicated post-separation visual master / keyframe when the story geometry is locked.

Until that story patch is explicitly approved, B remains the active intact-city production master.
