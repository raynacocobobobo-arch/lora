# 《重庆时间》女科长 FACE PROMPT V2 — 任务执行提示词包

- Updated: 2026-09-04
- Status: `ACTIVE / EXECUTION PROMPT PACKAGE`
- Use with: `FEMALE-CHIEF-VISUAL-PROFILE-V2.md` + `2026-09-04-FEMALE-CHIEF-FACE-LOCK-V2.md`

---

# 01｜先决规则

此提示词用于**修订当前已存在的人物脸**，不是从零设计新角色。

必须同时使用原始近景图（身份主锚点）与原始全身图（体态 / 服装 / 年龄副锚点）。仓库内的 JPG 只作为移交预览；真正高质量编辑时，如接手会话没有原始高分辨率图，先请用户补传原图，不要从预览图重新发明人物。

默认规则：

> **Preserve identity first. Improve facial specificity second. Style comes after identity.**

---

# 02｜中文主提示词 — 近景修脸

以提供的女科长近景原始基准图作为绝对人物身份母图，并同时参考全身原始基准图锁定年龄、体态、宇航服和整体气质。

这不是重新设计一个新角色，也不是随机生成一个更漂亮的女性。必须保留当前人物约 80–85% 的身份连续性，只允许约 15–20% 的脸部结构优化。

完整保留当前头型、脸宽大关系、发际线、五官基本落点、低位马尾、视觉年龄、白色轻型宇航服、颈环、背景、镜头、整体动画电影帧画风和材质质感。

只优化脸部：眼裂横向略拉长约 5–8%，上眼睑更平、更利落，下眼睑减少圆弧，外眼角仅轻微上扬 1–2 度；虹膜视觉尺寸缩小约 8–12%，避免少女大眼感。眉毛略加粗但保持自然女性眉，眉眼距离略收紧，眉峰克制，不做攻击性上挑眉。加强鼻根到鼻梁的体积结构，但不要做高挺网红鼻。嘴部横向略增加约 5–8%，保留成年女性自然唇量，嘴角平静克制。下颌增加非常轻微的结构转折，但不能加宽、不能变方、不能变男性化，下巴不能变尖。

允许极轻微自然左右不对称，让脸摆脱美容式镜像平均，但不得出现大小眼或五官歪斜。

人物气质应是：约 30 岁的东亚女性，漂亮但不网红，温和但不柔弱，安静、清醒、克制、有判断力，有一点疲惫和距离感。她不是在摆冷脸，而是在观察，并且已经理解了眼前发生的事情。

沿用当前低调方向性硬光：亮侧约 -1EV，暗侧约 -2EV，一侧眼窝可以进入暗部，鼻影明确，但必须保留额头、眉骨、眼窝、鼻梁、鼻翼、唇部、下巴的结构层次，不能把整张脸一起压成灰。

最终目标：还是同一个女科长，但脸具有稳定、长期可复用的主角辨识度；第一眼克制，第二眼已经能记住。

---

# 03｜English master prompt — face revision

Use the provided original close-up image of the Female Chief as the absolute identity master, and use the original full-body reference as the secondary anchor for age, body proportions, suit design, and overall character presence.

This is NOT a redesign and NOT a request to generate a different, prettier woman. Preserve approximately 80–85% identity continuity and limit the facial revision to roughly 15–20%.

Keep the current head shape, overall face width, hairline, fundamental landmark placement, low ponytail, apparent age, white lightweight pressure suit, neck ring, background, framing, cinematic animation rendering, and material treatment unchanged.

Revise only the facial structure: lengthen the eye opening horizontally by roughly 5–8%; make the upper eyelid flatter and more decisive; reduce the roundness of the lower eyelid; raise the outer corner only about 1–2 degrees; reduce the apparent iris size by roughly 8–12% to remove juvenile large-eye softness. Make the eyebrows slightly fuller while keeping them natural and feminine; slightly reduce brow-to-eye distance; keep the arch restrained and non-aggressive. Strengthen the nasion-to-bridge structure without creating a high sculpted influencer nose. Widen the mouth horizontally by roughly 5–8% while preserving natural adult female lip volume and neutral mouth corners. Add a subtle structural break to the jawline without widening or squaring the jaw, and do not sharpen the chin.

Allow extremely subtle natural asymmetry between eyelids, brows, or mouth corners so the face does not feel cosmetically mirrored, but do not introduce visible eye-size mismatch or facial distortion.

The character should read as an East Asian woman around thirty: attractive but not influencer-like, gentle but not weak, quiet, lucid, restrained, observant, and decisive, with a trace of fatigue and emotional distance. She is not posing as cold or aggressive; she is watching and has already understood what is happening.

Preserve the existing low-key directional hard-light logic: approximately -1 EV on the lit side and -2 EV on the shadow side. One eye socket may fall into shadow and the nose shadow should remain clear, but the structural sequence of forehead, brow ridge, orbit, nasal bridge, nostril plane, lips, and chin must remain readable rather than collapsing into flat gray.

Final target: unmistakably the same Female Chief, now with stable protagonist-level facial specificity. Restrained at first glance, memorable at second glance.

---

# 04｜Negative / 禁止项

Do NOT:

- replace her with a different attractive woman;
- beautify toward an influencer face;
- make her younger or more juvenile;
- enlarge the eyes or irises;
- create a V-shaped jaw or pointed chin;
- create a tall sculpted cosmetic nose;
- add aggressive arched brows;
- masculinize the brow ridge, eye socket, jaw, or chin;
- turn her into a military officer / female warrior archetype;
- add scars, beauty marks, heterochromia, facial tattoos, or other recognition gimmicks;
- change the low ponytail into short hair;
- change the suit, neck ring, body proportions, pose, background, camera, or composition;
- change the established animation-film rendering style;
- add excessive micro-texture, dirty noise, fragmented brushwork, or high-frequency detail;
- make the face photorealistic if the source remains stylized animation.

---

# 05｜身份锁定补充口令

模型容易自由发挥时，在提示词最前加入：

> **IDENTITY PRESERVATION IS THE HIGHEST PRIORITY. THIS IS A CONTROLLED FACE REVISION OF THE PROVIDED CHARACTER ASSET, NOT A NEW CHARACTER GENERATION.**

容易改服装 / 背景时加入：

> **DO NOT REDESIGN OR RECONSTRUCT ANY NON-FACIAL ELEMENT. ALL NON-FACIAL STRUCTURES SHOULD REMAIN AS CLOSE TO THE SOURCE AS THE EDITING SYSTEM ALLOWS.**

容易网红化时加入：

> **NO BEAUTY-FILTER CONVERGENCE: avoid generic influencer proportions, oversized eyes, tiny nose, tiny mouth, pointed chin, porcelain skin, cosmetic symmetry, and glamour portrait lighting.**

---

# 06｜执行顺序

接手 ChatGPT：

1. 先读 Handoff 与 Face Lock；
2. 先确认理解“只修脸，不换人”；
3. 用户没有明确说“开始出图”之前，不主动生成；
4. 用户明确开始后，先处理原始近景 Anchor；
5. 单次一个候选；
6. 用户通过近景后才处理全身；
7. 全身通过后再建立 45° / 侧面身份资产。

---

# 07｜快速短提示词

> **Same woman, same identity, same low ponytail, same suit, same background, same animation-film style. Controlled 15–20% facial revision only: slightly longer eyes, flatter upper lids, smaller irises, slightly tighter brow-eye spacing, stronger natural nose bridge structure, slightly wider adult mouth, subtle feminine jaw break, natural micro-asymmetry. Around 30, East Asian, restrained, observant, lucid, quietly authoritative, attractive but not influencer-like, no juvenile features, no military-warrior face, no V-jaw, no redesign.**
