# EP01 Task-Record Gravity Redesign Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Replace EP01's stale-occupancy/cutover engine with the approved task-record → time-offset → gravity-escape → AI safety-choice architecture and repair its direct cross-episode callbacks.

**Architecture:** Keep the existing V4 world and character canon intact, but use the story-causal branch precedence patch to supersede EP01 episode-specific causality. EP01 becomes the authoritative macro story artifact; CURRENT/PATCH/verification and EP02/EP09/EP10 are updated only where they directly reference the superseded EP01 engine.

**Tech Stack:** Markdown story-canon documents in GitHub; Hermes Creative AI Short Drama V1.1 architecture/episode-contract gates.

**Spec:** `重庆时间/docs/superpowers/specs/2026-09-02-ep01-task-record-gravity-redesign.md`

## Global Constraints

- Work only on branch `chongqing-time-story-causal-repair`; do not modify `main`.
- Preserve `CHONGQING-TIME-MASTER-CANON-V4.md`, `WORLD-ARCHITECTURE-CANON-V4.md`, and `CHARACTER-RELATIONSHIP-BIBLE-V4.md` except through branch-scoped precedence where EP01 now conflicts.
- EP01 opening must use an active maintenance task record to establish the world; no lore dump and no delayed orbital-city twist.
- Time and gravity remain independent T0 aftermath axes.
- Exactly one dominant turn: full gravity control becomes available, but the private AI refuses immediate restoration because the current physical state makes restoration lethal.
- Plan B must still aim to reach a safe reset position and restore normal gravity.
- The safe-point recovery must genuinely begin working before latent T0 structural damage invalidates it.
- No early identifiable chief; final human hand only.
- No post-space rescue-device cascade.
- AI local shutdown frees shared suit power for life support + minimum rescue beacon; it is not permanent continuity death.

---

### Task 1: Replace EP01 macro story artifact

**Files:**
- Modify: `重庆时间/Pilot-EP01-LATEST-CANON-SNAPSHOT-V4.md`

**Interfaces:**
- Consumes: approved redesign spec; active world/character canon.
- Produces: authoritative EP01 Episode Card, macro beat architecture, State Delta and continuation capsule for EP02.

- [ ] **Step 1:** Remove all stale occupancy-record / final-clearance / wrong-cutover material from the active EP01 snapshot.
- [ ] **Step 2:** Add task-record opening that establishes Second New Chongqing, T0 aftermath, local operation, local time/gravity and today's 302 reset work order through current action.
- [ ] **Step 3:** Lock the causal chain: routine nodes → final handshake failure → partial handshake reveals `+08:00` → gravity cycle already active → evacuation while handshake continues → full control → AI refuses immediate restore → safe-reset Plan B → genuine recovery success → latent structure fracture → still no-restore → space survival → AI shutdown → final hand.
- [ ] **Step 4:** Rewrite Episode Card so the dominant turn is the AI's refusal to restore immediately, not the time reveal or structural fracture.
- [ ] **Step 5:** Rewrite State Delta and continuation capsule so EP02 opens from rescue/incident responsibility rather than stale occupancy/cutover review.

### Task 2: Update branch precedence and entry point

**Files:**
- Modify: `重庆时间/STORY-CAUSAL-CANON-PATCH-V1.md`
- Modify: `重庆时间/CURRENT.md`

**Interfaces:**
- Consumes: Task 1 authoritative EP01 snapshot.
- Produces: branch read-order/preference rules that prevent the superseded occupancy engine from being resurrected.

- [ ] **Step 1:** Replace PATCH-01/02 EP01 premise and 302 continuity language with the new routine gravity-maintenance/time-reference story.
- [ ] **Step 2:** Update CURRENT critical override and episode map.
- [ ] **Step 3:** Explicitly mark stale-occupancy/cutover EP01 as `SUPERSEDED / NOT_CANON ON THIS BRANCH`.

### Task 3: Repair direct episode callbacks

**Files:**
- Modify: `重庆时间/Pilot-EP02-LATEST-CANON-SNAPSHOT-V4.md`
- Modify: `重庆时间/Pilot-EP09-LATEST-CANON-SNAPSHOT-V4.md`
- Modify: `重庆时间/Pilot-EP10-LATEST-CANON-SNAPSHOT-V4.md`

**Interfaces:**
- Consumes: new EP01 continuation state.
- Produces: season continuity that no longer depends on a stale occupancy record while preserving chief reveal, 302 later use, and finale legacy compatibility.

- [ ] **Step 1:** EP02: replace HOLD-CUTOVER responsibility opening with post-rescue/incident review; keep chief identity reveal and narrow field-fact/public-responsibility split.
- [ ] **Step 2:** EP09: replace stale-history mirror with “current operability must be acknowledged, but does not automatically create permanent future obligation”; preserve 302 as real/occupied/safe/maintainable.
- [ ] **Step 3:** EP10: replace the old EP01→remap callback chain with 302's T0 gravity/time/reference scar → later limited reuse → EP09 boundary trial → final legacy compatibility exit.

### Task 4: Re-run causal verification for changed scope

**Files:**
- Modify: `重庆时间/consistency-reports/2026-09-02-EP01-EP10-STORY-CAUSAL-VERIFICATION-V1.md`

**Interfaces:**
- Consumes: Tasks 1–3.
- Produces: explicit re-verification of EP01 and its EP02/09/10 handoffs.

- [ ] **Step 1:** Replace EP01 verification section with the new Trigger → Goal → Obstacle → Choice → Turn → Cost → State Delta chain.
- [ ] **Step 2:** Update cross-episode 302, Male/Chief and Male/Private-AI spines.
- [ ] **Step 3:** Mark the old EP01 stale-occupancy verification result superseded.
- [ ] **Step 4:** Confirm exact mechanism/dialogue/shot timing remain downstream and are not accidentally locked.

### Task 5: Verify repository state

**Files:**
- Read all files changed in Tasks 1–4.

**Interfaces:**
- Consumes: all prior tasks.
- Produces: evidence that branch docs agree and `main` remains untouched.

- [ ] **Step 1:** Search/read changed docs for forbidden active phrases such as `occupancy record` as EP01 engine, `HOLD CUTOVER`, or early chief involvement.
- [ ] **Step 2:** Verify branch head and compare against `main`.
- [ ] **Step 3:** Report remaining `TBD / VALIDATE_LATER` scopes and do not claim screenplay approval.
