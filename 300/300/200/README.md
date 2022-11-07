# 200 - Publish Action

Add a ```publish.yml``` GitHub Action to your project by creating this YAML file and saving it to ```.github/workflows/publish.yml```:

```
on:
  workflow_dispatch:
  push:
    branches: main

name: Quarto Publish

jobs:
  build-deploy:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - name: Check out repository
        uses: actions/checkout@v2

      - name: Set up Quarto
        uses: quarto-dev/quarto-actions/setup@v2

      - name: Render and Publish
        uses: quarto-dev/quarto-actions/publish@v2
        with:
          target: gh-pages
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```
.github/workflows/publish.yml

Once you’ve done this, check all of the newly created files (including the ```_freeze``` directory) into your repository and then push to GitHub. A GitHub Pages site will be created for your repository, and every time you push a new change to the repository it will be automatically rebuilt to reflect the change. Consult the **Pages** section of your repository **Settings** to see what the URL and publish status for your site is.
