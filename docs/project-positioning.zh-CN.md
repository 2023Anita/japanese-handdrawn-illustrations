# 项目说明与传播定位

## 一句话介绍

`japanese-handdrawn-illustrations` 是一个 Codex Skill：它把中文文章、教学材料、学习笔记和方法论内容，转化成安静、清爽、带日式手账气质的正文配图。

它不是一段万能提示词，而是一套可维护的视觉生成工作流。

## 1. 项目的优势

### 1.1 从 prompt 升级到 skill

普通生图 prompt 的问题是：一次有效，后续容易漂移，难以复用，也难以解释为什么某张图不合格。

这个项目把生图经验拆成了稳定结构：

- `SKILL.md`：定义触发场景、工作流和交付方式。
- `style-dna.md`：定义日式手绘风格边界。
- `character-ip.md`：定义默认角色“小旅人”。
- `composition-patterns.md`：定义可复用构图模式。
- `prompt-template.md`：把策略转成单张生图提示词。
- `qa-checklist.md`：生成后检查和迭代。

### 1.2 中文内容友好

很多视觉 prompt 面向英文海报或商业插画，这个项目更适合中文正文配图：

- 支持中文短标注。
- 适合公众号、博客、Obsidian、Notion、医学科普和教学材料。
- 关注“认知锚点”，不是给每段文字平均配图。

### 1.3 风格明确，但不绑定具体艺术家

项目定义的是“日式编辑插图 / 手账草图 / 温柔留白”的视觉方向，而不是模仿某位具体艺术家或动画工作室。

这让项目更安全，也更容易开源传播。

### 1.4 有角色 IP，输出更稳定

默认角色“小旅人”不是装饰物，而是图里的动作主体。

它可以：

- 整理便签
- 撑伞保护注意力
- 在车站转乘
- 把信息放进便当分格
- 在小房间里维护一个工作系统

这让不同图片之间有连续感，也更适合形成长期内容品牌。

### 1.5 自带 QA，减少跑偏

项目明确拒绝：

- 日漫 / 二次元
- 大眼萌系角色
- 儿童绘本
- 商业海报
- PPT 信息图
- 复杂流程图
- 具体艺术家或工作室复刻

这比“请画得高级一点”更可执行。

## 2. 涉及的技术细节

### 2.1 Codex Skill 结构

项目遵循 Codex Skill 的标准结构：

```text
skills/japanese-handdrawn-illustrations/
├── SKILL.md
├── agents/openai.yaml
├── references/
│   ├── style-dna.md
│   ├── character-ip.md
│   ├── composition-patterns.md
│   ├── prompt-template.md
│   └── qa-checklist.md
└── assets/examples/
```

这种结构的好处是渐进加载：

- Codex 默认只看到 skill 的名称和描述。
- 触发 skill 后读取 `SKILL.md`。
- 需要更细规则时再读取 `references/`。

这比把所有规则塞进一个超长 prompt 更省 token，也更容易维护。

### 2.2 提示词工程不是单点 prompt，而是模块化约束

项目把提示词拆成几个模块：

- Visual DNA：背景、线条、颜色、留白、禁忌。
- Character IP：小旅人的外形、性格、动作职责。
- Theme：当前文章配图主题。
- Structure type：桌面整理、窗边观察、车站转乘等构图模式。
- Core idea：这张图只表达一个核心意思。
- Composition：具体画面安排。
- Chinese labels：控制中文标注数量和长度。
- Constraints：防止跑偏的硬规则。

### 2.3 构图模式库

项目内置 8 种构图方向：

- 桌面整理
- 窗边观察
- 车站转乘
- 便当分格
- 雨伞保护
- 小房间系统
- 手账地图
- 四格生活分镜

这些不是模板复制，而是隐喻生成的约束空间。它帮助模型保持一致，同时保留每次创作的新鲜感。

### 2.4 QA 作为生成闭环

`qa-checklist.md` 把审美判断变成可检查规则：

- 是否 16:9
- 是否有足够留白
- 小旅人是否参与核心动作
- 是否避免日漫/PPT/商业海报
- 中文是否太多或不可读
- 背景是否过脏
- 是否只表达一个核心结构

这让图片生成从“抽卡”更接近“可迭代生产”。

## 3. 如何描述才能吸引更多 Star

### 3.1 不要把它描述成“又一个 prompt”

GitHub 用户对 prompt 仓库已经有疲劳感。更吸引人的说法是：

> A reusable Codex skill that turns Chinese articles into consistent Japanese hand-drawn editorial illustrations.

中文可以说：

> 不是万能提示词，而是一套可复用的正文配图生产系统。

### 3.2 强调解决的问题

建议重点打这几个痛点：

- AI 配图风格不稳定。
- 中文文章配图容易变成 PPT 或商业海报。
- prompt 难复用、难维护。
- 文章配图需要先理解内容，而不是随机装饰。
- 生成后缺少质量检查标准。

### 3.3 强调可 fork 和可改编

这个项目真正有传播力的地方是“模板价值”：

- 可以改成医学科普风格。
- 可以改成小红书手账风。
- 可以改成技术博客插图风。
- 可以换角色 IP。
- 可以扩展构图库。

建议 README 里突出：

> Fork it, replace the character, rewrite the style DNA, and you have your own illustration skill.

### 3.4 GitHub 标题建议

推荐仓库描述：

```text
A Codex skill for generating quiet Japanese hand-drawn illustrations for Chinese articles, notes, and teaching materials.
```

更吸引 Star 的短版：

```text
Turn Chinese articles into consistent Japanese hand-drawn editorial illustrations with a reusable Codex skill.
```

### 3.5 推荐 Topics

```text
codex
codex-skill
ai-art
image-generation
prompt-engineering
chinese-content
illustration
hand-drawn
japanese-style
knowledge-management
obsidian
teaching-materials
```

### 3.6 推荐 README 开头

建议开头直接讲差异：

```text
Most AI image prompts are fragile. They work once, drift quickly, and are hard to reuse.

This project turns a visual style into a reusable Codex skill: style DNA, character IP, composition patterns, prompt templates, and QA rules.
```

这个表达比“这是一个生成日式手绘图的 prompt”更有工程感，也更容易吸引开发者 Star。
