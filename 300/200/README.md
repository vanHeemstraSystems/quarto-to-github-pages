# 200 - Publish Command

The ```quarto publish``` command is an easy way to publish locally rendered documents and websites. Before attempting to use ```quarto publish``` (either locally or from a GitHub Action) you should be sure to configure the [Source Branch](https://quarto.org/docs/publishing/github-pages.html#source-branch) and [Ignore Output](https://quarto.org/docs/publishing/github-pages.html#ignoring-output) as described below.

**Windows Compatibility**

Many users have reported problems with using ```quarto publish gh-pages``` on Windows systems. We are investigating and hoping to have a fix for this soon, but in the meantime we recommend against using ```quarto publish gh-pages``` on Windows (rather, try using the [Render to ```docs```](https://quarto.org/docs/publishing/github-pages.html#render-to-docs) workflow described above).

## 100 - Source Branch

See [README.md](./100/README.md)

## 200 - Ignore Output

See [README.md](./200/README.md)
