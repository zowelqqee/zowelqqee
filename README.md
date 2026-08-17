<p align="center">
  <picture>
    <source media="(prefers-color-scheme: light)" srcset="https://www.gitskins.com/api/section/hero?username=zowelqqee&theme=github-dark&mode=light" />
    <img src="https://www.gitskins.com/api/section/hero?username=zowelqqee&theme=github-dark" alt="zowelqqee hero section" />
  </picture>
</p>
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: light)" srcset="https://www.gitskins.com/api/section/stats?username=zowelqqee&theme=github-dark&mode=light" />
    <img src="https://www.gitskins.com/api/section/stats?username=zowelqqee&theme=github-dark" alt="zowelqqee stats section" />
  </picture>
</p>
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: light)" srcset="https://www.gitskins.com/api/section/projects?username=zowelqqee&theme=github-dark&mode=light" />
    <img src="https://www.gitskins.com/api/section/projects?username=zowelqqee&theme=github-dark" alt="zowelqqee projects section" />
  </picture>
</p>
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: light)" srcset="https://www.gitskins.com/api/section/social?username=zowelqqee&theme=github-dark&mode=light" />
    <img src="https://www.gitskins.com/api/section/social?username=zowelqqee&theme=github-dark" alt="zowelqqee social section" />
  </picture>
</p>

name: Generate contribution snake

on:
  schedule:
    - cron: "0 3 * * *"
  workflow_dispatch:

permissions:
  contents: write

jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10

    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: zowelqqee
          outputs: |
            dist/github-snake.svg?color_snake=#7c3aed&color_dots=#161b22,#312e81,#4338ca,#7c3aed,#c084fc
            dist/github-snake-dark.svg?color_snake=#22d3ee&color_dots=#0d1117,#164e63,#0891b2,#22d3ee,#a5f3fc

      - uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

<!-- Sections: Header, Heatmap, GitHub Stats, Projects, Connect -->
