# Japanese Handdrawn Illustrations

<p align="center">
  <a href="../README.md">🇬🇧 English</a> ·
  <a href="README.zh-CN.md">🇨🇳 简体中文</a> ·
  <a href="README.ja.md">🇯🇵 日本語</a> ·
  <a href="README.fr.md">🇫🇷 Français</a> ·
  <a href="README.ko.md">🇰🇷 한국어</a>
</p>

<p align="center">
  <strong>Page multilingue en un clic :</strong>
  <a href="https://2023anita.github.io/japanese-handdrawn-illustrations/">ouvrir GitHub Pages</a>
</p>

![Japanese handdrawn illustration skill workroom](../assets/demo/01-skill-workroom.png)

Un Codex Skill qui transforme des articles chinois, des notes, des supports pédagogiques et des documents de workflow en illustrations éditoriales dessinées à la main, calmes et inspirées d'une esthétique japonaise.

Ce n'est pas un simple méga prompt. Le projet structure un workflow visuel réutilisable : ADN de style, personnage récurrent, modèles de composition, templates de prompts et règles de QA.

## Expérience multilingue

Les README GitHub ne peuvent pas exécuter JavaScript. Ce dépôt propose donc deux niveaux de traduction :

- **Liens de langue dans le README** : cliquez sur un drapeau pour ouvrir la version traduite.
- **Page de démonstration** : la page GitHub Pages permet de changer de langue instantanément dans la même page.

## Points forts

La plupart des prompts d'images IA sont fragiles : ils fonctionnent une fois, dérivent rapidement et sont difficiles à réutiliser.

Ce skill rend le processus plus maintenable :

- **Système visuel réutilisable** : pas seulement un prompt, mais un skill structuré.
- **Personnage cohérent** : `小旅人` ancre le style.
- **Workflow centré sur l'article** : on part des points cognitifs importants, pas d'une décoration aléatoire.
- **QA intégrée** : évite les dérives anime, les diagrammes de type PPT, les compositions trop chargées et les labels illisibles.
- **Adapté au contenu chinois** : optimisé pour les annotations courtes en chinois.
- **Facile à adapter** : fork, remplacement du personnage, réécriture du style DNA.

## Demo

| Skill system | Workflow | Prompt cards | QA guardrail |
|---|---|---|---|
| ![](../assets/demo/01-skill-workroom.png) | ![](../assets/demo/02-content-to-image-workflow.png) | ![](../assets/demo/03-prompt-system-cards.png) | ![](../assets/demo/04-qa-umbrella.png) |

## Installation

```bash
cp -R "skills/japanese-handdrawn-illustrations" "$HOME/.codex/skills/"
```

Puis démarrez une nouvelle session Codex et utilisez :

```text
Use $japanese-handdrawn-illustrations to design and generate Japanese hand-drawn illustrations for this Chinese article.
```

## Licence

MIT
