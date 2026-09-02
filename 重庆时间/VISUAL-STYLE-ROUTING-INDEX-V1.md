# 《重庆时间》VISUAL STYLE ROUTING INDEX V1

- Updated: 2026-09-03
- Status: `ACTIVE VISUAL STYLE ROUTER`
- Purpose: keep multiple approved visual lanes explicit and prevent accidental style overwrite

---

# 01｜Routing principle

Visual style is not Canon.

Story/spatial facts are resolved first.

Then select one visual lane.

Default routing order:

1. current explicit user style instruction;
2. scene/asset-specific approved style lock;
3. this routing index;
4. general Visual Bible / legacy anchors.

Do not silently hybridize two lanes.

---

# 02｜DUNGEON STYLE / 地牢风格

Status:

> **ACTIVE / DEFAULT FOR NEW SETTING ART**

Primary style master:

> `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_DUNGEON_STYLE_MASTER_V1.png`

Style lock:

> `docs/visual/2026-09-03-DUNGEON-STYLE-VISUAL-ASSET-LOCK-V1.md`

Prompt:

> `docs/visual/2026-09-03-DUNGEON-STYLE-PROMPT-V1.md`

Default usage:

- new environment setting art;
- architecture / city setting sheets;
- infrastructure / bridge / interface setting art;
- municipal robot/equipment setting art;
- Seedance-friendly environment source images.

Style shorthand:

> **black-white-gray graphic construction + aged off-white industrial masses + sparse rust-red / red-white bands + strong negative space + simplified ink-like industrial linework + hard cel shadows + visible repair history + low high-frequency detail.**

---

# 03｜OSHII STYLE / 押井守风格

Status:

> **PRESERVED / PARALLEL / NOT SUPERSEDED**

The project already established an Oshii-style route before Dungeon Style was named.

This router explicitly preserves that route.

Rules:

- Dungeon Style does not rename Oshii Style;
- Dungeon Style does not retroactively restyle Oshii assets;
- if user explicitly asks for `押井守风格`, route to that lane;
- if an asset already has an explicit Oshii-style lock, keep it there unless the user requests conversion;
- do not merge Dungeon + Oshii automatically.

If a future audit locates a dedicated existing Oshii-style master/prompt document, register its exact path here without altering the parallel-status rule.

---

# 04｜Default decision table

| Request type | Default visual route |
|---|---|
| New environment / city setting image | **DUNGEON STYLE** |
| New architecture / bridge / facility setting art | **DUNGEON STYLE** |
| Seedance environment source image | **DUNGEON STYLE**, unless asset has another explicit lock |
| Existing Oshii-style asset continuation | **OSHII STYLE** |
| User explicitly says 押井守 | **OSHII STYLE** |
| User explicitly says 地牢风格 | **DUNGEON STYLE** |
| Character rendering with existing character style lock | follow character asset lock; do not force Dungeon |
| User asks for hybrid | hybrid only after explicit request |

---

# 05｜Mandatory setting-image workflow

For all new setting images:

> **READ SCRIPT/CANON → identify parent spatial asset → select style route → read style master/prompt → generate → two-layer QC.**

Two-layer QC:

## Story / spatial QC

- correct location;
- correct episode state;
- correct bridge/equipment scale;
- correct time/gravity state;
- no invented geography.

## Style QC

- routed to correct style lane;
- no accidental hybridization;
- scene looks like same visual project;
- source image is Seedance-friendly when required.

---

# 06｜Current default

As of 2026-09-03:

> **New setting art defaults to DUNGEON STYLE.**

This default can be overridden at any time by an explicit user instruction or a scene-specific approved style lock.
