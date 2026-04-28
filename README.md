## Contribution Snake

<div align="center">

![Snake animation](https://raw.githubusercontent.com/Prithibi17/Prithibi17/output/github-contribution-grid-snake-dark.svg)

</div>

---

## Required GitHub Action Workflow

Create this file:

```yml id="dr4g1x"
# .github/workflows/snake.yml

name: Generate Snake

on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: Prithibi17
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark

      - uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

---

## Important Fixes

### Make sure:

* Repository name is exactly: `Prithibi17`
* Profile README repo is: `Prithibi17/Prithibi17`
* Actions are enabled
* `output` branch exists
* Workflow has run successfully at least once

---

## After setup:

* Go to Actions tab
* Run `Generate Snake`
* Wait 1–2 minutes
* Refresh profile

---

## Correct Image Path:

```md id="w2lk9n"
![Snake animation](https://raw.githubusercontent.com/Prithibi17/Prithibi17/output/github-contribution-grid-snake-dark.svg)
```

---

Using `raw.githubusercontent.com` fixes the broken image issue caused by blob links.
