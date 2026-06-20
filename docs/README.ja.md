# Japanese Handdrawn Illustrations

<p align="center">
  <a href="../README.md">🇬🇧 English</a> ·
  <a href="README.zh-CN.md">🇨🇳 简体中文</a> ·
  <a href="README.ja.md">🇯🇵 日本語</a> ·
  <a href="README.fr.md">🇫🇷 Français</a> ·
  <a href="README.ko.md">🇰🇷 한국어</a>
</p>

<p align="center">
  <strong>ワンクリック多言語ページ：</strong>
  <a href="https://2023anita.github.io/japanese-handdrawn-illustrations/">GitHub Pages を開く</a>
</p>

![Japanese handdrawn illustration skill workroom](../assets/demo/01-skill-workroom.png)

中国語の記事、ノート、教材、ワークフロードキュメントを、静かで余白のある日本風エディトリアル手描きイラストに変換する Codex Skill です。

これは単なる万能プロンプトではありません。スタイル DNA、固定キャラクター、構図パターン、プロンプトテンプレート、QA ルールをまとめた、再利用可能なビジュアルワークフローです。

## 多言語体験

GitHub の README では JavaScript を実行できないため、このリポジトリでは 2 つの翻訳導線を用意しています。

- **README の言語リンク**：上の国旗をクリックして翻訳版を開きます。
- **ライブ展示ページ**：GitHub Pages ではページ内で即時に言語を切り替えられます。

## 特長

多くの AI 画像プロンプトは壊れやすく、一度はうまくいっても、次の記事では雰囲気がぶれがちです。

この skill は、イラスト生成をより保守しやすい形にします。

- **再利用できるビジュアルシステム**：単発の prompt ではなく、構造化された skill。
- **一貫したキャラクター**：`小旅人` がスタイルの軸になります。
- **記事優先の流れ**：装飾ではなく、本文の認知的な要点から始めます。
- **QA 内蔵**：アニメ調、PPT 風、詰め込みすぎ、読めないラベルを避けます。
- **中国語コンテンツ向け**：中国語の短い手書きラベルと本文挿絵に最適化。
- **改造しやすい**：fork してキャラクターや style DNA を差し替えられます。

## Demo

| Skill system | Workflow | Prompt cards | QA guardrail |
|---|---|---|---|
| ![](../assets/demo/01-skill-workroom.png) | ![](../assets/demo/02-content-to-image-workflow.png) | ![](../assets/demo/03-prompt-system-cards.png) | ![](../assets/demo/04-qa-umbrella.png) |

## Install

```bash
cp -R "skills/japanese-handdrawn-illustrations" "$HOME/.codex/skills/"
```

Then start a new Codex session and invoke:

```text
Use $japanese-handdrawn-illustrations to design and generate Japanese hand-drawn illustrations for this Chinese article.
```

## License

MIT
