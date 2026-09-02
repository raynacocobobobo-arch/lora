# 《重庆时间》VISUAL STYLE ROUTING INDEX V2

- Updated: 2026-09-03
- Status: `ACTIVE VISUAL STYLE ROUTER / ANIMATION STYLE V1 DEFAULT`
- Supersedes routing default in: `VISUAL-STYLE-ROUTING-INDEX-V1.md`

---

# 01｜Routing principle

Visual style is not Canon.

Resolve story/spatial facts first, then select one visual lane.

Default order:

1. current explicit user instruction;
2. scene/asset-specific approved style lock;
3. this routing index;
4. general Visual Bible / legacy anchors.

Do not silently hybridize lanes.

---

# 02｜ANIMATION STYLE V1

Status:

> **ACTIVE / DEFAULT FOR ALL NEW ENVIRONMENT + SETTING ART**
>
> **ACTIVE / DEFAULT FOR SEEDANCE ENVIRONMENT SOURCE IMAGES**

Style master:

> `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_ANIMATION_STYLE_MASTER_V1.png`

Style lock:

> `docs/visual/2026-09-03-ANIMATION-STYLE-V1-LOCK.md`

Prompt package:

> `docs/visual/2026-09-03-ANIMATION-STYLE-V1-PROMPT.md`

Current station master:

> `docs/visual/2026-09-03-SECOND-NEW-CHONGQING-ANIMATION-MASTER-V1.md`

Style shorthand:

> **graphic cel-animation + manga architectural linework + black/off-white/cold-gray large masses + large black negative space + 2–3 hard shadow tiers + sparse rust-red civic/repair accents + old maintained public infrastructure + visible repair history + Seedance-stable low micro-detail.**

---

# 03｜Dungeon Style provenance

Status:

> **PRESERVED AS VISUAL-DEVELOPMENT PROVENANCE / NO LONGER DEFAULT PRODUCTION NAME**

The previous Dungeon Style documents remain useful for tracing the origin of the graphic simplification language.

Future prompts do not need to reference `Dungeon Style` or an external work.

Use the project's own production name:

> **《重庆时间》Animation Style V1**

---

# 04｜Oshii Style lane

Status:

> **PRESERVED / PARALLEL / NOT SUPERSEDED**

If the user explicitly requests `押井守风格`, route to the preserved Oshii lane.

Do not auto-hybridize Animation Style V1 + Oshii.

Existing explicit Oshii assets remain Oshii unless the user asks to convert them.

---

# 05｜Default decision table

| Request | Default route |
|---|---|
| New city / environment setting image | **ANIMATION STYLE V1** |
| New architecture / bridge / facility setting art | **ANIMATION STYLE V1** |
| Seedance environment source | **ANIMATION STYLE V1** |
| Second New Chongqing exterior | **ANIMATION STYLE V1 + current station master geometry** |
| Existing Oshii-style asset continuation | **OSHII STYLE** |
| User explicitly asks 押井守 | **OSHII STYLE** |
| User explicitly requests another style | follow explicit request |
| Character with separate locked character style | follow character lock; do not force environment style |

---

# 06｜Mandatory setting-image workflow

```text
READ SCRIPT / CANON
→ identify parent spatial asset
→ identify valid geometry anchor
→ route style
→ read selected style lock + prompt
→ generate one production reference image
→ story/spatial QC
→ style/Seedance QC
```

For the default lane:

```yaml
style_route: animation_style_v1
style_lock: docs/visual/2026-09-03-ANIMATION-STYLE-V1-LOCK.md
prompt_package: docs/visual/2026-09-03-ANIMATION-STYLE-V1-PROMPT.md
```

---

# 07｜Text routing

Default production source frames:

- no floating film title;
- no infographic explanation;
- in-world civic slogans allowed when contextually justified;
- municipal markings allowed;
- `第二新重庆市` is an in-world municipal marking, not a default poster title.

---

# 08｜Seedance priority

When a frame is intended for image-to-video, prioritize in this order:

1. large silhouette;
2. main structural geometry;
3. value block stability;
4. major damage / repair landmarks;
5. large color distribution;
6. signage placement if visible;
7. micro-detail last.

If detail threatens temporal stability, simplify it.
