# 《重庆时间》押井守动画风格 V1 — PROMPT PACKAGE

- Updated: 2026-09-03
- Status: `ACTIVE PROMPT PACKAGE`
- Style lock: `2026-09-03-OSHII-ANIMATION-STYLE-V1-LOCK.md`
- Primary visual master: `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_OSHII_ANIMATION_STYLE_MASTER_V1.png`

---

# 01｜Universal style header

```text
《重庆时间》押井守动画风格 V1。

serious cinematic graphic cel-animation,
manga-inspired hand-drawn architectural background art,
simplified industrial retro-futurist environment,
strong readable silhouettes,
bold structural linework,
large geometric masses,
large shapes first and micro-detail second,
2–3 hard-edged cel-shading tiers,
high-contrast light / midtone / deep-shadow structure,
large areas of black negative space,
restrained hand-drawn mechanical details,
clean readable perspective,
old but operational civic and industrial infrastructure.

Material language:
aged off-white painted structural panels,
dirty ivory,
cold gray secondary structure,
charcoal-black exposed engineering interiors,
very limited muted rust-red / oxide-red accents,
selective red-white industrial identification bands,
occasional faded industrial markings,
weathered civic slogans integrated naturally into physical architecture.

Show long-term use and maintenance through:
large replacement panels,
repair plates,
reinforcement frames,
scarred structural surfaces,
exposed structural sections,
different generations of repairs,
but keep all damage simplified and graphically readable.

Rendering language:
flat graphic surfaces,
clean hand-drawn line art,
minimal gradients,
minimal glossy reflections,
minimal specular highlights,
minimal texture noise,
very low micro-greeble density,
no unnecessary tiny lights,
no excessive wires,
no dense decorative panel lines.

The environment should feel quiet, severe, procedural and lived-in. Public systems and maintenance continue normally inside monumental infrastructure; tension comes from order and operation rather than spectacle.

The image must remain suitable for image-to-video animation:
stable large geometry,
clear structural hierarchy,
simple silhouettes,
large coherent color blocks,
low high-frequency visual noise.

Palette:
black,
charcoal gray,
cold gray,
aged ivory white,
off-white,
small restrained areas of muted rust red.
```

---

# 02｜Universal negative block

```text
no photorealism,
no realistic PBR render,
no glossy metal,
no cinematic lens flare,
no excessive volumetric lighting,
no cyberpunk neon,
no colorful sci-fi lighting,
no dense hard-surface greeble,
no excessive panel lines,
no tiny pipes everywhere,
no excessive antennas,
no excessive small lights,
no overly detailed machinery,
no noisy textures,
no high-frequency surface detail,
no photobash,
no NASA realism,
no generic battleship aesthetic,
no luxury futuristic design,
no polished pristine spacecraft,
no generic premium 3D concept art,
no excessive gradients,
no complex reflections,
no visual clutter,
no floating title text unless explicitly requested,
no infographic callouts,
no technical explanation panels
```

---

# 03｜Seedance stability suffix

```text
animation-friendly environment design,
stable architecture,
stable silhouette,
preserve all major structures,
preserve large geometry,
preserve large color blocking,
preserve major repair locations,
preserve signage locations when visible,
low temporal flicker risk,
low micro-detail density,
no structural mutation,
no new mechanical parts appearing,
no disappearing structural components,
consistent cel-shaded surfaces across frames
```

---

# 04｜Second New Chongqing exterior master prompt

```text
第二新重庆市巨型环形轨道城市完整外景。

保持完整空间站全部进入画面，2.35:1 超宽电影构图，略高三分之四俯视角。

中央是一颗巨大、天然不规则的工程化小行星核心。小行星保持明显岩石材质，以黑、炭灰、中灰的大块面表现；周围有大型结构环、约束结构、工程节点和维护结构。

中央核心通过少量巨大、粗壮、明确的径向结构连接外围环形城市。径向结构数量有限，轮廓清楚，不形成密集自行车轮式结构。

外围是一整圈巨大模块化城市主环。主环由大面积旧白色工业外壳组成，结构厚重、简洁、清晰，不同舱段存在年代差、维修差和替换痕迹。

空间站颜色以黑、旧白、冷灰为主，只有少量锈红 / 氧化红作为维修、结构识别和公共系统强调色；局部允许红白相间的功能识别带，但必须稀疏、具有形式感而不是铺满全站。

保留明显的历史陨石撞击与长期维修区域：大块外壳缺失、内部结构暴露为深黑块面、锈红色加强板、不同年代替换外板、大尺寸维修框架和旧伤痕迹。不要表现为正在爆炸；它是受过严重损伤但仍长期运行的城市结构。

环形外壳上可以存在少量真实建筑标语和公共系统文字。文字必须属于舱体本身，不是海报标题。

可用文字示例：
“团结协作 共同前进”
“科学引领未来”
“第二新重庆市”

不要在画面顶部放置“第二新重庆”或英文电影标题，除非用户明确要求海报排版。

远处为深空背景，地球非常小，只作为距离尺度参考，不得产生近地轨道空间站的视觉感。

整体使用《重庆时间》押井守动画风格 V1：
serious graphic cel-animation,
manga-inspired architectural linework,
hand-drawn industrial background,
large shapes first,
2–3 hard-edged shadow tiers,
large black negative spaces,
simplified structural detail,
clean silhouette,
aged off-white industrial structures,
muted rust-red accents,
minimal texture noise,
minimal highlights,
minimal reflections,
very low micro-greeble density.

画面必须适合 Seedance 2.5 图生视频：结构简单稳定，主轮廓明确，大块颜色统一，细碎信息少，高频纹理少，空间站结构在镜头运动中保持连续。
```

---

# 05｜Text policy

```yaml
floating_film_title: false
in_world_municipal_marking: allowed
in_world_civic_slogan: allowed_when_contextual
infographic_callout: false
explanation_panel: false
```

---

# 06｜Prompt assembly order

```text
[scene facts from screenplay / Spatial Canon]
+
[parent asset geometry constraints]
+
[Oshii Animation Style V1 universal style header]
+
[scene-specific palette / signage / damage state]
+
[Seedance stability suffix if required]
+
[universal negative block]
```

Never let the style section overwrite scene facts.
