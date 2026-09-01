# 《重庆时间》SCENE PROMPT TEMPLATE V2

- Updated: 2026-09-01
- Status: `LOCKED / ACTIVE NON-CANON SCENE GENERATION TEMPLATE`
- Canon basis: V4 Master + World + Character + relevant episode snapshot
- Visual basis: `VISUAL-CONSISTENCY-BIBLE-V2.md`
- Default aspect: **2.35:1**

---

# 01｜Mandatory workflow

Every new scene / KV / storyboard keyframe follows:

> **READ → CANON HANDSHAKE → DRAMATIC HANDSHAKE → WORLD-STATE HANDSHAKE → VISUAL HANDSHAKE → PROMPT ASSEMBLY → GENERATE → TWO-LAYER QC**

Do not prompt from memory alone when the relevant Active Canon exists.

---

# 02｜Mandatory read order

1. `CURRENT.md`
2. `ACTIVE-DOCS-INDEX.md`
3. `CANON-PRECEDENCE-V4.md`
4. `CHONGQING-TIME-MASTER-CANON-V4.md`
5. `WORLD-ARCHITECTURE-CANON-V4.md`
6. `CHARACTER-RELATIONSHIP-BIBLE-V4.md`
7. relevant highest V4 Episode Snapshot
8. current execution doc, if any
9. `VISUAL-CONSISTENCY-BIBLE-V2.md`
10. `VISUAL-ANCHOR-INDEX-V2.md`

Historical source only when an active document explicitly leaves the detail `EXECUTION_TBD` and the old source does not conflict with V4.

---

# 03｜Canon Handshake

Before writing a visual prompt, fill:

```yaml
scene_id:
episode_id:
execution_layer: KV / storyboard / shot / generation segment
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

Then write one plain factual sentence:

> **“This scene is: [who/what] doing [specific action] at [specific location] under [specific public/physical condition].”**

If this sentence is generic, do not prompt yet.

---

# 04｜Dramatic Handshake

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

> **Without caption text, can a viewer identify the intended action rather than only “cool sci-fi place”?**

Examples:

- EP02: first read = a bridge is entering controlled separation while evacuation / service activity still exists.
- EP06: first read = one enclosed interface visibly joins two different civic time states.
- EP08: first read = two unequal local security resources face each other across a suspended public bridge while the bridge remains a real route.
- EP10: first read = a still-healthy familiar bridge is being procedurally taken out of shared city operation.

---

# 05｜World-State Handshake

This replaces the old tendency to write only “season/weather.”

```yaml
bridge_connection_state: none / ordinary / reduced-capacity / lifeline / contested / separating / decommissioned
bridge_level: trunk / regional / utility / maintenance / not_applicable
jialing_context: absent / peripheral / lived_public_layer / major_cavity / finale_state
local_public_time_state:
neighbor_public_time_state:
shared_now_status: shared / drifting / absent / one-time-reference-only / not_relevant
gravity_frame_state:
gravity_transition_state:
gravity_severity: 0 / 1 / 2 / 3 / 4 / extreme
islanding_state:
service_capability_state:
public_authorization_state:
protocol_handshake_state:
finite_volume_boundary_cues:
earth_visibility: none / tiny_subordinate / not_applicable
```

Rules:

- `local_public_time_state` describes civic operation, not sky position.
- Do not automatically change gravity because time differs.
- Do not automatically add Jialing River because the episode mentions a bridge.
- If `jialing_context != absent`, name the enclosure cues that keep the space finite.
- If Earth is visible, it stays small and subordinate.

---

# 06｜Visual Handshake

```yaml
aspect_ratio: 2.35:1
approved_anchor_family:
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
4. Which micro-details can be deleted without losing the scene?
5. Does the space look like a mature municipal city rather than a spaceship set?
6. If macro city-scale, is bridge-network topology legible?
7. If enclosed, where are the walls / decks / service boundaries?
8. Is signage confirming, not explaining?

---

# 07｜Master visual prompt block

Use as a base, then insert actual scene facts:

> **Serious cinematic hand-drawn cel-animation background for 《重庆时间》, set inside Second New Chongqing, a mature orbital megacity built from layered urban districts connected by bridges, rail bridges, utility links and maintenance structures rather than a single continuous city ground. Chinese municipal retro-futurist public infrastructure, industrial brutalism, aged dark blue-gray painted steel, repaired structural plates, old off-white civic equipment, restrained blue hard signage, limited muted red warnings, large clear architectural masses, a few thick pipe groups, readable circulation, strong negative space, clear line hierarchy, simplified mechanical contours, 2–3 hard cel-shadow tiers, broad light/dark masses, restrained reflections and bloom, visible ongoing public life or maintenance, huge but finite engineered volume. Scene-specific geometry must match its real function; do not copy another KV’s room or central-axis layout.**

Then append scene-specific paragraph from handshakes.

---

# 08｜Bridge-network prompt patch

Use only when the scene actually needs macro connectivity:

> **At city scale, avoid a continuous ground-plane city. Show distinct layered urban masses and functional platforms connected by a readable hierarchy of bridges. Make the bridge relation clear before micro-detail. Bridges are ordinary municipal infrastructure that may carry people, transit, services, data and gravity handoff; they should not all look like heroic landmark bridges.**

---

# 09｜Jialing River prompt patch

Use only when the scene is actually in / across the Jialing megaspace:

> **The Jialing River is not water and not open outer space. It is a colossal enclosed engineered structural canyon inside the orbital city, with bridges at different elevations, giant wall/deck boundaries, maintenance platforms, service layers and sparse thick pipe systems. The volume feels monumental yet finite. A tiny distant Earth may be visible only through a far structural aperture when canonically useful; it remains subordinate.**

---

# 10｜Local-time prompt patch

> **Express different local public times through civic lighting cycles, traffic density, shop/service state, maintenance shifts, worker/robot activity and restrained public clocks. Do not require visible sky. The two local states should look like different operating rhythms of the same city, not two separate planets.**

If only one local time is relevant, do not force a split-screen day/night composition.

---

# 11｜Gravity prompt patch

Choose actual severity.

### Level 1

> **Subtle local-gravity evidence only: slightly tilted liquid surface, hanging objects leaning, tiny loose items drifting/sliding, residents treating it as routine.**

### Level 2

> **Readable bridge gravity-handoff constraint: people use handrails, industrial robots adapt gait, stretchers/cargo are strapped, posture changes across the transition.**

### Level 3

> **Public operation is visibly constrained: transport capacity reduced, cargo secured, temporary supports/markers, narrow operational window.**

### Extreme

Use only when Canon explicitly requires severe body danger.

Do not automatically add wall-walking / Escher geometry.

---

# 12｜EP08 bridge-standoff patch

> **Suspended inter-district public bridge/interface over a bounded Jialing structural cavity. One better-resourced side fields one medium four-legged municipal public-security platform; the degraded island side coordinates multiple smaller ordinary industrial humanoid robots to maintain order because specialized resources are scarce. Clear size/capability asymmetry, both visibly from the same municipal civilization, degraded side more worn and lower-capability. No wheeled security vehicles. No generic military mecha. The bridge remains an active public route, not a battlefield. Do not write “医疗转运通道” on signage.**

---

# 13｜EP10 procedural separation patch

> **The familiar bridge is technically healthy and still operational. Show staged decommissioning rather than destruction: public traffic cleared, service systems exiting, data/energy connections reduced, gravity transition unloading, mechanical locks releasing in sequence, bridge sections slowly retracting/separating. Public lights may still work until their scheduled shutdown. No explosion, fireball or heroic demolition.**

---

# 14｜Global negative prompt direction

Avoid:

> generic cyberpunk, neon city, premium photoreal hard-SF render, endless space dock, infinite abyss, massive open outer-space void replacing interior enclosure, luxury spaceship, sleek clean future, NASA aesthetic, every-surface greeble, countless thin pipes, dense tiny lights, excessive screens, labels explaining every state, mirror metal, dramatic bloom, giant Earth dominating frame, repeated central-axis hall, generic ground city at macro scale, random military mecha, unexplained battlefield staging, all bridges designed as landmarks, time split shown only by text, gravity spectacle unrelated to action.

---

# 15｜Two-layer QC

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

## Layer B — dramatic / world continuity

```yaml
actual_scene_action_readable: pass/fail
scene_unique_vs_other_KVs: pass/fail
bridge_state_matches_canon: pass/fail/not_applicable
local_public_time_matches_canon: pass/fail/not_applicable
gravity_state_matches_canon: pass/fail/not_applicable
time_gravity_independent: pass/fail
jialing_geometry_matches_canon: pass/fail/not_applicable
continuing_public_behavior_present: pass/fail
no_protected_reveal_leak: pass/fail
no_text_explaining_the_plot: pass/fail
```

A scene passes only when both layers pass.

---

# 16｜Anchor promotion rule

A generated image becomes an official visual anchor only after explicit or clearly affirmative user approval of that image / direction.

Approval of one image does not automatically lock:

- every sign in it；
- every small prop；
- accidental model errors；
- a composition that conflicts with later Canon。

When Canon changes scene geometry, content truth supersedes the old anchor’s spatial accident while its approved art/render/material DNA may remain useful.
