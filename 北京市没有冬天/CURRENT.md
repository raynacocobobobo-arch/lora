# 《北京市没有冬天》CURRENT — Canonical Entry Point

- Updated: 2026-09-01
- Status: `LOCKED / MASTER V3.2 ACTIVE / EPISODE CARD MACRO PASS IN PROGRESS`
- Purpose: future ChatGPT / Codex / Agent sessions MUST start here.
- Detailed architecture log: `decision-logs/2026-09-01-1000plus-DETAILED.md`
- Latest episode/workflow log: `decision-logs/2026-09-01-1113-EP03-DRAMA-SKILL-DETAILED.md`

---

# 01｜Canonical precedence

1. **later explicit user confirmation**;
2. **highest-numbered active `Pilot-EPXX-LATEST-CANON-SNAPSHOT-V*.md`** for concrete episode facts;
3. **`BEIJING-NO-WINTER-MASTER-CANON-V3.2.md`** for current series architecture, season dynamics, character arcs, theme hierarchy, Hand/Handshake structure and episode-revision criteria;
4. retained derived series references;
5. archived historical Canon / superseded Masters / patches.

Source chronology:

> **最早对话记录(1).md < 中间对话记录.md < 对话记录.md < later explicit user confirmation**

Rules:

- `TBD` remains unresolved;
- `NEEDS_REVIEW` remains unresolved;
- do not silently overwrite a LOCKED matter;
- when a new Master becomes active, the old Master leaves the active root and is recorded under `archive/master-canon/` / Git history;
- architecture-level Git revisions must preserve a detailed Decision Log, not only extracted slogans;
- when the user approves a significant episode/architecture revision, Git both the **current Canon** and a **detailed Decision Log preserving the original discussion semantics**.

---

# 02｜Primary read order

1. `CANON-PRECEDENCE-V0.1-LATEST-CONVERSATION-WINS.md`
2. `ACTIVE-DOCS-INDEX.md`
3. **`BEIJING-NO-WINTER-MASTER-CANON-V3.2.md`**
4. **`Pilot-EP01-LATEST-CANON-SNAPSHOT-V2.md`**
5. **`Pilot-EP02-LATEST-CANON-SNAPSHOT-V2.md`**
6. **`Pilot-EP03-LATEST-CANON-SNAPSHOT-V2.md`**
7. `Pilot-EP04-LATEST-CANON-SNAPSHOT-V1.md`
8. `Pilot-EP05-LATEST-CANON-SNAPSHOT-V1.md`
9. **`Pilot-EP06-LATEST-CANON-SNAPSHOT-V2.md`**
10. **`Pilot-EP07-LATEST-CANON-SNAPSHOT-V2.md`**
11. `Pilot-EP08-LATEST-CANON-SNAPSHOT-V1.md`
12. **`Pilot-EP09-LATEST-CANON-SNAPSHOT-V2.md`**
13. `Pilot-EP10-LATEST-CANON-SNAPSHOT-V1.md`

For architecture reasoning/history, read the relevant `decision-logs/` entry before reopening raw conversation records.

---

# 03｜Drama Skill is now a HARD GATE for episode development

`LOCKED WORKFLOW RULE`

This project is not a worldbuilding archive. It is a pure-AI serialized short drama intended to proceed all the way to screenplay, storyboard, Shot Specs and a Seedance-oriented Production Pack.

Current drama skill authority:

> **Hermes Creative AI Short Drama V1.1**

Source repo:

> `raynacocobobobo-arch/skills-share/plugins/hermes-skills/skills/hermes-creative-ai-short-drama/`

For **every episode revision / creation from now on**, after loading Canon, explicitly read the current:

1. `SKILL.md`;
2. `workflows/create-episode.md`;
3. `references/episode-contract.md` when building/reviewing the Episode Card;
4. `references/story-architecture.md` when checking episode differentiation, progression, callbacks, third-path cost or finale setup.

Division of responsibility:

> **Canon answers: what cannot drift, why characters/world reached this state, what persists across episodes.**
>
> **Drama Skill answers: why this is an episode worth watching — Hook, Pressure, one Dominant Turn, conflict grammar, observable payoff, changed end meaning and next prediction.**

Do not substitute one for the other.

Current `create-episode` order:

> **load canon → prior-function audit → Episode Card → macro approval → screenplay → State Delta draft → Continuation Capsule draft**

Therefore future Episode Latest revisions should, where practical, include / satisfy:

- Prior Episode Function Audit;
- Episode Card;
- exactly one Dominant Turn;
- Core Conflict / Conflict Grammar;
- Novelty vs Prior;
- Reveal / Public Action / Relationship progression;
- Callback / Debt;
- Cost after solution;
- Observable Payoff / Progress;
- Ending Cliffhanger / End Image;
- Draft State Delta;
- Draft Continuation Capsule;
- mechanism/dialogue approval scope kept separate.

---

# 04｜Production direction — do not remain in Canon Revision forever

`LOCKED WORKFLOW DIRECTION`

Full intended chain:

> **revise-canon → create-episode → screenplay → Continuity State / Shot Specs → asset & keyframe plan → Generation Segments → Seedance Production Pack → actual media Review / Retake when output exists**

Current project phase:

> **one bounded final Macro / Episode Card pass across EP01–EP10.**

### Macro-pass exit condition

Once all ten episodes have:

- macro-approved Episode Card / equivalent contract;
- clear one-episode dramatic function;
- no key cross-episode contradiction;
- State Delta intent;
- usable Continuation Capsule;
- unresolved mechanism/dialogue correctly marked TBD;

then:

> **STOP broad Series Architecture restructuring and switch to screenplay production from EP01 forward.**

Do not keep adding theory indefinitely unless screenplay reveals a real contradiction.

### After the macro pass

**Phase B — Screenplay**

> EP01 screenplay → review → EP02 screenplay → review → …

Lock scene IDs, visible actions, dialogue, scene end states, final State Delta and final Continuation Capsule.

**Phase C — Storyboard / continuity**

> screenplay → asset inventory → continuity compile → fewest readable Shot Specs

Prefer one visible action per Shot.

**Phase D — Seedance Production Pack**

> validated shots → asset/keyframe readiness → Generation Segments → generation mode → prompt/NOT constraints → `READY / BLOCKED / NEEDS_REVIEW`

Without actual generated media, never claim `PASS`.

---

# 05｜Current season axis — Master V3.2

The season is NOT:

> characters gradually learn sacrifice is the right answer.

Locked sequence:

> **EP01–EP06：尽可能全部保存。**
>
> **EP07：第一次在局部案件中承认“全部保存”已经失败。**
>
> **EP08：证明完整保全目标会产生系统级次生灾害 / 制度暴力。**
>
> **EP09：把 EP07–08 已经证明的事实制度化为最低共同现实。**
>
> **EP10：城市级主动执行新的共同边界；同一原则落到私人 AI 与男主自己。**

Internal structure:

> **被动失血 → 局部保存目标裂开 → 保全悖论系统级爆发 → 制度化新目标 → 主动失血 / 向死而生。**

## Preservation Paradox

> **每个系统都在正确保护自己负责的部分；共同前提破坏后，局部保全会把资源、规则、权限、时间和基础设施锁进不同现实，整体北京反而越来越无法维持。**

Secondary disaster is:

> **the externality of locally correct preservation under broken common conditions.**

---

# 06｜Hidden social-structure reference — INTERNAL ONLY

`LOCKED / NEVER EXPLICIT ALLEGORY`

For EP02→EP08 social evolution:

> **临时措施 → 临时例外 → 必要通道 → 重复使用 → 例外常态化 → 新生活依赖 → 制度沉积 → 新秩序 → 新正当性冲突。**

This is structural reference only, never an explicit COVID / lockdown allegory.

Hard requirement:

> **结构可以借，表征必须彻底换掉。**

No recognizable epidemic-policy imagery, terminology, testing analogues, quarantine-camp analogues, color-pass systems, slogans or one-to-one real events.

Critical cross-episode consequence:

> **EP03 的一次医疗连接因为真的救过人而被重复依赖，逐步沉积成公共通道、管理边界与两套秩序重叠点，最终自然解释 EP08 的检查点。**

Internal regional-interest rule:

> **你口中的恢复，对我可能是第二次失序。**

Not mandatory dialogue.

---

# 07｜Three levels of loss

## L1｜Forced Loss — EP01–EP06

- disaster creates incompatible conditions first;
- everyone still tries to preserve as much as possible;
- no one yet accepts a smaller future Beijing as the goal.

## L2｜Local Preservation Break / Tactical Sacrifice — EP07

- hub is actively and irreversibly removed;
- A+B remain the preservation objective;
- first local admission A+B+hub cannot all be saved;
- not yet a smaller future community.

## L3｜Institutionalized Boundary / Active Contraction — EP09–EP10

- EP09 turns “cannot preserve everything” into public governance;
- EP10 executes it at city scale;
- people should be migrated / evacuated in advance;
- contraction targets continuing operations, old links, permanent exceptions, regional public states and some digital continuities, not last-second abandonment of living residents.

---

# 08｜AI principle-consistency arc — LOCKED

### EP06 — experience

> **共同规则也必须约束拥有权力的人自己。**

AI experiences chief's limited use of private AI, shared-reference constraint, and authority boundaries.

### EP07 — internalization

Locked line:

> **“我看不见外面，所以我开始读你们已经留下来的东西。”**

Internal principle:

> **规则如果只在代价落到别人身上时成立，就不是共同规则。**

### EP09 — self-application

AI independently concludes 302 should exit, then realizes the principle may reach her own continuity.

> **She does not want to leave.**

### EP10 — consequence

> **She cannot invalidate the principle merely because she is now paying the cost.**

---

# 09｜Male exception rule — LOCKED CORRECTION

“不能在原则落到自己这里以后突然要求例外” does NOT mean the male cannot try to save the private AI.

> **He MUST first try.**

Migration, backup nodes, delay, copy/new instance, continuity-preserving options, temporary exceptions and a real third path may all be investigated.

Actual test:

> if preserving the same continuous AI requires a permanent private exception that cannot be generalized and keeps consuming scarce common-city operating conditions, he does not convert private attachment into permanent public privilege.

---

# 10｜Handshake Ladder — current

- EP01 — failed handshake / verification ≠ nonexistence;
- EP02 — no forced handshake motif;
- EP03 — handshake complete ≠ physical connection;
- EP05 — reconstructed hand / ring / contact;
- EP06 — no shared reference → no trustworthy handshake;
- EP08 — mutual authorization handshake fails; protected-person constraint remains;
- EP09 — define future minimum mutually confirmable states;
- EP10 — spoken “握手” + unreachable human hand + real technical handshake.

Technical handshake ≠ upload / fusion / migration / continuity preservation.

---

# 11｜EP03 V2 — CURRENT AUTHORITY / Drama Skill Episode Card pass complete

Current file:

> **`Pilot-EP03-LATEST-CANON-SNAPSHOT-V2.md`**

Approval scope:

> **macro structure / episode function / causal consequences LOCKED; exact mechanism, dialogue, names, scene/shot timing remain TBD.**

Dominant Turn:

> **两个区域都认为对接已经完成，但现实中的可通行状态没有真正重合；男主重新找到真实物理窗口，女科长只授权这一次，药真正过去。北京没有恢复连接；他们只是把一次连接做成了。**

Key V2 changes:

1. EP02 handoff corrected: accident tore the connection; everyone salvaged it but could not fully save it;
2. seven minutes remains but is NOT locked as a simple clock difference;
3. ordinary technical `handshake complete` becomes visible/audible, but does not equal physical connection;
4. conflict grammar = complete public procedure not restored vs an essential medical action cannot wait;
5. chief uses sufficient facts + sufficient authorization for this action only;
6. male gets positive reinforcement that broken Beijing needs his field judgment;
7. private AI experiences “seeing both sides ≠ possessing the physical relationship between them”;
8. successful rescue itself creates future dependency: repeated need → maintenance → ordering → safety confirmation → management → de facto public corridor → EP08 overlap;
9. medical girl remains the same person who naturally returns in EP08;
10. V2 includes a Drama Skill Prior-Function Audit, Episode Card, Draft State Delta and Draft Continuation Capsule.

Core long-term rule:

> **EP08 的问题不是 EP03 的失败造成的；恰恰是 EP03 成功以后才可能出现。**

---

# 12｜Current active episode versions

| Episode | Active Latest Snapshot | Macro / Drama Skill status |
|---|---|---|
| EP01 | `Pilot-EP01-LATEST-CANON-SNAPSHOT-V2.md` | `MACRO V3 PASS DONE / formal card retrofit later if needed` |
| EP02 | `Pilot-EP02-LATEST-CANON-SNAPSHOT-V2.md` | `MACRO V3 PASS DONE / formal card retrofit later if needed` |
| **EP03** | **`Pilot-EP03-LATEST-CANON-SNAPSHOT-V2.md`** | **`DONE — Drama Skill Episode Card pass`** |
| EP04 | `Pilot-EP04-LATEST-CANON-SNAPSHOT-V1.md` | **`NEXT`** |
| EP05 | `Pilot-EP05-LATEST-CANON-SNAPSHOT-V1.md` | `PENDING` |
| EP06 | `Pilot-EP06-LATEST-CANON-SNAPSHOT-V2.md` | `MACRO principle-learning pass done / card audit later` |
| EP07 | `Pilot-EP07-LATEST-CANON-SNAPSHOT-V2.md` | `MACRO preservation-break pass done / card audit later` |
| EP08 | `Pilot-EP08-LATEST-CANON-SNAPSHOT-V1.md` | `PENDING — needs V3.2 + institutional-sediment pass` |
| EP09 | `Pilot-EP09-LATEST-CANON-SNAPSHOT-V2.md` | `MACRO institutionalization pass done / card audit later` |
| EP10 | `Pilot-EP10-LATEST-CANON-SNAPSHOT-V1.md` | `PENDING` |

Current bounded macro sequence:

> **EP04 → EP05 → audit/retrofit EP06 → audit/retrofit EP07 → EP08 V2 → audit/retrofit EP09 → EP10 V2 → final ten-card consistency check → SCREENPLAY PHASE.**

EP01/02 formal Episode Cards can be retrofitted during the final consistency check if their V2 files do not already contain all required contract fields; do not re-architect them without cause.

---

# 13｜Current macro that must not drift

1. EP01 — 302 / existence / world reveal / one-point model-reality failure.
2. EP02 — islanding / failing bridge / forced salvage / people still believe restoration is the goal.
3. **EP03 — medicine / seven-minute physical-window mismatch / one real connection / handshake complete ≠ physical contact / successful temporary exception begins repeat-use dependency.**
4. EP04 — daily work / cinema / Rashomon / ordinary life sustained under fragmented reality / temporary exceptions begin to feel like normal life.
5. EP05 — Wedding Mirror / representation vs continuity / hand-ring-snow motif.
6. EP06 — winter divergence / shared physical reference / three-way relay / AI learns common rules also bind power-holders.
7. EP07 — shared hub / first local admission total preservation failed / AI internalizes principle consistency.
8. EP08 — two security orders preserve correctly and still create institutional violence / checkpoint grows from accumulated management needs.
9. EP09 — minimum common reality / 302 / institutionalize cannot-preserve-everything / hidden AI farewell.
10. EP10 — strategic active contraction / male first tries to preserve AI / final handshake / farewells / one public now / winter.

---

# 14｜Highest unresolved finale items remain open

- female chief's exact EP10 physical onsite action;
- final handshake's minimum necessary technical function;
- why the continuous old private-AI subject must participate;
- male's concrete preservation attempts;
- exact threshold / visible indicators of islanding irreversibility;
- public/private/city intercut order;
- multilingual farewell justification;
- EP10 remaining two theme words;
- final city shot / title placement;
- final dialogue.

Do not resolve these merely to complete an Episode Card unless they actually affect the card's causal validity; otherwise keep TBD.

---

# 15｜Document governance

Primary series architecture:

> **`BEIJING-NO-WINTER-MASTER-CANON-V3.2.md`**

Detailed recent architecture history:

> `decision-logs/2026-09-01-1000plus-DETAILED.md`

Detailed EP03 approval + Drama Skill workflow history:

> **`decision-logs/2026-09-01-1113-EP03-DRAMA-SKILL-DETAILED.md`**

Superseded Master provenance:

> `archive/master-canon/README.md`

Current episode authority:

> **use the highest-numbered active Latest Snapshot per episode.**

Future approved architecture/episode Git rule:

> **write current Canon + detailed Decision Log preserving original user wording/semantic context, rejected interpretation, why it changed, exact boundaries and downstream consequences.**
