# 《重庆时间》EP01 Task-Record / Gravity Redesign Spec

- Date: 2026-09-02
- Branch: `chongqing-time-story-causal-repair`
- Scope: EP01 macro story architecture only
- Status: `APPROVED DIRECTION / IMPLEMENT ON REPAIR BRANCH`

## Goal

Replace the stale-occupancy/cutover EP01 engine with one coherent pilot story:

> **A routine 302 gravity-reference maintenance task exposes an eight-minute split between Chongqing public time and 302 local time. The gravity instability window has already begun. The private AI eventually gains full gravity-control authority, but restoring nominal gravity immediately would kill the male operator, so she delays restoration and routes him toward a safe reset position. They nearly complete the original task, then a latent T0 structural fracture invalidates the safe point. The AI again concludes that not restoring gravity is the least-bad option, abandons task completion in favor of his survival, later powers down to preserve life support, and an unidentified human hand catches him as he loses consciousness.**

## Pilot opening function

EP01 must establish the world through an active **maintenance task record**, not a lore lecture and not a delayed “they are in space” twist.

The opening must make the following legible through one ordinary work commute / task intake:

1. the setting is **第二新重庆市**, a layered bridge-network orbital megacity;
2. T0 meteor impact happened before EP01 and the city is in long-term repair/recovery;
3. districts can run `LOCAL OPERATION` with local public time and Local Gravity Frames;
4. the citywide/common reference is degraded;
5. bridges/interfaces carry people plus time/gravity/protocol handoff;
6. male + private AI are already a mature everyday/work pair;
7. today's task is routine: establish trusted handshake, reset 302 gravity reference, leave before the safe reset window closes.

World exposition must remain action-bound. No historical prologue, no encyclopedia voice-over, no council briefing.

## Episode dramatic architecture

### Cold Open — task record / ordinary city

A normal working day. Public transit, layered bridges, different local light/service states, maintenance activity and ordinary residents establish that the city still lives.

The maintenance record narrows from city status to today's 302 work order:

> T0 aftermath maintenance → 302 local operation → gravity-reference reset → public/local handshake required → safe reset window.

The AI and male treat this as familiar work.

### Pressure 1 — routine task mostly works

The pair successfully clear early nodes. Only the final handshake layer fails. Small gravity-drift evidence appears but is consistent with the known job, so neither behaves foolishly or panics.

The physical reason the male must be there: remote systems cannot create a trusted local/public reference; he must bridge an old disaster relay from the current physical site while the AI performs protocol and model work.

### Pressure 2 — partial handshake reveals the real clock

A partial handshake restores a trusted local safety/time channel but not full gravity control.

For the first time both references are trustworthy and visible:

- `CHONGQING PUBLIC`
- `302 LOCAL`
- offset: `+08:00`

The safe reset window is already expired. The 302 gravity re-lock/instability cycle has therefore already begun.

Time does **not** cause gravity failure. They are independent T0 aftermath axes; bad shared time mapping caused the crew to misjudge where the known gravity cycle already was.

### Dominant Turn — full control arrives too late for the original action

During evacuation, the AI continues the handshake over the physical bridge the male already established.

`FULL HANDSHAKE` succeeds. The AI can restore nominal gravity.

The male asks to restore. She refuses because the real current geometry has already changed: the male, debris and structural loads are displaced under the abnormal vector. Immediate nominal restoration would reverse loads and make his survival near-zero.

This is the episode's **single dominant turn**:

> **The goal changes from “restore gravity now” to “delay restoration until he reaches a safe reset position.”**

The AI is not choosing permanent abnormal gravity. Her Plan B still ends with normal gravity restored and the maintenance task completed.

### Payoff — exploit the bad state to reach a safe reset point

The abnormal vector becomes the only usable route toward an outer-hull gravity transition / emergency reset position.

The male physically moves through the changing ruined geometry while the AI navigates and controls what she can. The target remains singular: reach the safe reset position, secure him, then restore gravity.

He reaches it and is genuinely secured / being recovered. The AI prepares `RESTORE` and both believe the task is about to end.

### Cost after solution — the safe point itself ceases to be safe

A latent meteor-impact fracture, not fully observable beforehand, propagates under prolonged abnormal loading and tears the safe reset anchor/supporting structure loose.

The plan was valid. The male did not miss. The AI did not make a stupid calculation. The supporting physical reality changed after the plan had begun succeeding.

The AI reassesses whether to restore nominal gravity. The answer remains **do not restore** because the male is now near/beyond the hull boundary with outward velocity while restoration would still reverse debris/loads without returning him safely.

This is not a second dominant turn; it is the cost that proves the first turn's rule under a worse state.

### End progression — task gives way to survival

The male crosses beyond the Local Gravity Frame. Artificial acceleration ends; inertia carries him outward.

The AI uses EVA capability only to stop rotation and reduce outbound relative speed. Those actions succeed but cannot provide enough delta-v to return him.

The story then decelerates. No new device cascade.

As suit power becomes critical, the AI shuts down high-compute search/modeling first. When even the local AI core measurably reduces remaining life-support time, she powers down completely and leaves power to life support + minimum rescue beacon.

Approved final dialogue direction:

> “我很抱歉。”
>
> “祝你早安……晚安。”

No dialogue after AI shutdown.

The male nearly loses consciousness. An unidentified EVA-gloved human hand catches his wrist; a second hand moves to his rescue ring/tether. Cut to black. The rescuer's identity is revealed in EP02, not in EP01.

## Character functions

### Male

- current physical operator;
- must physically establish the trusted local bridge;
- survives by executing in changing geometry rather than by possessing omniscient knowledge;
- his field presence materially changes what the AI/system can know and do;
- EP01 reinforces his temptation to equate value with irreplaceable field presence, without giving him broad authority.

### Private AI

- broad historical/protocol/model access;
- mature companion relationship already established before the episode;
- independently refuses the male's immediate restore command because it is unsafe;
- proposes a complete Plan B rather than merely “keeping gravity broken”;
- first wound: correct reasoning can still be defeated by a newly revealed physical fact;
- voluntarily shuts down only after no viable return path remains and doing so extends the male's life-support window.

### Female chief

- no early POV, no opening involvement, no visible managerial framing;
- only enters physically in the last image as the unidentified rescuer;
- EP02 reveals her identity and formalizes responsibility/public authorization.

## Hard prohibitions

- no stale occupancy-record engine;
- no hidden/current resident rescue in EP01;
- no early chief POV or identifiable chief reveal;
- no “time error causes gravity failure” causation;
- no random 180-degree magic flip as the only gravity grammar; use escalating vector instability / re-lock cascade;
- no omnipotent AI;
- no restore-normal-is-always-good rule;
- no repeated drone/hoist/device failure cascade after entering space;
- no vacuum-suction explanation;
- no fake rescue miss: the safe-point recovery must actually begin working before latent structure failure interrupts it;
- no “AI becomes a battery”; shutdown frees shared suit power draw;
- no permanent AI death claim from EP01 local shutdown;
- no explanatory line after the final hand appears.

## Cross-episode consequences to preserve

- EP02: the unidentified rescuer is revealed as the current/new chief; male physical fact and chief public responsibility become formal complementary roles.
- EP04/09: 302 remains a real old district/service node capable of later limited use; EP01 no longer supplies a stale-occupancy remap story.
- EP09 mirror changes to: current reality and current operability must be acknowledged, but neither automatically creates a permanent future public obligation.
- EP10 can still return to 302/legacy compatibility, but not through the old “EP01 proved a hidden resident existed” callback.
- Series grammar seeded by EP01:
  - `system functioning != shared reality intact`;
  - `restore normal != safest current action`;
  - `correct plan != guaranteed outcome`;
  - `present physical fact retains final veto over models`.
