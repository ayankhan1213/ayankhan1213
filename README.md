<h1 align="center">Hi there, I'm Ayan Khan 👋</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=61DAFB&center=true&vCenter=true&width=600&lines=Full+Stack+MERN+Developer;Building+Scalable+Web+Applications;Always+Learning%2C+Always+Building;Let's+Connect+and+Collaborate!" alt="Typing SVG" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=ayankhan1213&icon=0&color=0d1117&style=flat-square" alt="Profile views" />
  <img src="https://img.shields.io/github/followers/ayankhan1213?label=Followers&style=flat-square&color=0d1117" alt="GitHub followers" />
  <img src="https://img.shields.io/badge/Status-Available%20for%20Hire-brightgreen?style=flat-square" alt="Status" />
</p>

---

### 🐍 Contribution Snake

<p align="center">
  <img src="https://raw.githubusercontent.com/ayankhan1213/ayankhan1213/output/github-contribution-grid-snake-dark.svg" alt="Contribution Snake animation" />
</p>

<p align="center">
  <i>This snake animates your real contribution graph. It updates automatically every day via GitHub Actions.</i>
</p>

<details>
<summary><b>📌 Setup Instructions for Snake Animation</b></summary>

Add this workflow file (`.github/workflows/snake.yml`) to your repository:

```yaml
name: Generate Snake Animation

on:
  schedule:
    - cron: "0 0 * * *"  # Runs daily at midnight
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: Platane/snk@v3
        with:
          github_user_name: ayankhan1213
          outputs: |
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
      - uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
