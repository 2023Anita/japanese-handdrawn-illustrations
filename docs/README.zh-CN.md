# Japanese Handdrawn Illustrations

<p align="center">
  <a href="../README.md">🇬🇧 English</a> ·
  <a href="README.zh-CN.md">🇨🇳 简体中文</a> ·
  <a href="README.ja.md">🇯🇵 日本語</a> ·
  <a href="README.fr.md">🇫🇷 Français</a> ·
  <a href="README.ko.md">🇰🇷 한국어</a>
</p>

<p align="center">
  <strong>一键切换语言展示页：</strong>
  <a href="https://2023anita.github.io/japanese-handdrawn-illustrations/">打开 GitHub Pages</a>
</p>

![日式手绘 Codex Skill 工作间](../assets/demo/01-skill-workroom.png)

一个 Codex Skill：把中文文章、笔记、教学材料和工作流文档，转化成安静、清爽、带日式编辑插图气质的手绘正文配图。

它不是一段万能提示词，而是一套可复用的视觉工作流：风格 DNA、固定角色、构图模式、提示词模板和 QA 检查。

## 多语言体验

GitHub README 不能运行 JavaScript，所以这个仓库提供两层翻译：

- **README 语言链接**：点击上方国旗打开对应语言文档。
- **在线展示页**：GitHub Pages 支持页面内一键切换语言。

## 项目优势

大多数 AI 生图提示词都很脆弱：一次有效，后续容易漂移，也很难跨文章复用。

这个 skill 让正文配图流程更可维护：

- **可复用视觉系统**：不是单一 prompt，而是结构化 skill。
- **稳定角色 IP**：默认角色 `小旅人` 让图像更一致。
- **正文优先**：先找文章里的认知锚点，而不是随机装饰。
- **内置 QA**：避免日漫跑偏、PPT 化、画面太满和中文不可读。
- **中文内容友好**：适合中文短标注和中文正文配图。
- **轻量可改编**：很容易 fork、替换角色、重写风格 DNA。

## Demo

| Skill 系统 | 工作流 | Prompt 卡片 | QA 防护 |
|---|---|---|---|
| ![](../assets/demo/01-skill-workroom.png) | ![](../assets/demo/02-content-to-image-workflow.png) | ![](../assets/demo/03-prompt-system-cards.png) | ![](../assets/demo/04-qa-umbrella.png) |

## 安装

```bash
cp -R "skills/japanese-handdrawn-illustrations" "$HOME/.codex/skills/"
```

然后在新的 Codex 会话中调用：

```text
Use $japanese-handdrawn-illustrations to design and generate Japanese hand-drawn illustrations for this Chinese article.
```

## License

MIT
