# 《重庆时间》DUNGEON STYLE PROMPT V1

- Updated: 2026-09-03
- Internal style name: **地牢风格 / DUNGEON STYLE**
- Status: `ACTIVE PROMPT / DEFAULT NEW SETTING-ART STYLE`
- Style lock: `2026-09-03-DUNGEON-STYLE-VISUAL-ASSET-LOCK-V1.md`
- Production master image: `/重庆时间/visual/style-masters/SECOND_NEW_CHONGQING_DUNGEON_STYLE_MASTER_V1.png`

---

# 00｜Usage rule

This prompt does not determine story facts.

Before using it, insert the exact scene facts from current Canon / episode / screenplay.

Prompt structure:

> **SCRIPT FACTS → SPATIAL FACTS → DUNGEON STYLE BLOCK → SCENE-SPECIFIC COMPOSITION → NEGATIVE / ANTI-DRIFT**

Do not use the style block as a substitute for reading the script.

---

# 01｜Universal Dungeon Style block — Chinese

```text
沿用《重庆时间》“地牢风格 / DUNGEON STYLE”统一视觉系统。

画面采用高度图形化、强设计感、成熟克制的未来工业赛璐璐插画语言。黑、旧白、灰构成主要视觉关系，使用大面积黑色负空间、浅灰白结构块、深灰承力结构和少量锈红/褪色工业红作为功能性强调色。局部可以使用红白相间的模块识别条带、维修区段涂装或市政工程分区标识，但红色保持克制，不覆盖整个画面。

优先保证大轮廓、大结构、大黑白关系和一眼可读的空间关系。所有设备和建筑先用3–5个大块面建立，再补少量必要结构线。线稿明确、略带手绘不规则感，不做CAD式密集机械描线。明暗以2–3档硬边赛璐璐阴影为主，大片暗部直接归入黑色或深炭灰，不依靠体积雾、镜面高光和复杂渐变制造高级感。

材质是老旧但长期维护运行中的公共工业设施：旧白喷涂板、深灰结构框架、黑色密封/关节、锈红维修模块、补丁板、替换结构、裸露的少量加固构件。保留使用、磨损、陨石损伤和维修历史，但损伤表达以大块结构缺失、烧蚀暗区、后装加固框和异色替换板为主，不铺满无数裂纹和细碎锈迹。

整体具有强烈平面设计意识。黑色区域作为主动构图，不要把所有黑色区域填满细管、灯点和星星。结构在缩略图尺寸下仍然清楚。

文字如果出现，必须是画面世界内部的正式城市/公共设施文字，直接印刷或喷涂在结构表面，少而大，参与构图，不做浮在画面上方的电影标题，不做说明图，不做密集参数标注。允许根据场景使用大型市政标识、区域编号或少量公共标语。

适合 Seedance 图生视频：压低高频细节，减少密集小窗、小灯、天线、细管、微型桁架和面板缝；保持主结构轮廓、红白条带、维修区、人物/机器大形体稳定。优先时序稳定性而不是静帧微细节密度。

整体气质：巨大、安静、克制、公共、工业、旧而仍在工作；不是废土，不是豪华太空船，不是霓虹赛博朋克，不是写实3D硬表面概念图。
```

---

# 02｜Universal Dungeon Style block — English

```text
Use the approved CHONGQING TIME “DUNGEON STYLE” visual system.

Create a highly graphic, design-forward, mature industrial cel-illustration. Build the image primarily from deep black negative space, aged off-white structural masses, controlled mid-gray/deep-gray frames, and only a small amount of muted rust-red / faded industrial red as functional accent. Selected red-white alternating bands may appear as module identification, repair-sector paint, engineering zoning or municipal functional markings, but red must remain subordinate to the black-white composition.

Prioritize macro silhouette, large structural relationships and strong black-white shape design. Construct architecture and equipment from a few large masses first, then add only necessary structural lines. Use clear slightly hand-drawn linework rather than dense CAD-like mechanical outlines. Lighting uses 2–3 hard-edged cel-shading tiers with large black/charcoal shadow masses. Avoid relying on volumetric fog, glossy reflections, complex gradients or micro-greeble for visual richness.

Materials feel old, public, industrial, repaired and continuously maintained: aged off-white painted shells, deep gray structural frames, black seals/joints, rust-red legacy or repair modules, replacement plates and selective exposed reinforcement. Damage history remains visible but simplified into large readable events: missing/torn shell, dark ablation zones, reinforcement frames, mismatched replacement modules and aged repair patches rather than thousands of small cracks.

Treat black negative space as an active graphic design element. Do not fill every dark region with pipes, tiny lights, stars or texture. The main structure must remain readable at thumbnail scale.

If text appears, it must exist inside the world as large civic/municipal graphics painted or printed on physical structures. Use very few large words. Do not place a floating movie title over the image, do not create an infographic, and do not fill surfaces with tiny technical labels.

Seedance-friendly design: suppress high-frequency detail, dense windows, tiny lights, antennas, pipe bundles, miniature trusses and excessive panel seams. Preserve stable silhouettes, large red-white pattern blocks, repair landmarks and large-scale object identity across frames.

Mood: monumental, quiet, restrained, civic, industrial, old but operational. Not wasteland, not luxury sci-fi, not cyberpunk neon, not photoreal 3D hard-surface concept art.
```

---

# 03｜Scene prompt template

```text
【CANON / 剧本事实】
场景：<填写当前剧本中的真实地点>
时间/Local Public Time：<填写>
本场主要动作/状态：<填写>
人物/机器人/设备：<填写>
桥/接口物理尺度：<如适用，填写 Level 1/2/3/4 或实际功能>
必须保留的跨集资产：<填写>
禁止出现的剧情内容：<填写>

【空间关系】
父级城市资产：<填写>
一眼应该读到的主要空间关系：<填写>
空间边界：<填写>
对岸/相邻模块/临空关系：<填写>

【DUNGEON STYLE】
<粘贴 Universal Dungeon Style block>

【构图】
2.35:1 cinematic setting image unless otherwise specified.
One dominant spatial relationship, one dominant scene state.
Large shapes first, strong black-white negative-space design.
Do not copy the exterior ring composition unless this is actually an exterior ring-city shot.

【场景专属视觉元素】
<填入例如：小桥、桥头四足机器人、普通工业人形机器人、站厅、旧白列车、维修平台等>

【文字】
<无文字 / 第二新重庆市 / 区域编号 / 单条标语，根据本场设定填写>
Text must be in-world and physically integrated.

【损伤/维修】
<无 / 一般维修 / T0旧伤 / 退化资源侧，按剧本填写>

【Seedance 优化】
Stable macro silhouette.
Suppress micro detail and repetitive tiny elements.
Preserve major object positions and graphic color blocks.
```

---

# 04｜Second New Chongqing exterior style prompt

Use when the user asks for the macro city exterior or a related exterior derivative.

```text
严格继承第二新重庆市当前小行星核心环城 Canon 和已批准的宏观构型：中央工程化小行星核心、外围闭合永久环形城市骨架、有限数量粗壮径向结构、模块化城区环、明显但长期修复中的 T0 撞击区、远距离小地球。

在几何结构正确的前提下，采用“地牢风格 / DUNGEON STYLE”：深黑宇宙负空间，主体以旧白和浅灰大块面为主，深灰/黑色结构层，少量锈红工业模块。局部加入清楚的红白相间工程分段条带，条带与模块/维修/识别逻辑一致，不随机装饰。

整体进一步风格化：减少小天线、小灯、小面板和密集桁架，保留少数大节点和大结构缝。中央小行星使用黑灰大块岩面，保持天然岩体轮廓，不做照片级石头纹理。

T0 旧伤集中在一个可识别环段：局部白色外壳撕裂或缺失，深层黑色结构暴露，锈红维修带和后装加固构件形成强烈设计性图形，但无主动爆炸。

可在结构表面出现大型世界内文字，例如“第二新重庆市”作为市政身份标识；如果需要公共标语，只保留一条主要标语。禁止在画面顶部放片名式“第二新重庆”标题。

高对比度、平面设计感、手绘工业线条、2–3档硬阴影、大形优先、低高频噪声、适合 Seedance 图生视频。
```

---

# 05｜Interior / public-space adaptation

For an interior city setting, do NOT force outer-space black background. Transfer the graphic system by using architectural darkness/negative space.

```text
Interior Dungeon Style adaptation:
use large off-white wall/beam/platform masses against deep black or charcoal service voids, shadow wells, ceiling gaps and dark background bays. Use muted rust-red bands on selected columns, gates, repair modules or public-equipment zones. Keep linework sparse and architectural. Reduce screen/light clutter. Preserve normal public activity and functional circulation from the script.
```

---

# 06｜Robot / equipment adaptation

```text
Dungeon Style municipal equipment:
strong simple silhouette, aged off-white shell, deep black joints/chassis, one limited rust-red or red-white identification zone, clear tool/function geometry, visible repair panel, hard cel shadow blocks, very low decorative armor and micro-greeble. Equipment must look municipal/industrial rather than military hero mecha unless Canon explicitly says otherwise.
```

---

# 07｜Text / slogan prompt rules

Use only if the scene benefits from text.

```text
Text is physical in-world civic graphics integrated into the structure. One main identifier or one main slogan at a time. Large readable Chinese characters, industrial/public-infrastructure placement, muted rust-red or off-white depending surface contrast. No floating title, no poster overlay, no explanatory paragraphs, no tiny technical text wall.
```

Current master examples:

- `第二新重庆市` — municipal identity / in-world structure marking;
- `科学引领未来` — civic slogan example already validated in the style master.

Do not assume these words belong in every scene.

---

# 08｜Universal negative prompt

```text
no photorealism,
no glossy 3D hard-surface render,
no dense hard-SF kitbash,
no cyberpunk neon,
no luxury spacecraft aesthetic,
no dense tiny windows,
no excessive tiny lights,
no endless small panel seams,
no dense pipe bundles,
no dense antennas,
no high-frequency star noise,
no excessive greeble,
no soft pastel rendering,
no painterly fog dependence,
no random red decoration,
no candy stripe aesthetic,
no giant floating title text,
no infographic layout,
no technical paragraph labels,
no unexplained new architecture,
no story-incompatible spectacle,
no scale drift,
no bridge scale inflation
```

---

# 09｜Style routing reminder

`DUNGEON STYLE` is the default **new setting-art** route.

It does **not** supersede `OSHII STYLE`.

If the user asks for Oshii-style rendering, use the preserved Oshii lane rather than trying to hybridize both by default.

Only combine visual lanes when the user explicitly requests a hybrid.
