# 《北京市没有冬天》 Master Canon V3 Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build and activate one information-dense Master Canon V3 that becomes the series-level basis for future EP01–EP10 revisions.

**Architecture:** Preserve episode-specific Latest snapshots as factual authority, but introduce a new master series layer that reverse-engineers theme, character, world, motif and episode state changes from the ten-episode macro. Existing Series Bible/Ladders/Checklist remain as derived references; CURRENT and ACTIVE INDEX are updated so future agents read Master V3 before those derivatives.

**Tech Stack:** Markdown documents in GitHub repository `raynacocobobobo-arch/lora`.

**Spec:** `北京市没有冬天/docs/superpowers/specs/2026-09-01-master-canon-v3-design.md`

## Global Constraints

- Source chronology: earliest conversation < middle conversation < latest conversation < later explicit user confirmations.
- Episode-specific `LATEST-CANON-SNAPSHOT` facts override conflicting series-level synthesis.
- Preserve unresolved engineering/dialogue as unresolved; the master may define function and thematic requirement without inventing mechanism.
- Connection becomes the deep story engine; order/sacrifice remains the highest moral axis.
- Correctness, justice and legitimacy must be separated analytically.
- Hand/contact and protocol handshake must be distinguished but made into a recurring season motif.
- No villain simplification, human-supremacy ending, AI-girlfriend framing, hidden upload survival, or perfect reset.

---

### Task 1: Create Master Canon V3

**Files:**
- Create: `北京市没有冬天/BEIJING-NO-WINTER-MASTER-CANON-V3.md`

**Interfaces:**
- Consumes: three conversation records, CURRENT, episode Latest snapshots, existing series-level derived docs.
- Produces: primary series creative basis used by all future episode revisions.

- [ ] Write source/precedence and document-role sections.
- [ ] Write the new thematic hierarchy: connection → order → correctness → justice → legitimacy → dilemma → sacrifice → continuity.
- [ ] Write the six-layer connection model and Hand/Handshake motif architecture.
- [ ] Rewrite the three core character architectures with Want/Need/False Belief/Fear/Leverage/Moral Problem/season transformation.
- [ ] Integrate world, AI, fragmentation, four-layer reality, time, winter, minimum common reality and irreversibility window.
- [ ] Build the EP01–EP10 thematic state matrix with every required column from the design spec.
- [ ] Integrate Reveal, Public Action, Companion Access, Pressure, Dilemma, Order/Justice/Legitimacy and Handshake ladders.
- [ ] Integrate payoff debt, recurring locations/entities, visual motifs, prohibitions and superseded paths.
- [ ] End with future episode-revision rules and an unresolved-decision register.
- [ ] Commit the new Master Canon.

### Task 2: Demote derived series documents and update read order

**Files:**
- Modify: `北京市没有冬天/CURRENT.md`
- Modify: `北京市没有冬天/ACTIVE-DOCS-INDEX.md`
- Modify: `北京市没有冬天/Series-LATEST-CANON-SNAPSHOT-V1.md`
- Modify: `北京市没有冬天/Series-Bible-V2.1-SKILL-COMPLIANT-CANONICAL.md`
- Modify: `北京市没有冬天/Series-Ladders-Payoff-V0.1-CANONICAL.md`
- Modify: `北京市没有冬天/Series-Development-Status-V0.1-SKILL-CHECKLIST.md`

**Interfaces:**
- Consumes: Master Canon V3.
- Produces: deterministic future-agent read order.

- [ ] Put `BEIJING-NO-WINTER-MASTER-CANON-V3.md` immediately after precedence in the substantive read order.
- [ ] Mark older series-level documents as `DERIVED / REFERENCE` without deleting their information.
- [ ] State that episode Latest snapshots remain episode-specific authority.
- [ ] State that future EP rewrites must update Master V3's episode matrix when a macro function changes.
- [ ] Commit entry-point synchronization.

### Task 3: Verification

**Files:**
- Verify all files created/modified above on `main`.

**Interfaces:**
- Consumes: committed repository state.
- Produces: evidence that V3 is active and no unresolved field was silently resolved.

- [ ] Fetch Master V3 from `main` and verify source precedence, theme hierarchy, character architecture, handshake ladder and EP01–EP10 matrix exist.
- [ ] Fetch CURRENT and ACTIVE INDEX and verify Master V3 is first substantive creative document.
- [ ] Search Master V3 for unresolved finale items and confirm they remain explicitly open where mechanism/dialogue is not confirmed.
- [ ] Fetch branch head and record final commit SHA.
