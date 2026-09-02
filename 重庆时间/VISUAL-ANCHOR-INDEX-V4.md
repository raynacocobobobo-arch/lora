# 《重庆时间》VISUAL ANCHOR INDEX V4

- Updated: 2026-09-03
- Status: `ACTIVE VISUAL ANCHOR OVERLAY / ANIMATION STYLE V1 ROUTED`
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
6. selected style master;
7. scene-specific Seedance constraints.

Short form:

> **Canon 决定画什么；geometry anchor 决定空间资产怎么长；Animation Style V1 决定怎么画。**

---

# 02｜Primary project-wide animation style anchor

## CHONGQING-TIME-ANIMATION-STYLE-V1

Status:

> **APPROVED / ACTIVE / DEFAULT FOR NEW SETTING ART**

Persistent master image:

> `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_ANIMATION_STYLE_MASTER_V1.png`

Fingerprint:

- `1918 × 820`
- SHA-256 `35f4f27601817f95a7bc7f1c5854aa8aaa0eba5afa613600f1d842edae15f80a`

Style lock:

> `docs/visual/2026-09-03-ANIMATION-STYLE-V1-LOCK.md`

Prompt:

> `docs/visual/2026-09-03-ANIMATION-STYLE-V1-PROMPT.md`

Locked style DNA:

- manga-inspired hand-drawn architectural linework;
- large black negative space;
- old off-white / cold-gray structural masses;
- 2–3 hard cel-shadow tiers;
- sparse muted rust-red accents;
- repair / maintenance history expressed as large readable shapes;
- low micro-detail density;
- Seedance-stable silhouettes;
- in-world municipal/civic lettering allowed;
- no floating title text by default.

---

# 03｜RING-ORIENT-01 / Second New Chongqing exterior

Status:

> **APPROVED / CURRENT SPACE-STATION VISUAL MASTER**
>
> **APPROVED / ACTIVE ANIMATION-STYLE SEEDANCE SOURCE REFERENCE**

Current master document:

> `docs/visual/2026-09-03-SECOND-NEW-CHONGQING-ANIMATION-MASTER-V1.md`

Current master image:

> `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_ANIMATION_STYLE_MASTER_V1.png`

Preserve:

- full closed ring-city silhouette;
- central engineered asteroid core;
- limited heavy radial links;
- modular outer city ring;
- recognizable historical impact / repair sector;
- sparse rust-red identification / repair distribution;
- small distant Earth;
- simplified animation rendering.

Text behavior:

- `第二新重庆市` may appear as in-world municipal text;
- `团结协作 共同前进` and `科学引领未来` are approved examples of contextual civic lettering;
- no floating `第二新重庆` / `SECOND NEW CHONGQING` title in ordinary production frames.

Earlier Seedance Master B remains macro-geometry / provenance evidence but is no longer the preferred rendered exterior master.

---

# 04｜Legacy KV and spatial anchors

All detailed KV01–KV06 / EP08 / bridge-scale / geometry statuses remain in `VISUAL-ANCHOR-INDEX-V2.md` unless explicitly superseded by current Canon.

When regenerating those settings:

> keep valid story/spatial function and geometry, but render the new setting asset in **Animation Style V1** unless another lane is explicitly requested.

Style must never enlarge or distort scene scale.

---

# 05｜Oshii preservation

Status:

> **PRESERVED / PARALLEL**

Explicit Oshii-style assets and requests remain routed to the Oshii lane.

Do not auto-convert them to Animation Style V1.

---

# 06｜Dungeon Style provenance

The earlier Dungeon Style master remains provenance and visual-development history.

Its useful discoveries were absorbed into Animation Style V1, especially:

- strong black-white graphic relationships;
- simplified architecture;
- rust-red accents;
- lower detail density;
- visible wear / repair.

Future production naming should use:

> **《重庆时间》Animation Style V1**

rather than requiring an external-style reference name.

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
- prefer large stable structures over micro-detail;
- visible repair history is part of the visual DNA;
- Seedance source geometry continuity outranks decorative detail.

---

# 08｜Current default generation gate

```yaml
script_or_canon_read: yes
parent_spatial_asset_identified: yes
valid_geometry_anchor_identified: yes
style_route: animation_style_v1
style_lock_read: yes
seedance_source_required: yes/no
floating_title_default: no
in_world_signage: contextual
```

For major structural changes such as a possible later EP10 macro separation:

> **lock story geometry first → approve target-state keyframe → then animate.**
