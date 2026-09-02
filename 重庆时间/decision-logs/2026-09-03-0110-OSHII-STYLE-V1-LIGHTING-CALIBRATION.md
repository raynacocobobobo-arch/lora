# Decision Log — Oshii Animation Style V1 Lighting Calibration

- Date: 2026-09-03 01:10 (+08)
- Status: `APPROVED / ACTIVE`
- Scope: non-Canon visual execution layer

## User correction

The previously generated public-observation-hall frames exposed a prompt drift: the active Oshii Style V1 was being interpreted too strongly as flat black-white manga/poster graphics.

The user explicitly corrected the style direction:

- the project needs clear white / off-white structural surfaces;
- lighting structure must be obvious and readable;
- flat/even lighting is incorrect;
- the style must remain suitable for Seedance;
- major environment masters use 2.35:1 for this workflow.

The user then approved the brighter observation-hall result as the correct direction.

## Decision

**Oshii Animation Style V1 remains the name. The style definition is calibrated, not renamed.**

New hard priority:

> **old-white industrial/public structure + strong directional architectural lighting + large hard-edged cel-shaded light/shadow blocks + restrained rust-red accents + low micro-detail Seedance stability.**

The style must no longer be summarized as a flat black-white manga poster look.

## Lighting lock

When a scene has a plausible directional source:

- use strong directional light;
- show large illuminated wall / floor / hull planes;
- use hard-edged architectural cast shadows;
- maintain clear light / midtone / deep-shadow separation;
- light must reveal architecture rather than flatten it.

Forbidden default:

- flat lighting;
- evenly lit gray exposure;
- black-dominant poster-only composition;
- weak structural shadows.

## Color / material lock

Dominant visible architectural material:

> **aged off-white / warm off-white / dirty ivory**

Secondary:

> pale gray / cold gray

Deep shadow / exposed engineering / void:

> charcoal / near-black

Accent:

> restrained muted rust red / oxide red

Black is no longer interpreted as the dominant architectural surface color.

## Seedance rule

Seedance optimization order:

1. preserve major geometry;
2. preserve major directional lighting and cast-shadow shapes;
3. preserve large off-white / gray / charcoal value blocks;
4. preserve major repair / damage landmarks;
5. preserve restrained rust-red distribution;
6. remove fragile micro-detail first.

> **Do not flatten the lighting to make animation easier.**

For major environment production masters, default aspect ratio is `2.35:1` unless another scene-specific ratio is explicitly locked.

## New calibration anchor

Persistent Library image:

> `/重庆时间/visual/style-masters/OSHII_STYLE_V1_LIGHTING_CALIBRATION_HALL_V1.png`

Fingerprint:

- dimensions: `1915 × 821`
- SHA-256: `a991c49eecf481dd2785e7c38587499ea71ff059fed06141b4760a34ff005c31`

Role:

> **LIGHTING / WHITE-MATERIAL / INTERIOR CONTRAST CALIBRATION ANCHOR**

It supplements, but does not replace, the primary space-station style master.

## Files updated

- `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-LOCK.md`
- `docs/visual/2026-09-03-OSHII-ANIMATION-STYLE-V1-PROMPT.md`
- `VISUAL-STYLE-ROUTING-INDEX-V2.md`
- `VISUAL-ANCHOR-INDEX-V4.md`

## Precedence

For visual execution after this decision:

> **current user instruction → current Canon / scene facts → valid geometry anchor → Oshii Style V1 corrected lock/prompt → lighting calibration anchor → Seedance constraints.**
