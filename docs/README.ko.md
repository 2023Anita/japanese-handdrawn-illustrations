# Japanese Handdrawn Illustrations

<p align="center">
  <a href="../README.md">🇬🇧 English</a> ·
  <a href="README.zh-CN.md">🇨🇳 简体中文</a> ·
  <a href="README.ja.md">🇯🇵 日本語</a> ·
  <a href="README.fr.md">🇫🇷 Français</a> ·
  <a href="README.ko.md">🇰🇷 한국어</a>
</p>

<p align="center">
  <strong>원클릭 다국어 쇼케이스:</strong>
  <a href="https://2023anita.github.io/japanese-handdrawn-illustrations/">GitHub Pages 열기</a>
</p>

![Japanese handdrawn illustration skill workroom](../assets/demo/01-skill-workroom.png)

중국어 기사, 노트, 교육 자료, 워크플로 문서를 조용하고 여백이 많은 일본식 에디토리얼 손그림 삽화로 바꾸는 Codex Skill입니다.

이 프로젝트는 하나의 만능 프롬프트가 아닙니다. 스타일 DNA, 반복 캐릭터, 구도 패턴, 프롬프트 템플릿, QA 규칙을 묶은 재사용 가능한 시각 워크플로입니다.

## 다국어 경험

GitHub README에서는 JavaScript를 실행할 수 없으므로, 이 저장소는 두 가지 번역 방식을 제공합니다.

- **README 언어 링크**: 위의 국기를 클릭해 번역 문서를 엽니다.
- **라이브 쇼케이스 페이지**: GitHub Pages에서 같은 페이지 안에서 즉시 언어를 전환합니다.

## 장점

대부분의 AI 이미지 프롬프트는 쉽게 흔들립니다. 한 번은 잘 작동해도 다음 글에서는 스타일이 빠르게 달라집니다.

이 skill은 삽화 생성 과정을 더 유지보수하기 쉽게 만듭니다.

- **재사용 가능한 시각 시스템**: 단일 prompt가 아니라 구조화된 skill입니다.
- **일관된 캐릭터 IP**: `小旅人`이 스타일을 잡아 줍니다.
- **본문 우선 워크플로**: 무작위 장식이 아니라 글의 핵심 인지 지점에서 시작합니다.
- **내장 QA**: 애니풍, PPT풍, 과밀한 레이아웃, 읽기 어려운 라벨을 피합니다.
- **중국어 콘텐츠 친화적**: 짧은 중국어 손글씨 라벨과 본문 삽화에 최적화되어 있습니다.
- **쉽게 개조 가능**: fork 후 캐릭터와 style DNA를 바꾸면 됩니다.

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
