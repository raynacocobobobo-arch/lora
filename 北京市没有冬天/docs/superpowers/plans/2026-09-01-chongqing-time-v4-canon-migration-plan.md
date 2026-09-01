# 《重庆时间》V4 Canon Migration Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** 将现有《北京市没有冬天》V3.2 工作集完整迁移为《重庆时间》V4：第二新重庆市桥网城市、嘉陵江巨型封闭结构空腔、日夜时间断层、Local Gravity Frames、EP01–EP10 有机因果链、EP10 疏散/断桥/废弃城区终局，并确保旧设定被移除时由新机制完整接替其原有叙事/工程/视觉功能。

**Architecture:** 新建 `重庆时间/` 作为唯一 Active 项目根目录；旧 `北京市没有冬天/` 保留为 legacy/provenance 来源。迁移不是全局替词，而是以已批准 V4 World Architecture + Episode Architecture 两份 spec 为依据，先建 Master/World Canon，再逐集迁移，最后重写视觉/Teaser/索引并做全仓一致性检查。旧非聊天项目文档在迁移前按原 blob 归档；`decision-logs/` 与全文聊天记录保留为 provenance，不进入旧设定归档批次。

**Tech Stack:** GitHub Markdown Canon documents, GitHub Contents/Git Tree APIs, semantic consistency review.

**Spec:**
- `北京市没有冬天/docs/superpowers/specs/2026-09-01-chongqing-time-v4-world-architecture-design.md`
- `北京市没有冬天/docs/superpowers/specs/2026-09-01-chongqing-time-v4-episode-architecture-design.md`

## Global Constraints

- Project title is **《重庆时间》**.
- Active fictional city is **第二新重庆市**; new Active Canon must not retain Beijing as current-series identity.
- Meteor impact remains **before EP01**; EP05 remains the only explicit ordinary-person return to T0 impact day.
- **No snow / winter as an active series mechanism or finale payoff.** Every removed winter/snow function must receive a defined replacement.
- Second New Chongqing is a **bridge-network orbital megacity**, not a continuous-ground city at city scale.
- **嘉陵江** is a colossal enclosed engineered structural canyon crossed by bridge layers; distant Earth may be visible only through a bounded far structural opening and remains subordinate.
- Districts maintain **Local Gravity Frames**; gravity failure concentrates at bridge handoffs and recurs across the season at controlled severity.
- Time fragmentation and gravity fragmentation are **independent axes**.
- Time fracture is expressed as local **day / dusk / night / shift / public-service rhythms**, usually without sky.
- Organic integration is mandatory: **character need/public action first; setting only enters where it changes action or consequence.**
- Preserve existing strong causal/character material: 302, protocol handshake ladder, EP04 Rashomon influence, memorial/reconstruction practice, Wedding Mirror, chief↔private-AI EP06 relationship turn, healthy Hub exit, EP08 no-villain institutional violence, minimum common reality, private-AI continuity cost.
- EP08 bridge standoff: no wheeled vehicles; one medium quadruped public-security platform on one side; multiple ordinary industrial humanoid robots on the degraded island side; no generic military mecha; no `医疗转运通道` sign.
- EP10 final familiar bridge must be technically healthy; no explosion shortcut; separation is procedural/mechanical.
- Private AI wants to survive, genuinely searches for a preservation route, never becomes/merges into city AI, and copy/upload does not equal continuity.
- Historical/legacy files may contain 北京/雪/冬季 because they are archived provenance; **new Active root may not accidentally inherit those as live facts.**

## Mandatory old→new replacement matrix

| Removed / superseded old function | Required V4 replacement — no gap allowed |
|---|---|
| 北京 / 第二新北京 as active city identity | 第二新重庆市 + Chongqing-derived layered bridge-city spatial grammar |
| Continuous city ground at macro scale | District modules + multi-level bridge / rail / utility / maintenance connection network |
| Winter / snow as regional-state contrast | Local day/dusk/night public-time fragmentation and civic operating rhythms |
| EP05 artificial snow → real local snow → EP06 transition | Wedding local-time visual counterpoint → direct escalation into EP06 loss of common now |
| EP06 dual-season / dual-winter imagery | Enclosed day/night split, public clocks, shifts, transit/maintenance/service cycles |
| EP10 unified winter protocol → snow proof | Remaining districts share one public Chongqing time; synchronized ordinary night-life behaviors prove convergence |
| EP01 one-off gravity inversion | Local Gravity Frames + bridge gravity-handoff failure ladder recurring across EP02/03/04/07/08/09/10 |
| Generic internal abyss / open dock | Bounded engineered 嘉陵江 cavity with enclosing walls/decks/service layers and subordinate distant Earth |
| Generic ground checkpoint in EP08 | Suspended bridge/interface above 嘉陵江, derived organically from EP03 lifeline → EP04 routine infrastructure |
| Abstract EP10 `legacy branch` | Evacuated old district + final bridge/service/time/gravity/protocol compatibility stack |
| Abstract AI-preservation cost | Keep final legacy district/bridge/time/gravity compatibility condition alive indefinitely |
| Random final disconnection | Season-long familiar EP03 lifeline becomes EP10 final important connection |

---

### Task 1: Freeze legacy sources and establish the V4 root

**Files:**
- Create: `北京市没有冬天/archive/2026-09-01-pre-chongqing-time-v4/README.md`
- Create: exact blob-preserving archive copies of pre-V4 non-chat project documents under `北京市没有冬天/archive/2026-09-01-pre-chongqing-time-v4/`
- Exclude from that archive batch: `北京市没有冬天/decision-logs/**`, the two approved V4 specs, and this implementation plan.
- Create: `重庆时间/README.md`
- Create/copy: `重庆时间/docs/superpowers/specs/2026-09-01-chongqing-time-v4-world-architecture-design.md`
- Create/copy: `重庆时间/docs/superpowers/specs/2026-09-01-chongqing-time-v4-episode-architecture-design.md`
- Create/copy: `重庆时间/docs/superpowers/plans/2026-09-01-chongqing-time-v4-canon-migration-plan.md`

**Produces:** immutable pre-V4 reference set and a clean active root.

- [ ] Step 1: capture the current main commit SHA as the archive source baseline and record it in the archive README.
- [ ] Step 2: create archive entries by reusing original blob SHAs so archived text is byte-identical; do not rewrite historical Beijing/snow wording.
- [ ] Step 3: create `重庆时间/README.md` declaring it the sole Active root and linking legacy provenance to `北京市没有冬天/`.
- [ ] Step 4: copy approved V4 specs and this plan into the new root unchanged.
- [ ] Step 5: verify archived `CURRENT.md`, Master V3.2, highest EP snapshots, active visual docs, Teaser V2, and consistency reports retain their source blob/content; verify `decision-logs` were not copied into the archive batch.
- [ ] Step 6: commit with a migration-foundation message.

### Task 2: Build clean V4 world authority before episodes

**Files:**
- Create: `重庆时间/CHONGQING-TIME-MASTER-CANON-V4.md`
- Create: `重庆时间/WORLD-ARCHITECTURE-CANON-V4.md`
- Create: `重庆时间/CANON-PRECEDENCE-V4.md`
- Create: `重庆时间/CHARACTER-RELATIONSHIP-BIBLE-V4.md`

**Consumes:** V3.2 Master, patches V3.2.1–V3.2.5, approved V4 world/episode specs.

**Produces:** one consolidated V4 authority with no patch-sprawl dependency for core facts.

- [ ] Step 1: write Master V4 with premise, T0 timeline, Preservation Paradox progression, series theme, public-governance arc, three-person role architecture, episode summary, and finale outcome.
- [ ] Step 2: write World Architecture Canon with bridge hierarchy, district topology, 嘉陵江, bounded volume rule, local time architecture, Local Gravity Frames, gravity severity ladder, time/gravity independence, islanding as loss of connection density, and bridge carrying city state as well as people.
- [ ] Step 3: integrate protocol-handshake terminology from V3.2.1 directly into V4 authority: `协议握手 / protocol handshake`, physical connection, physical-hand motif remain distinct.
- [ ] Step 4: integrate EP04→EP07 Rashomon cognitive-source chain from V3.2.2 without making the film an explicit puzzle key.
- [ ] Step 5: integrate pre-EP01 meteor timeline and visual-scale semantics from V3.2.3, translated to Second New Chongqing/Jialing River geometry.
- [ ] Step 6: integrate memorial/reconstruction practice and Wedding Mirror social origin from V3.2.4.
- [ ] Step 7: integrate unconditional male/private-AI belonging, chief↔AI EP06 restrained recognition, and EP10 narrow authorization/relay roles from V3.2.5.
- [ ] Step 8: write precedence so later explicit user decisions > V4 episode snapshot > Master V4 > active execution docs > legacy archive; old V3 patches become provenance rather than live dependencies.
- [ ] Step 9: run conceptual replacement audit against the mandatory old→new matrix. No old seasonal/Beijing function may be deleted without a V4 successor paragraph.
- [ ] Step 10: commit world authority as a self-contained reviewable batch.

### Task 3: Migrate EP01–EP03 and establish the physical spine

**Files:**
- Create: `重庆时间/Pilot-EP01-LATEST-CANON-SNAPSHOT-V4.md`
- Create: `重庆时间/Pilot-EP02-LATEST-CANON-SNAPSHOT-V4.md`
- Create: `重庆时间/Pilot-EP03-LATEST-CANON-SNAPSHOT-V4.md`

**Produces:** 302 → failing trunk bridge → seven-minute lifeline causal chain.

- [ ] Step 1: EP01 retains anonymous realtime resident + independent physical evidence + narrow authority + chief physical catch; locate 302 organically near older Jialing River service layers; replace gravity-cause gap with bridge-adjacent Local Gravity Frame handoff instability; seed time divergence without explaining it.
- [ ] Step 2: EP02 concretize the long-supported cross-district structure as a major Jialing River trunk bridge; gravity drift contributes to accumulated load but does not become a single-cause gimmick; forced loss creates the island boundary.
- [ ] Step 3: EP03 convert the existing seven-minute state mismatch into the first explicit crack in shared now; use a low-capacity maintenance bridge through the Jialing network; keep protocol-handshake-complete ≠ reality-connected; integrate Level-2 gravity crossing constraints.
- [ ] Step 4: explicitly create the long causal debt: EP03 bridge succeeds, therefore society reuses it; do not call it iconic yet.
- [ ] Step 5: verify EP01–03 do not mechanically foreground bridge/time/gravity simultaneously; each retains its original dominant dramatic function.
- [ ] Step 6: commit EP01–03 as one physical-foundation batch.

### Task 4: Migrate EP04–EP06 and replace the entire winter/snow chain

**Files:**
- Create: `重庆时间/Pilot-EP04-LATEST-CANON-SNAPSHOT-V4.md`
- Create: `重庆时间/Pilot-EP05-LATEST-CANON-SNAPSHOT-V5.md`
- Create: `重庆时间/Pilot-EP06-LATEST-CANON-SNAPSHOT-V4.md`

**Produces:** emergency infrastructure becomes life → Wedding Mirror/private-time continuity → title episode `重庆时间`.

- [ ] Step 1: EP04 keep cinema/Rashomon/memorial seed/ordinary-life function; make EP03 lifeline visibly routine through schedules/capacity/maintenance; let 嘉陵江 feel lived-in; gravity only in minor physical behavior.
- [ ] Step 2: EP05 preserve Wedding Mirror and T0 ordinary-person flashback; remove every artificial-snow/real-snow/winter bridge; replace its transition function with local-time contrast around the wedding and bridge-shaped life paths.
- [ ] Step 3: ensure EP05 wedding remains a memorial/continuation ritual supported by living friends/family/community and does not imply reconstructed personality = original continuity.
- [ ] Step 4: EP06 remove all dual-season/winter logic and make the episode explicitly about two valid local day/night/public rhythms lacking a common now; retain shared-infrastructure synchronous action and mutually constraining physical reference.
- [ ] Step 5: deliberately keep EP06 gravity mostly compatible so the audience learns time fracture and gravity fracture are independent.
- [ ] Step 6: verify the old EP05 snow ending no longer leaves a transition hole: the wedding's temporal counterpoint must directly create curiosity/pressure that EP06 answers.
- [ ] Step 7: commit EP04–06 as the time-fracture batch.

### Task 5: Migrate EP07–EP08 and turn infrastructure success into political collision

**Files:**
- Create: `重庆时间/Pilot-EP07-LATEST-CANON-SNAPSHOT-V4.md`
- Create: `重庆时间/Pilot-EP08-LATEST-CANON-SNAPSHOT-V3.md`

**Produces:** total-preservation failure → two valid local orders collide on the familiar bridge.

- [ ] Step 1: EP07 retain healthy Hub exit and A/B degraded survival; define Hub as a shared bridge-network municipal node, not an isolated server room; retain Rashomon + EP06 self-limitation + history + real A/B degraded capability as the four-source reframing chain.
- [ ] Step 2: EP08 locate conflict on the same bridge-life family born in EP03 and normalized in EP04, suspended above a bounded Jialing River cavity.
- [ ] Step 3: lock resource asymmetry: one medium quadruped public-security robot/platform on the better-resourced side; multiple ordinary industrial humanoid robots coordinating order on the degraded side; no wheeled security vehicles and no generic military-mecha grammar.
- [ ] Step 4: keep old EP08 no-villain causal result: disarming one side can make it legitimately reclassified as uncontrolled armed platforms and trigger programmatic destruction by the other system.
- [ ] Step 5: use different local times only to worsen operational/authorization mismatch; explicitly state that clock synchronization cannot answer legitimacy.
- [ ] Step 6: commit EP07–08 as the preservation-to-governance batch.

### Task 6: Migrate EP09–EP10 and complete bridge/time/gravity/AI convergence

**Files:**
- Create: `重庆时间/Pilot-EP09-LATEST-CANON-SNAPSHOT-V4.md`
- Create: `重庆时间/Pilot-EP10-LATEST-CANON-SNAPSHOT-V4.md`

**Produces:** first future-boundary test → citywide evacuation/bridge cut/private-AI final cost.

- [ ] Step 1: EP09 retain female chief as minimum-common-reality proposer, upper layer as limited-trial authorizer, and chief as chooser of 302.
- [ ] Step 2: make 302's permanent cost concrete: old local-time compatibility + dedicated Local Gravity Frame/transition support + bridge/service/data/energy/environment/protocol compatibility stack.
- [ ] Step 3: preserve EP01→EP09 mirror: system cannot erase a real 302; reality still does not guarantee a permanent special future promise.
- [ ] Step 4: EP10 transform abstract legacy branch into a still-functioning old district and the final bridge/service/time/gravity/protocol stack connecting it to shared Chongqing.
- [ ] Step 5: make citywide action explicit: evacuate → verify → close/transit/service dependencies → unload gravity transition → end legacy state compatibility → mechanically isolate/separate bridge/district.
- [ ] Step 6: retain three-party action: male = present physical fact; private AI = continuous cross-fragment state mapping/relay; chief = narrow public authorization and cutover recognition.
- [ ] Step 7: retain a real AI-preservation route: keep the old district and compatibility stack active; AI wants to live and helps search for this route; cost is permanent unresolved fragmentation in future Chongqing.
- [ ] Step 8: make the final important bridge the familiar EP03→EP04→EP08 lifeline and explicitly keep it structurally/operationally healthy. No explosion; use staged service and mechanical separation.
- [ ] Step 9: replace unified-winter/snow finale with one shared public now demonstrated by ordinary synchronized life; exact clock digits are execution detail, not required Canon.
- [ ] Step 10: commit EP09–10 as the finale batch.

### Task 7: Rebuild visual execution around Canon V4

**Files:**
- Create: `重庆时间/VISUAL-CONSISTENCY-BIBLE-V2.md`
- Create: `重庆时间/SCENE-PROMPT-TEMPLATE-V2.md`
- Create: `重庆时间/VISUAL-ANCHOR-INDEX-V2.md`

**Produces:** bridge-city/Jialing/time/gravity visual grammar tied to Canon rather than a visual-only rename patch.

- [ ] Step 1: preserve existing aged municipal steel / old white equipment / dark blue-gray / blue hard signage / simplified cel-megastructure / 2–3 hard shadow tiers / 2.35:1 rules.
- [ ] Step 2: promote `第二新重庆市 / SECOND NEW CHONGQING` from visual override into Canon-consistent naming; remove the warning that story Canon is still Beijing.
- [ ] Step 3: add bridge-network composition rules: local ground may exist inside districts, but macro city images must reveal multi-level connectivity rather than default continuous floor.
- [ ] Step 4: add `嘉陵江` visual Canon: colossal enclosed structural canyon, multiple bridge heights, finite engineered boundaries, sparse distant Earth aperture, early→mid→late→EP10 degradation states.
- [ ] Step 5: add day/dusk/night fragmentation visual grammar with no-sky default for enclosed interfaces; signage confirms state rather than explaining it.
- [ ] Step 6: add gravity visual grammar by severity: tilted loose objects/liquid, rail use, robot gait, cargo restraint, rare severe inversion; do not create Escher spectacle in every shot.
- [ ] Step 7: update KV03/EP08 interpretation from ground checkpoint to suspended bridge confrontation; retain user-approved robot resource asymmetry.
- [ ] Step 8: keep KV05 cel simplification principles as active V2 production rules rather than a separate fragile patch dependency.
- [ ] Step 9: update scene prompt handshake fields from `time_or_season_state/weather_state` toward `local_public_time_state`, `gravity_frame_state`, `bridge_connection_state`, `jialing_context`, while keeping weather only where independently relevant.
- [ ] Step 10: commit visual V2 batch.

### Task 8: Rewrite teaser as a consequence of V4, not by find/replace

**Files:**
- Create: `重庆时间/TRAILER-TEASER-V3.md`

**Produces:** 45–60s teaser whose spectacle pool matches V4.

- [ ] Step 1: preserve wedding vow audio spine and serious cel/environmental-storytelling rhythm.
- [ ] Step 2: remove clearing-snow/storm/snow-machine spectacle and every dual-season beat.
- [ ] Step 3: replace those functions with: enclosed day/night interface, Jialing River bridge field, gravity-transition physical detail, EP08 bridge standoff, EP10 procedural bridge separation.
- [ ] Step 4: preserve `将我们分开 → female chief catches falling male` counterpoint if it still fits the cut.
- [ ] Step 5: make the trailer show connections becoming fewer across shots without turning bridge imagery into repetitive wallpaper.
- [ ] Step 6: commit Teaser V3.

### Task 9: Run V4 consistency and no-gap audit

**Files:**
- Create: `重庆时间/consistency-reports/2026-09-01-CHONGQING-TIME-V4-CONSISTENCY-CHECK.md`

**Produces:** evidence that old setting functions were replaced rather than merely removed.

- [ ] Step 1: audit EP01→EP10 bridge progression: network background → failing trunk → temporary lifeline → daily infrastructure → life-path dependency → shared interface/node → armed boundary → future obligation → final bridge cut.
- [ ] Step 2: audit time progression: seed → seven-minute crack → daily divergent rhythms → Wedding emotional counterpoint → EP06 no-common-now → local normalization/authorization effects → governance → final common public now.
- [ ] Step 3: audit gravity progression: EP01 extreme → EP02 structural load → EP03 crossing constraint → EP04 adaptation → EP06 independence demonstration → EP07 degraded service → EP08 embodied boundary → EP09 permanent support cost → EP10 shutdown.
- [ ] Step 4: audit Preservation Paradox: missing reality → forced loss → finite successful connection → life builds on exceptions → continuity limit → one-time cooperation → healthy value exits → complete local protection harms → acknowledge≠permanent preservation → healthy bridge voluntarily ends.
- [ ] Step 5: audit character continuity: male false belief, AI unconditional belonging, chief operational care, EP06 chief↔AI recognition, Rashomon source, memorial practice, AI survival desire, final three-person role split.
- [ ] Step 6: search new Active root for `北京市没有冬天`, `第二新北京`, `BEIJING`, `冬季`, `下雪`, `雪`, `统一冬季`. Every hit must be either an explicit historical/provenance statement or removed; no live V4 fact may rely on them.
- [ ] Step 7: search for bridge/time/gravity references and verify no episode is forced to foreground all three mechanically.
- [ ] Step 8: document every old→new replacement from the mandatory matrix and mark PASS only when successor function is present.
- [ ] Step 9: commit consistency report.

### Task 10: Switch canonical entry points and freeze the old root

**Files:**
- Create: `重庆时间/CURRENT.md`
- Create: `重庆时间/ACTIVE-DOCS-INDEX.md`
- Create: `重庆时间/MIGRATION-SOURCE-INDEX.md`
- Create: `北京市没有冬天/ARCHIVED-PROJECT-REDIRECT.md`
- Modify after archived copies are safely preserved: `北京市没有冬天/CURRENT.md`
- Modify after archived copies are safely preserved: `北京市没有冬天/ACTIVE-DOCS-INDEX.md`

**Produces:** future sessions start from V4 and cannot accidentally mix V3.2.

- [ ] Step 1: write `重庆时间/CURRENT.md` with V4 read order: CURRENT → Active Index → Precedence V4 → Master V4 → World Architecture V4 → Character Relationship V4 → relevant EP V4 → execution docs.
- [ ] Step 2: write Active Index listing exactly one active Master, one world authority, one relationship authority, ten V4 episode snapshots, Visual V2, Prompt V2, Anchor Index V2, Teaser V3, and V4 consistency report.
- [ ] Step 3: write Migration Source Index mapping old active V3.2 sources and decision-log provenance to their V4 destinations.
- [ ] Step 4: add archived-project redirect in old root explaining that historical text is intentionally unchanged and must not be used as active Canon.
- [ ] Step 5: replace old `CURRENT.md` and `ACTIVE-DOCS-INDEX.md` with short redirects to `../重庆时间/CURRENT.md` only after their exact originals exist in the pre-V4 archive batch.
- [ ] Step 6: verify old decision logs/full conversation records remain present and unmodified as provenance.
- [ ] Step 7: final read-back of every Active V4 file and all entry-point links.
- [ ] Step 8: commit activation switch.

## Final completion gate

Do not claim migration complete until all are true:

- `重庆时间/` exists and is the only root designated Active.
- Master V4 + World Architecture V4 contain explicit replacements for every removed Beijing/winter/snow function.
- EP01–EP10 V4 all exist and form the approved organic causal chain.
- EP05→EP06 transition works without snow.
- EP10 outcome works without winter/snow and visibly resolves common time.
- Local Gravity Frames recur after EP01 and have a clear season progression.
- 嘉陵江 is important but not mechanically forced into every episode.
- EP03 familiar lifeline causally reaches EP04, EP08 and EP10.
- Old non-chat source documents have an explicit archived snapshot/provenance path; decision logs/full chats remain provenance, not active Canon.
- New Active root passes residue search for Beijing/winter/snow live-setting remnants.
- New CURRENT/Active Index do not point to superseded V3.2 active files.
- Fresh GitHub read-back confirms written content and file SHAs.