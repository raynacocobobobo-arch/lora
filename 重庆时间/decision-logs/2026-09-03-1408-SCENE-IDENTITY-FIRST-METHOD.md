# Decision Log — Scene Identity First

- Date: 2026-09-03 14:08 (+08)
- Status: `APPROVED / ACTIVE`
- Scope: environment image-generation methodology

## Problem observed

A generated 302 public/lived image matched the project style and Seedance detail target, but read as a generic old future-city corridor. The failure was not primarily style drift; it was loss of scene identity.

Root cause:

> style + Seedance simplification were applied before the parent-space relationship and scene-defining physical cues were locked.

## Locked method

Future environment generation order:

> **Canon facts → scene identity → parent-space relation → semantic anchors → style → Seedance compression → generation → QC.**

Hard rule:

> **If changing the sign could relabel the image as another generic district, the scene is not ready to generate.**

Seedance rule:

> **删噪声，不删身份。**

High-frequency detail may be removed, but large physical cues that explain history, function, parent-space relation, bridge scale or episode action must survive.

## 302 consequence

When generating 302, read `SPATIAL-ENVIRONMENT-CANON-PATCH-V2.2-302-ORIGIN-LAYER.md`.

The outer lived/public layer must show genuine civic life while retaining a few large inherited industrial/logistics cues. The asteroid mining origin layer remains mainly an EP09/EP10 location and should not be inserted into EP01 merely to make 302 recognizable.

## Files updated

- `SCENE-PROMPT-TEMPLATE-V2.md`
- `VISUAL-STYLE-ROUTING-INDEX-V2.md`
