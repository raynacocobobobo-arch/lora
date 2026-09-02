# 《重庆时间》VISUAL ANCHOR INDEX V3

- Updated: 2026-09-03
- Status: `ACTIVE VISUAL ANCHOR OVERLAY / DUNGEON STYLE ROUTED`
- Base anchor registry: `VISUAL-ANCHOR-INDEX-V2.md`
- Style router: `VISUAL-STYLE-ROUTING-INDEX-V1.md`
- Rule: V3 adds the new Dungeon Style master and style-routing behavior; V2 remains the detailed registry for previously approved KV/geometry anchors unless explicitly superseded below.

---

# 01｜Authority order for new setting art

For a new setting image:

1. current user instruction;
2. current story / episode / screenplay facts;
3. `SPATIAL-ENVIRONMENT-CANON-PATCH-V2.1-ASTEROID-CORE.md` + `SPATIAL-ENVIRONMENT-CANON-V2.md` where relevant;
4. parent spatial asset / existing geometry anchor from `VISUAL-ANCHOR-INDEX-V2.md`;
5. `VISUAL-STYLE-ROUTING-INDEX-V1.md`;
6. selected style master;
7. scene prompt / Seedance constraints.

Short form:

> **Canon/剧本决定画什么；geometry anchor决定空间资产长什么；style route决定怎么画。**

---

# 02｜NEW PRIMARY SETTING-ART STYLE ANCHOR

## SECOND-NEW-CHONGQING-DUNGEON-STYLE-MASTER-V1

Status:

> **APPROVED / ACTIVE STYLE + MATERIAL + GRAPHIC-LANGUAGE ANCHOR**
>
> **DEFAULT FOR NEW SETTING ART**

Internal style name:

> **地牢风格 / DUNGEON STYLE**

Persistent source image:

> `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_DUNGEON_STYLE_MASTER_V1.png`

Source fingerprint:

- dimensions: `1923 × 818`;
- SHA-256: `d0dd5a9029108c07d14f37d2e9968d4bb6e63a93d094f1736a5b83bf36c913c9`.

Style lock:

> `docs/visual/2026-09-03-DUNGEON-STYLE-VISUAL-ASSET-LOCK-V1.md`

Prompt:

> `docs/visual/2026-09-03-DUNGEON-STYLE-PROMPT-V1.md`

Locked style DNA:

- high graphic design / poster-like structural clarity;
- strong black negative space;
- aged off-white / gray dominant structural masses;
- sparse muted rust-red accents;
- selective red-white industrial identification bands;
- simplified hand-drawn industrial linework;
- 2–3 hard cel-shadow tiers;
- reduced micro-detail / Seedance-friendly design;
- visible impact/repair/maintenance history;
- large in-world municipal/civic text allowed when compositionally useful;
- no floating movie-title text by default.

The approved master demonstrates that `第二新重庆市` can appear as an **in-world municipal structure marking**, while `科学引领未来` is a valid example of a single large civic slogan. Neither is mandatory in every scene.

---

# 03｜Relationship to RING-ORIENT-01 / Seedance Master B

`VISUAL-ANCHOR-INDEX-V2.md` already locks `RING-ORIENT-01` / Seedance Master B as an approved macro geometry / intact-city production baseline.

V3 does not discard that work.

Use the separation:

> **RING-ORIENT-01 / B = macro geometry + landmark continuity evidence**
>
> **DUNGEON STYLE MASTER V1 = preferred new setting-art rendering/material/graphic style**

For future Second New Chongqing exterior stills:

- preserve current Canon macro structure;
- preserve asteroid-core relationship;
- preserve T0 repair-sector logic;
- render through Dungeon Style unless the user selects another lane.

For Seedance source images, use the Dungeon Style simplification rules from the start.

---

# 04｜Oshii lane preservation

Status:

> **OSHII STYLE PRESERVED / PARALLEL / NOT SUPERSEDED**

Nothing in V3 converts or deletes the prior Oshii-style route.

If the user explicitly asks for `押井守风格`, route away from Dungeon Style and use the preserved Oshii lane.

Do not auto-hybridize.

---

# 05｜Legacy KV anchors

All detailed statuses for KV01–KV06, EP08 direction, bridge scale and prior macro geometry remain in:

> `VISUAL-ANCHOR-INDEX-V2.md`

V3 changes their default **future restyling route**, not their approved story/spatial function.

If a legacy KV is regenerated as a new setting asset without another explicit style instruction:

> **keep its valid scene function/geometry, but render the new version in Dungeon Style.**

Do not blindly copy obsolete geometry that V2 already marked superseded.

---

# 06｜Default routing examples

## New 嘉陵江 wide setting art

- read Spatial V2 + relevant episode state;
- use Jialing bridge-scale facts;
- use Dungeon Style for rendering.

## New 302 orientation art

- preserve one-side-city / one-side-space logic;
- use Dungeon Style for rendering.

## New EP02 Trunk Bridge

- keep Level-1 large scale;
- use Dungeon Style for rendering.

## New Familiar Lifeline

- keep Level-4 physically small;
- use Dungeon Style for rendering;
- style must not enlarge it into a heroic mega-bridge.

## Existing Oshii-style character/image continuation

- keep Oshii route unless user asks to convert.

---

# 07｜New-setting generation gate

Before generating any new setting image, confirm internally:

```yaml
script_read: yes/no
spatial_canon_read: yes/no
parent_asset_identified: yes/no
style_route: dungeon | oshii | other_explicit
style_master_read: yes/no
seedance_source_required: yes/no
```

If `style_route: dungeon`, read the Dungeon Style lock + prompt before generation.
