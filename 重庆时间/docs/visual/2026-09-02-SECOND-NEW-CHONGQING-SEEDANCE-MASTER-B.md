# 第二新重庆｜Seedance 生产母版 B

- Updated: 2026-09-02
- Project: **《重庆时间》**
- City: **第二新重庆市**
- Status: `APPROVED / ACTIVE PRODUCTION VISUAL MASTER / SEEDANCE 2.5`
- Role: **第二新重庆外景图生视频唯一生产主母版**
- Canon basis: `SPATIAL-ENVIRONMENT-CANON-PATCH-V2.1-ASTEROID-CORE.md` + `SPATIAL-ENVIRONMENT-CANON-V2.md`
- Rendering basis: approved simplified cel-animation environment language, especially KV05 `large shapes first; micro-detail second`
- Git reference asset: `../../assets/visual/second-new-chongqing/SECOND_NEW_CHONGQING_SEEDANCE_MASTER_B.webp`

---

# 00｜Production decision

User explicitly approved the Seedance-optimized B image and chose it as the direct production source.

From this document forward:

> **B is the sole required exterior production master for image-to-video work.**

A separate high-detail A master is **not required** for production.

Production logic:

> **approved original B image + stable reproduction prompt + shot-specific motion instruction + anti-drift constraints**

The original approved B image is the geometry authority whenever it is available to the production operator.

---

# 01｜Asset identity and reproducibility

## Human-readable source name

> `第二新重庆_Seedance优化母版.png`

## Approved original source

- dimensions: `1919 × 820`
- SHA-256: `945c168efd56322ecf129124c2190e922fcd6a8f337e17c88a3720ce55d8e183`
- role: **production-quality source to supply directly to Seedance 2.5**

The source dimensions + SHA-256 are the authoritative visual fingerprint. If the production operator has this PNG, use it rather than reconstructing B from text.

## Git reference / fallback derivative

Because the current Git connector has practical binary-payload limits, the repository stores a deliberately small visual-reference derivative rather than pretending it is the full production PNG.

- repository path: `重庆时间/assets/visual/second-new-chongqing/SECOND_NEW_CHONGQING_SEEDANCE_MASTER_B.webp`
- dimensions: `420 × 179`
- WebP quality: `65`
- file size: `9026 bytes`
- SHA-256: `94c9f39041dc94a705ef9879ba6ca173858e2c3eaffd3fbe076e44b24a2a5fed`
- Git blob SHA: `155abfdb39ff391d4e2f2dee4ead7196da50642b`
- role: **durable visual fingerprint / retrieval reference / fallback preview**

Important:

> **The 420×179 Git WebP is not intended to replace the approved 1919×820 PNG as the highest-quality Seedance input.**

It exists so future sessions can reliably identify the correct B image family, path, composition and checksum-linked source rather than guessing which exterior image was approved.

---

# 02｜Why B is the production master

The downstream target is Seedance 2.5 image-to-video. The production problem is therefore temporal stability, not maximum static concept-art density.

B prioritizes:

- stable macro silhouette;
- stable geometry across frames;
- readable large structures;
- low high-frequency flicker risk;
- predictable camera motion;
- recognizable station identity across multiple shots.

B intentionally suppresses excessive:

- tiny window/light fields;
- dense panel seams;
- fine pipe bundles;
- miniature antenna clutter;
- narrow repeated trusses;
- high-frequency star noise;
- decorative hard-surface greeble.

Production priority:

> **structure continuity > silhouette continuity > material/color continuity > hero damage landmarks > micro-detail fidelity.**

---

# 03｜Approved B geometry lock

## 03.1 Complete ring-city silhouette

The entire Second New Chongqing station is visible in one establishing view.

Primary read:

> **one huge finite closed ring-city centered around one engineered asteroid core.**

Do not mutate it into multiple rings, an open horseshoe, a flat disk, a fleet, a Stanford torus, or a hollow-center ring.

## 03.2 Central engineered asteroid core

The center contains one large irregular natural asteroid with:

- broad charcoal-gray rock planes;
- visible natural silhouette;
- engineered attachment / containment structures;
- a central industrial collar / dock system;
- several main structural/service links toward the ring.

The asteroid remains rock. It must not become a smooth metal sphere, planet, garden world or glowing reactor.

## 03.3 Major radial links

A limited number of strong radial structural/service links connect the core toward the ring.

They read as heavy, broad, industrial and structurally important.

Preserve their general layout impression before preserving tiny truss detail.

## 03.4 Outer ring-city body

The outer ring combines:

- permanent structural spine;
- district modules;
- civic/public compartments;
- service/industry layers;
- docking and maintenance attachments.

It must read as modular and old, not as one seamless new metal tube.

## 03.5 T0 impact / long-term repair landmark

One outer-ring sector contains the recognizable historical T0 damage/repair region.

Preserve:

- torn/absent exterior shell;
- exposed deeper structure;
- dark burn/ablation areas;
- faded red-brown repair / legacy modules;
- later structural reinforcement;
- long-term maintenance rather than active destruction.

This landmark should remain in a consistent ring sector across shots.

The central asteroid is **not** the T0 impactor.

## 03.6 Distant Earth relation

Earth remains small and distant. It is a quiet scale/home reference, not a low-Earth-orbit backdrop.

---

# 04｜Visual style lock

Preserve:

- serious cinematic cel-animation environment;
- hand-drawn / illustrated architectural edges;
- 2–3 dominant hard-edged shading tiers;
- large shape grouping;
- simplified monumental industrial forms;
- controlled mechanical detail;
- low glossy reflection;
- low cyberpunk/neon dependence;
- mature Chinese retro-futurist orbital-city identity.

Palette:

- aged off-white;
- dirty ivory;
- cold blue-gray;
- deep steel blue;
- charcoal asteroid gray;
- faded industrial red;
- muted rust / repair brown;
- very small amounts of muted safety yellow;
- sparse warm practical lights.

---

# 05｜Still-image reproduction contract

Preserve in this order.

## Tier 1 — non-negotiable

1. entire station visible;
2. single closed outer ring silhouette;
3. engineered asteroid core in center;
4. limited major radial links;
5. broad three-quarter elevated viewing angle;
6. T0 repair/damage landmark in a consistent ring sector;
7. distant small Earth;
8. simplified cel-animation large-shape rendering.

## Tier 2 — strongly preferred

- old off-white dominant modules;
- red-brown legacy/repair area;
- exposed maintenance/service attachments;
- central industrial collar;
- cold deep-space negative area.

## Tier 3 — expendable

- exact tiny docking-arm count;
- exact antenna placement;
- individual panel seams;
- tiny lamps;
- tiny maintenance craft;
- small surface text/numbering.

---

# 06｜Master still reproduction prompt

```text
SECOND NEW CHONGQING — SEEDANCE PRODUCTION MASTER B.

Create a complete wide exterior establishing view of the same asteroid-centered modular orbital city. The entire station must fit clearly inside frame, seen from a stable distant three-quarter elevated angle.

Second New Chongqing is one massive closed ring-city built around one engineered asteroid core. The center is not hollow. The asteroid is a large irregular natural rock body with simplified broad charcoal-gray cel-shaded planes, partially integrated into a heavy central industrial dock/collar system. The asteroid remains visibly natural rock and must never become a smooth metal sphere, planet, garden world or glowing reactor.

A limited number of large, thick radial structural/service links connect the central engineered core toward the surrounding ring. Keep them broad and easy to read, with low micro-detail density. Do not create a dense bicycle-wheel spoke pattern.

The surrounding ring is the main city body: one continuous closed circular/elliptical ring silhouette with modular district masses, permanent structural spine, service/industry layers, docking and maintenance attachments. The ring feels old, repaired, inhabited and operational. Large modules are aged off-white and dirty ivory over cold gray-blue and deep steel structure, with selected faded industrial-red / rust-brown older modules and repair areas.

Keep one strong historical T0 meteor-impact / long-term-repair landmark on one sector of the outer ring. The damage is severe enough to expose deeper structural layers and locally break the clean hull silhouette, with dark burn/ablation areas, reinforcement frames, mismatched replacement plates and older red-brown repair structure. It is historical damage under continued maintenance, not an active explosion. The central asteroid is not the T0 impactor.

Earth is very far away and small in the background. The station must not look like a low-Earth-orbit station. Deep space occupies generous negative space around the city.

Rendering style: serious cinematic cel-animation environment, hand-drawn architectural line feeling, simplified monumental industrial forms, strong large silhouettes, 2–3 hard-edged shading tiers, large shapes first, micro-detail second, restrained practical lights, low glossy reflection, low hard-surface greeble density, mature Chinese civic-industrial retro-futurism.

Seedance-friendly simplification: suppress excessive panel seams, tiny windows, dense pipe bundles, tiny antennas, dense star noise and miniature truss clutter. Preserve macro geometry and recognizable landmarks instead of adding detail.

Aspect ratio approximately 2.34:1 to 2.35:1. Entire station fully visible.
```

---

# 07｜Negative prompt

```text
no hollow center,
no empty donut hole,
no second central city,
no giant central reactor,
no smooth metal asteroid,
no asteroid as T0 impactor,
no Stanford torus gravity,
no centrifugal gravity,
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

# 08｜Seedance use rule

When generating video, do not ask Seedance to redesign the station from text.

> **approved original B image supplies geometry; prompt supplies motion, emphasis, continuity and anti-drift constraints.**

The dedicated motion prompt is:

> `2026-09-02-SECOND-NEW-CHONGQING-SEEDANCE-VIDEO-PROMPT-B.md`

Do not overload motion prompts with new architecture.

---

# 09｜Relationship to EP10

B represents the recognizable intact-city macro baseline.

A possible future EP10 macro separation / Legacy Sector release remains provisional until explicitly promoted into story/spatial Canon.

If approved later:

- derive separation-state assets from B;
- preserve asteroid core and retained-city identity;
- preserve main landmark locations and visual language;
- create dedicated start/end or before/after source keyframes;
- do not ask one intact B image to hallucinate a city-scale split unaided.
