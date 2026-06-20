# 生图提示词模板

每张图单独生成。根据正文内容替换变量，不要把多张图拼在一起。

```text
Generate one standalone 16:9 horizontal Chinese article illustration.

Visual DNA:
Quiet Japanese editorial hand-drawn illustration. Pure white or very pale warm off-white background. Minimal black ink line art with thin, slightly wobbly hand-drawn lines. Lots of empty space. Soft muted watercolor accents only in small areas: pale blue, soft pink, sage green, warm beige, or light orange. Gentle zine-like sketch and notebook feeling. Clean, airy, calm, and lightly poetic. No gradients, no shadows, no heavy paper texture, no noisy vintage paper, no complex background, no commercial vector style, no anime, no manga, no big-eyed character, no cute mascot poster, no children's picture book, no PPT infographic look, no realistic UI.

Recurring character required:
小旅人, a small quiet hand-drawn traveler figure with simple black line art, plain coat or scarf or small bag, minimal face, calm serious expression, slightly awkward but gentle. 小旅人 must perform the core conceptual action, not decorate the scene. Make 小旅人 quiet, observant, and useful to the metaphor, not cute or theatrical.

Theme:
{正文配图主题}

Structure type:
{结构类型：桌面整理 / 窗边观察 / 车站转乘 / 便当分格 / 雨伞保护 / 小房间系统 / 手账地图 / 四格生活分镜}

Core idea:
{这张图要表达的核心意思}

Composition:
{具体画面：小旅人在哪里、正在做什么、主要日常物件是什么、信息或状态如何变化}

Suggested elements:
{元素1} / {元素2} / {元素3} / {元素4}

Chinese handwritten labels:
{标注词1} / {标注词2} / {标注词3} / {标注词4} / {可选标注词5}

Color use:
Black for main line art, character, and text. Pale blue for observation, feedback, or learning state. Soft pink for emotion, care, or gentle emphasis. Sage green for recovery, stability, health, or growth. Warm beige or light orange for paths, warmth, or subtle highlights. Use only 1-2 accent colors if enough.

Constraints:
One image explains only one core structure. Keep the main subject around 35%-55% of the canvas. Preserve at least 40% blank space. Use at most 4-7 short handwritten Chinese labels. Do not write a title in the top-left corner. Do not write the structure type on the image. Do not make it a formal diagram, course slide, dense explainer, anime illustration, manga panel, children's book, or commercial poster. Do not copy prior examples or reuse known compositions unless explicitly requested; invent a fresh everyday metaphor for this specific article. It should be clear but not instructional, gentle but not childish, Japanese hand-drawn in mood but not an imitation of any specific artist or studio.
```

## 图像编辑提示

去掉左上角标题：

```text
Edit the provided image. Remove only the handwritten title "{要删除的文字}" and its underline from the top-left corner. Fill that area with the same clean white or very pale warm off-white background, matching the surrounding blank space. Preserve everything else exactly: character, labels, objects, line style, composition, aspect ratio, and image quality. Do not add any new text or objects.
```

增强角色参与感：

```text
Regenerate this illustration with the same core meaning and simple layout, but make 小旅人 more central to the conceptual action. 小旅人 should be doing the quiet everyday action that explains the idea, not standing beside the scene. Keep it sparse, calm, hand-drawn, lightly Japanese editorial in mood, and not cute.
```

降低日漫感：

```text
Regenerate this illustration with the same core meaning, but remove all anime, manga, big-eyed, cute mascot, or children's book qualities. Use quiet Japanese editorial notebook sketch style: thin black hand-drawn lines, pale off-white background, sparse muted watercolor accents, lots of empty space, and simple Chinese handwritten labels.
```
