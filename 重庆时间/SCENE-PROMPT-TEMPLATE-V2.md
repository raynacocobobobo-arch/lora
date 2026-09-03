# 《重庆时间》SCENE PROMPT TEMPLATE V2

- Updated: 2026-09-03
- Status: `LOCKED / ACTIVE NON-CANON SCENE GENERATION METHOD / IDENTITY-FIRST / SEEDANCE-NATIVE`
- Canon basis: `CURRENT.md` + current precedence + Spatial V2.1/V2.2/V2 + relevant episode snapshot
- Visual basis: `VISUAL-CONSISTENCY-BIBLE-V2.md` + `VISUAL-STYLE-ROUTING-INDEX-V2.md` + **押井守动画风格 V1**
- Default aspect: **2.35:1**

---

# 01｜Highest method rule

Future environment generation must follow this order:

> **CANON FACTS → SCENE IDENTITY → PARENT-SPACE RELATION → SEMANTIC ANCHORS → STYLE → SEEDANCE COMPRESSION → GENERATE → QC**

Never reverse the order.

The style must not define what the place is.

Seedance simplification must not remove the structures that make the place identifiable.

Core rule:

> **先把“这是哪里、为什么只能是这里”画对，再把它画成《重庆时间》。最后才删动画不稳定的噪声。**

---

# 02｜Mandatory read order

Before a new major environment image, read only the relevant active material, but the following precedence must be respected:

1. current explicit user instruction;
2. `CURRENT.md` / `CANON-PRECEDENCE-V4.md`;
3. latest high-priority spatial patch relevant to the place;
4. `SPATIAL-ENVIRONMENT-CANON-PATCH-V2.1-ASTEROID-CORE.md` when city core is relevant;
5. `SPATIAL-ENVIRONMENT-CANON-PATCH-V2.2-302-ORIGIN-LAYER.md` when 302 is relevant;
6. `SPATIAL-ENVIRONMENT-CANON-V2.md`;
7. `EP01-EP10-SPATIAL-SCENE-MAP-V2.md`;
8. relevant highest active episode snapshot / outline / screenplay;
9. `VISUAL-CONSISTENCY-BIBLE-V2.md`;
10. `VISUAL-STYLE-ROUTING-INDEX-V2.md`;
11. `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-LOCK.md`;
12. approved visual anchor for that asset, if one exists.

Do not prompt from memory when active Canon exists.

An older reference image may provide geometry/function provenance, but may not silently overwrite newer Canon.

---

# 03｜Scene Identity Gate — mandatory

Before writing the style prompt, answer these five questions:

```yaml
scene_location:
scene_parent_space:
scene_function:
three_physical_identity_cues:
what_adjacent_space_or_system_does_this_connect_to:
```

Then write one sentence:

> **“This is [specific place], identifiable without text because [cue 1], [cue 2], [cue 3], and it physically connects toward [adjacent system/space].”**

Hard gate:

> **If the image could be relabeled as another generic district simply by changing a sign, do not generate yet.**

Signs confirm identity; they cannot create identity.

---

# 04｜Parent-space relationship

Every environment belongs to a larger spatial system.

Before generation, define:

```yaml
parent_asset:
position_inside_parent:
city_facing_or_space_facing:
entry_direction:
exit_or_next_space:
major_connector:
visible_parent_space_cues:
forbidden_geography:
```

Hard gate:

> **If you cannot explain how the character enters this space and where the next important space lies, the composition is not ready.**

Examples:

EP01:

> ordinary ring city → outer 302 public/lived side → 302 service/gravity area → small outer attached maintenance/interface segment → space.

EP03/04/08/10:

> the Familiar Lifeline is always the same physically small Level-4 maintenance bridge.

EP06/07:

> shared thermal/environment node and Shared Hub belong to the same Jialing shared-infrastructure family.

---

# 05｜Semantic anchors — do not simplify these away

Before Seedance optimization, identify **2–4 large semantic anchors** that make the scene unique.

Examples:

- 302 public/lived side: ordinary civic life **plus** visible inherited industrial ancestry such as a large old freight frame, heavy transfer structure, legacy service throat, or obvious engineering route toward Gravity Service;
- 302 Gravity Service: old relay / Gravity Service equipment + outer-facing engineering route + legacy compatibility infrastructure;
- EP02 Trunk Bridge: city-scale bridge body + large traffic/service capacity + long-term rescue reinforcement;
- Familiar Lifeline: narrow Level-4 span + compact bridgeheads + Gravity Handoff / maintenance equipment;
- EP06 shared node: one physically shared machine with two district interfaces and one readable mechanical phase;
- 302 asteroid origin layer: exposed asteroid rock + one dominant giant wheel-type excavator + old transfer/maintenance infrastructure.

Seedance compression may remove:

- repeated windows;
- small railings;
- tiny pipes;
- minor panel seams;
- distant people;
- small lights;
- decorative machinery.

Seedance compression may **not** remove:

> **the large structures that explain the scene's history, function, parent-space relationship or episode action.**

Rule:

> **删噪声，不删身份。**

---

# 06｜302 V2.2 identity rule

302 is now a distributed legacy industrial–residential–transfer–compatibility complex with an asteroid-core origin layer and outer lived/service layers.

Do not reduce 302 to either extreme:

- generic old residential district;
- giant mining complex everywhere.

## Outer public/lived layer

Must feel genuinely lived and civic, but should retain visible ancestry from old industrial/logistics infrastructure.

Use a few **large** cues, not dense detail:

- heavy inherited structural frame;
- old transfer/freight opening;
- broad service throat or engineering corridor leading toward Gravity Service;
- large legacy utility structure integrated with civic space.

The viewer should feel:

> **people live here now, but this place grew out of an older industrial system.**

Do not show the asteroid mine itself in EP01/EP04 merely to prove 302 identity.

## Asteroid origin layer

Mainly reserved for EP09 / EP10 under current Canon.

Identity cues:

- exposed asteroid rock face;
- dominant giant wheel-type excavation machine;
- old-white transfer/maintenance structures;
- historical labor/industrial traces;
- still legible and operational in EP09, quietly retired in EP10.

---

# 07｜Dramatic gate

For episode images, define:

```yaml
primary_action:
one_dominant_spatial_relationship:
one_dominant_state:
what_must_be_visible_for_the_episode_to_work:
what_must_not_become_the_subject:
```

Without captions, the viewer should understand the intended action rather than only see a "cool sci-fi place".

Examples:

- EP01: routine maintenance route becoming dangerous through gravity vector instability inside 302 service/interface geography;
- EP02: a **large** city Trunk Bridge reaching controlled forced loss;
- EP03: medical rack crossing a **small** maintenance bridge inside a narrow real window;
- EP06: one shared physical machine between two valid local-time states;
- EP08: two legitimate local orders meeting at the two compact bridgeheads of the same small lifeline;
- EP10: the same healthy small bridge being procedurally retired after people/services clear.

---

# 08｜Style application — only after identity is locked

After Sections 03–07 pass, apply:

> **《重庆时间》押井守动画风格 V1 / Seedance-native production style**

Default visual language:

- aged off-white / warm off-white major structural planes;
- pale/cold gray secondary planes;
- charcoal / near-black for deep structure and cast shadow;
- restrained muted rust-red civic/repair accents;
- strong structural light-shadow organization;
- 2–3 hard-edged cel-shadow tiers;
- hand-drawn architectural/industrial linework;
- visible age and repair history;
- low high-frequency detail.

Day / dusk / night / Local Public Time may vary according to scene facts.

> **统一光影组织，不统一成一种色温。**

---

# 09｜Seedance compression pass

Only after scene identity and style are correct, reduce instability risk.

Use progressive detail falloff:

- foreground: necessary functional detail;
- midground: major structures and key objects only;
- background: large masses, major light-shadow planes, few key lines.

Delete first:

- repeated small windows;
- dense railing patterns;
- fine pipes/cables;
- tiny lights;
- distant crowd detail;
- small signs;
- decorative greeble.

Never delete first:

- parent-space cues;
- scene-defining industrial ancestry;
- bridge scale cues;
- major functional machine;
- damage/repair landmark needed for continuity;
- entry/exit relationship.

---

# 10｜When to ask the user

Ask before generation only when the unresolved choice changes:

- Canon geography;
- major object/function;
- meaningful orientation;
- meaningful day/night/dusk state;
- episode blocking;
- whether a reveal is visible yet;
- which of two materially different parent-space interpretations is intended.

Do not repeatedly ask about ordinary art-direction details already controlled by the approved style master.

---

# 11｜Generation prompt assembly

Use this order:

```text
[scene identity sentence]
+
[parent-space relationship]
+
[2–4 semantic anchors]
+
[current episode action/state]
+
[Oshii Animation Style V1]
+
[scene-specific light/time state]
+
[Seedance compression requirements]
+
[negative constraints]
```

Never begin from the style header and then search for a scene to fit it.

---

# 12｜Final QC

Before accepting a generated environment master:

```yaml
scene_identity_readable_without_signage: pass/fail
could_not_be_relabelled_as_generic_other_district: pass/fail
parent_space_relationship_readable: pass/fail
semantic_anchors_survived_seedance_compression: pass/fail
scene_action_or_function_readable: pass/fail
canon_geography_correct: pass/fail
bridge_scale_correct: pass/fail/not_applicable
302_v2_2_identity_correct: pass/fail/not_applicable
jialing_finite_corridor_correct: pass/fail/not_applicable
oshii_v1_style_consistent: pass/fail
lighting_logic_matches_scene: pass/fail
midground_background_not_overdetailed: pass/fail
signage_confirms_not_creates_identity: pass/fail
```

If **scene identity** fails, reject the image even if the style is beautiful.

If **Seedance stability** fails, simplify high-frequency detail while preserving semantic anchors.

If **Canon** fails, regenerate from the correct parent-space facts rather than cosmetically editing the wrong geography.
