# 《重庆时间》SCENE PROMPT TEMPLATE V2

- Updated: 2026-09-02
- Status: `LOCKED / ACTIVE NON-CANON SCENE GENERATION TEMPLATE / SPATIAL V2 RECONCILED`
- Canon basis: `CURRENT.md` + Story Repair + `SPATIAL-ENVIRONMENT-CANON-V2.md` + Master/World/Character + relevant episode
- Visual basis: `VISUAL-CONSISTENCY-BIBLE-V2.md`
- Default aspect: **2.35:1**

---

# 01｜Mandatory workflow

Every new scene / KV / storyboard keyframe follows:

> **READ → SPATIAL HANDSHAKE → CANON HANDSHAKE → DRAMATIC HANDSHAKE → WORLD-STATE HANDSHAKE → VISUAL HANDSHAKE → PROMPT ASSEMBLY → GENERATE → TWO-LAYER QC**

Do not prompt from memory alone when active Canon exists.

Do not allow an older approved image to silently invent geography that conflicts with Spatial V2.

---

# 02｜Mandatory read order

1. `CURRENT.md`
2. `SPATIAL-ENVIRONMENT-CANON-V2.md`
3. `EP01-EP10-SPATIAL-SCENE-MAP-V2.md`
4. `CANON-PRECEDENCE-V4.md`
5. `STORY-CAUSAL-CANON-PATCH-V1.md` when relevant
6. `CHONGQING-TIME-MASTER-CANON-V4.md`
7. `WORLD-ARCHITECTURE-CANON-V4.md`
8. `CHARACTER-RELATIONSHIP-BIBLE-V4.md`
9. relevant highest episode snapshot / approved outline / screenplay
10. `VISUAL-CONSISTENCY-BIBLE-V2.md`
11. `VISUAL-ANCHOR-INDEX-V2.md`
12. current execution doc, if any.

Historical source only when active docs explicitly leave a detail open and the old source does not conflict.

---

# 03｜Spatial Handshake — mandatory before every environment prompt

```yaml
spatial_parent_asset: ordinary_district / jialing / 302 / trunk_bridge / familiar_lifeline / shared_infrastructure / outer_attached_segment / exterior_space / other_canon_location
ring_city_relation:
city_facing_or_space_facing: city_facing / jialing_facing / space_facing / not_relevant
movement_from_previous_space:
explicit_connector_used: bridge / rail / district_route / interface / maintenance_access / EVA / not_relevant
bridge_physical_level: level_1_trunk / level_2_regional / level_3_utility / level_4_maintenance / not_applicable
familiar_lifeline_check: same_small_level_4 / not_applicable
jialing_definition_check: finite_open_urban_corridor / not_applicable
ordinary_nominal_down: broadly_aligned / interface_exception / event_exception
space_boundary_readability:
forbidden_old_geometry:
```

Hard gate:

> **If you cannot explain how the character entered this space from the prior space in one sentence, do not prompt yet.**

For EP01, legal route is:

> `ordinary ring city → 302 → 302 service/gravity area → small outer attached segment → space`

For EP03/04/08/10, Familiar Lifeline must always remain:

> **physically small Level-4 maintenance bridge.**

---

# 04｜Canon Handshake

```yaml
scene_id:
episode_id:
execution_layer: KV / storyboard / shot / generation_segment
canon_sources_read:
current_turn_user_overrides:
scene_function:
location:
city_state:
core_physical_fact:
public_system_state:
characters_present:
required_objects:
required_signage:
forbidden_signage:
reveals_allowed:
reveals_protected:
```

Then one factual sentence:

> **“This scene is: [who/what] doing [specific action] at [specific location] under [specific public/physical condition].”**

If generic, do not prompt.

---

# 05｜Dramatic Handshake

```yaml
primary_readable_action:
core_conflict_in_frame:
continuing_operations_required:
scene_uniqueness_vs_existing_KVs:
background_suppression:
first_read:
second_read:
what_must_not_become_the_subject:
```

Test:

> **Without caption text, can viewer identify intended action rather than only “cool sci-fi place”?**

Examples:

- EP01: first read = one worker is being carried through a damaged 302 service/interface route by worsening gravity; not “endless upside-down city”.
- EP02: first read = a **large** city Trunk Bridge is entering controlled retirement while final service activity remains.
- EP03: first read = one medical rack is trying to cross a **small narrow maintenance bridge** during a constrained window.
- EP06: first read = one shared physical utility sits between two different civic time states.
- EP08: first read = unequal local security/maintenance resources confront each other at the **two bridgeheads of the same small lifeline**.
- EP10: first read = a **small familiar healthy bridge** is being procedurally removed from shared operation after people/services have largely cleared.

---

# 06｜World-State Handshake

```yaml
bridge_connection_state: none / ordinary / reduced_capacity / lifeline / contested / separating / decommissioned
bridge_level: level_1_trunk / level_2_regional / level_3_utility / level_4_maintenance / not_applicable
jialing_context: absent / peripheral / finite_open_corridor / shared_infrastructure / finale_state
local_public_time_state:
neighbor_public_time_state:
shared_now_status: shared / drifting / absent / one_time_reference_only / not_relevant
gravity_frame_state:
gravity_transition_state:
gravity_severity: 0 / 1 / 2 / 3 / 4 / extreme
islanding_state:
service_capability_state:
public_authorization_state:
protocol_handshake_state:
finite_volume_boundary_cues:
ring_topology_cues:
earth_visibility: none / tiny_subordinate / not_applicable
```

Rules:

- local time = civic operation, not sun/sky position;
- time difference does not automatically change gravity;
- ordinary district nominal down is broadly stable/aligned;
- do not automatically add Jialing because an episode mentions a bridge;
- if Jialing is present, it is a **finite urban corridor with district masses and multiple bridge scales**, not an infinite cavity;
- if Earth visible, keep small/subordinate.

---

# 07｜Visual Handshake

```yaml
aspect_ratio: 2.35:1
approved_anchor_family:
anchor_geometry_status: compatible / style_only_geometry_superseded / not_applicable
composition_family:
space_type:
major_shape_plan:
negative_space_plan:
material_family:
municipal_equipment_family:
palette:
lighting_logic:
local_time_visual_cues:
gravity_visual_cues:
cel_shadow_tiers: 2-3
micro_detail_budget: low / medium
signage_budget: low
ongoing_public_behaviors:
spatial_closure_rule:
anti_drift_notes:
```

Hard questions:

1. What are the 3–5 largest shapes?
2. What is the one dominant spatial relationship?
3. What is the one dominant state?
4. Which micro-details can be deleted?
5. Does this read as a mature municipal city rather than spaceship set?
6. If macro view, is the ring/module/bridge relation legible?
7. If Jialing, are bridge scale differences legible?
8. If 302, is city-facing vs space-facing logic correct?
9. If Familiar Lifeline, is it unmistakably small?
10. Is signage confirming rather than explaining?

---

# 08｜Master visual prompt block

Use as a base, then insert actual scene facts:

> **Serious cinematic hand-drawn cel-animation background for 《重庆时间》, set in Second New Chongqing, a mature modular ring-shipyard orbital city built on a permanent ring backbone. Large inhabited district modules, smaller attached service structures and a readable hierarchy of bridges form one finite urban whole. Chinese municipal retro-futurist public infrastructure, industrial brutalism, aged dark blue-gray painted steel, repaired structural plates, old off-white civic equipment, restrained blue hard signage, limited muted-red warnings, large clear architectural masses, a few thick pipe groups, readable circulation, strong negative space, clear line hierarchy, simplified mechanical contours, 2–3 hard cel-shadow tiers, broad light/dark masses, restrained reflections and bloom, visible ongoing public life or maintenance. Ordinary inhabited districts have a broadly stable nominal down; stronger gravity differences appear only where the scene requires a bridge/interface/damaged zone. Scene-specific geometry must match Spatial Environment Canon V2; do not copy an old KV’s accidental geography.**

Then append scene-specific paragraph.

---

# 09｜Ring-city macro prompt patch

Use when showing overall Second New Chongqing:

> **Read the city first as one finite irregular ring-shipyard structure, not an endless layered metropolis. Show distinct large district modules attached to a durable ring backbone, smaller service modules, and clearly different bridge scales. The ring form organizes the city but does not imply rotational gravity. Keep the city legible as a long-used expanding municipal structure rather than a pristine spacecraft.**

---

# 10｜Bridge-network prompt patch

> **Show bridge physical hierarchy clearly. Level-1 Trunk Bridges are massive city-scale composite links; Level-4 maintenance bridges are narrow, low-capacity industrial connections. Bridges may carry people, services, data and gravity handoff, but they should not all look like heroic landmarks. Narrative importance must not inflate physical bridge size.**

---

# 11｜Jialing prompt patch — V2

Use only when actually in/across Jialing:

> **The Jialing River is not water, not the torus central hole, and not open outer space. It is a broad finite open urban/public corridor running inside the ring city, bounded by inhabited district masses and engineered structure. Multiple bridge scales, rail links and shared utilities cross or occupy it. Make the corridor large but spatially readable; show structural boundaries and district faces rather than an infinite abyss. A tiny distant Earth may appear only through a canonical outer opening and must remain subordinate.**

---

# 12｜302 prompt patch

> **302 is an outer legacy district cluster with a clear two-sided orientation: its city-facing side contains ordinary lived/public urban space; its space-facing side contains older Gravity Service, legacy relay and small attached maintenance/interface structures leading toward EVA/exterior space. Do not depict 302 as a deep underground city or a stack of many districts.**

For EP01 cost:

> **Only one small outer attached maintenance/interface segment accidentally loses structural connection after Plan B has genuinely begun working; the 302 district itself remains attached. No deliberate ejection, no explosive hull rupture, no vacuum suction.**

---

# 13｜Familiar Lifeline prompt patch — V2

> **The EP03/04/08/10 Familiar Lifeline is always a physically small Level-4 maintenance bridge: narrow industrial passage, handrails, interface equipment, room for people on foot, a small transport rack and industrial humanoids, with compact maintenance bridgeheads at both ends. It can become socially or politically important without becoming physically large. Never render it as a wide rail/vehicle bridge or monumental landmark.**

---

# 14｜Local-time prompt patch

> **Express different local public times through civic lighting cycles, traffic density, shop/service state, maintenance shifts, worker/robot activity and restrained public clocks. Do not require visible sky. The states are different operating rhythms of the same city, not different planets.**

If one local time only, do not force split-screen day/night.

---

# 15｜Gravity prompt patch

### Ordinary district

> **Stable ordinary municipal gravity; architecture and people share one visually readable nominal down.**

### Level 1

> **Subtle local-gravity evidence only: slightly tilted liquid surface, hanging objects leaning, tiny loose items drifting/sliding, residents treating it as routine.**

### Level 2

> **Readable small bridge/interface Gravity Handoff: people use handrails, industrial robots adapt gait, stretchers/cargo are strapped, posture changes modestly through the transition.**

### Level 3

> **Public operation visibly constrained: capacity reduced, cargo secured, temporary supports/markers, narrow operating window.**

### Extreme

Use only when Canon requires severe body danger, principally EP01.

Do not automatically add wall-walking / Escher city geometry.

---

# 16｜EP08 bridgehead-standoff patch

> **Stage the scene around the two compact maintenance bridgeheads of the same narrow Level-4 Familiar Lifeline. On the better-resourced side, one medium four-legged municipal public-security platform approaches with local staff. On the degraded side, multiple smaller ordinary industrial humanoid robots are already working around bridgehead structure locks, interface equipment and Gravity Handoff maintenance; they may temporarily carry a public-order role, then return to maintenance. Clear capability asymmetry, same municipal civilization, degraded side more worn and resource-limited. The narrow bridge remains an active public route. No wheeled security vehicles, no generic military mecha, no giant bridge deck, no central battle arena, no “医疗转运通道” sign.**

---

# 17｜EP10 procedural separation patch

> **The same small Familiar Lifeline is technically healthy and still operational, but by this point most 302 residents have already migrated through earlier routes and staged transfers. Show final low-volume clearance and staged decommissioning: remaining people/services clear, data/energy/environment paths retire, Gravity Handoff unloads, time/protocol compatibility exits, then the small bridge’s mechanical connection releases/isolate. No giant evacuation crowd, no physical bridge scale-up, no explosion or heroic demolition. The permanent ring backbone remains.**

---

# 18｜Global negative prompt direction

Avoid:

> generic cyberpunk, neon city, premium photoreal hard-SF render, endless space dock, infinite abyss, bottomless Jialing canyon, torus central hole labeled Jialing, endless stacked city layers, default 90-degree rotated districts, luxury spaceship, sleek clean future, NASA aesthetic, every-surface greeble, countless thin pipes, dense tiny lights, excessive screens, labels explaining every state, mirror metal, dramatic bloom, giant Earth dominating frame, repeated central-axis hall, giant Familiar Lifeline, generic military bridge deck, random military mecha, unexplained battlefield staging, all bridges designed as landmarks, time split shown only by text, gravity spectacle unrelated to action.

---

# 19｜Two-layer QC

## Layer A — visual continuity

```yaml
same_art_department: pass/fail
same_city_material_family: pass/fail
cel_rendering_consistent: pass/fail
large_shapes_before_micro_detail: pass/fail
municipal_not_generic_spaceship: pass/fail
finite_volume: pass/fail
signage_restraint: pass/fail
```

## Layer B — dramatic / spatial / world continuity

```yaml
spatial_parent_asset_matches_v2: pass/fail
movement_from_previous_space_is_explicit: pass/fail/not_applicable
actual_scene_action_readable: pass/fail
scene_unique_vs_other_kvs: pass/fail
bridge_physical_level_matches_canon: pass/fail/not_applicable
familiar_lifeline_remains_small: pass/fail/not_applicable
local_public_time_matches_canon: pass/fail/not_applicable
gravity_state_matches_canon: pass/fail/not_applicable
ordinary_nominal_down_is_readable: pass/fail/not_applicable
time_gravity_independent: pass/fail
jialing_is_finite_ring_interior_corridor: pass/fail/not_applicable
302_city_space_orientation_matches: pass/fail/not_applicable
continuing_public_behavior_present: pass/fail
no_protected_reveal_leak: pass/fail
no_text_explaining_plot: pass/fail
```

Both layers must pass.

---

# 20｜Anchor promotion / supersession rule

A generated image becomes official visual anchor only after explicit or clearly affirmative user approval.

Approval of one image does not lock every accidental detail.

When later Canon changes geometry:

> **approved art/render/material DNA may remain active; incompatible spatial/content geometry becomes STYLE-ONLY provenance.**

Never resolve a Canon conflict by blindly copying an older approved image.
